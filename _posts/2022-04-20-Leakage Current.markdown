---
layout: post
title:  ACM IMWUT 2021 - User identification based on leakage current
date:   2022-04-20 
categories: jekyll update
sjtu_picture:
  src: /assets/img/title.png
  alt: website picture
---

### Abstract

The convenience of laptops brings with it the risk of information leakage, and conventional security systems based on the password or the explicit biometric do little to alleviate this problem. Biometric identification based on anatomical features provides far stronger security; however, a lack of suitable sensors on laptops limits the applicability of this technology. In this paper, we developed a behavior-irrelevant user identification system applicable to laptops with a metal casing. The proposed scheme, referred to as LeakPrint, is based on leakage current, wherein the system uses an earphone to capture current leaking through the body and then transmits the corresponding signal to a server for identification. The user identification is achieved via denoising, dimension reduction, and feature extraction. Compared to other biometric identification methods, the proposed system is less dependent on external hardware and more robust to environmental noise. The experiments in real-world environments demonstrated that LeakPrint can verify user identity with high accuracy (93.6%), while providing effective defense against replay attacks (96.5%) and mimicry attacks (90.9%).

### Contents
1. [Background](#background)
	* [Leakage Current](#leakage-current)
    * [User Identification](#user-identification)
2. [System](#system)
3. [Evaluation](#evaluation)
4. [Reference](#reference)

### Background

#### Leakage Current

As a laptop with a metal casing (such as a MacBook) is connected to a power source, the metal casing of the laptop will carry the leakage current from the adapter [1]. This leakage current comes from the Y-capacitor of the adapter’s safety capacitor, which is part of the EMI (Electromagnetic interference) filtering circuit of the switching power supply to eliminate common mode interference and improve electro- magnetic compatibility, and is usually configured on both the high and low voltage sides of the SMPS (switch mode power supply). As a common mode capacitor, grounding of the Y capacitor generates leakage current [26]. The leakage current in the metal casing can be written as:

<center><img src="{{ "/assets/img/leakprint/leakage current.png" | absolute_url }}" alt="background" width = "150" height = "80" class="post-pic"/></center>

where the leakage current in the high voltage side is 2πfC_hU_h. f refers to the mains frequency, C_h indicates the size of the capacitor, and Uh indicates the voltage. In the low- voltage side, k is the leakage current constant (about 0.01 to 0.03 depending on the manufacturer), C_l and U_l denote the corresponding Y capacitor and voltage. The Y capacitors used in laptop adapters are typically around 5nF. Therefore, a laptop powered by the 220V /50H z mains generates roughly 0.3mA of leakage current at the casing (U_l = 12V ).

Researchers [2] have used wristbands equipped with electrodes to collect electrical signals from the human body; however, those methods depend entirely on external hardware. We sought to build a more generalizable signal transmission channel between the laptop and user. As shown in Fig. 1(a), with the user’s hands placed on the laptop and the feet on the ground, leakage current flows from the laptop through the human body and eventually into the ground.

<table><tr>
<td><img src="{{ "/assets/img/leakprint/human.png" | absolute_url }}" alt="background" class="post-pic"/></td>
<td><img src="{{ "/assets/img/leakprint/human1.png" | absolute_url }}" alt="background" class="post-pic"/></td>
</tr></table>

<center>Fig.1: Fundamental principle of leakage current: 1(a) Under normal use, leakage current flows from the laptop through the user’s hands into the body and eventually into the ground; 1(b) Earphones can be used to capture the signal for transmission to a server.
</center>

#### User Identification

Leakage current flowing through the body can be affected by the anatomical traits of the individual (e.g., blood vessels, muscle, fat, bone), leading to subtle differences in impedance [3] with corresponding variations in signal attenuation at different frequencies. Preliminary experiments were conducted to verify the feasibility of the system. A MacBook Pro was used to collect data from two volunteers, both of whom were asked to place a hand in the same fixed position on the right side of the touchpad, while data was collected from a single channel of the earphone.

Most of the biometric characteristics were distributed in the high frequency band (stable in 55KHz and 70KHz), as shown in Fig. 2. Samples (duration = 1s) were analyzed in terms of frequency distribution after FFT (Fast Fourier Transform). As shown in Fig. 3(a), different users presented obvious differences in distribution and amplitude at some frequencies. As shown in Fig. 3(b), the two samples obtained from the same volunteer were extremely similar in terms of frequency distribution, with only slight differences in magnitude.

<center><img src="{{ "/assets/img/leakprint/con_cur_.png" | absolute_url }}" alt="background" width = "320" height = "240" class="post-pic"/></center>

<center>Fig.2: Spectrum of leakage current showing changes in current captured by an earphone when the user touches the laptop, where the dotted line indicates the time when the use came into contact with the laptop, leading to an increase in signal amplitude in the high frequency band (stable in 55KHz and 70KHz).</center>

<table><tr>
<td><img src="{{ "/assets/img/leakprint/2users.png" | absolute_url }}" alt="background" class="post-pic"/></td>
<td><img src="{{ "/assets/img/leakprint/same user.png" | absolute_url }}" alt="background" class="post-pic"/></td>
</tr></table>

<center>Fig.3: Preliminary experiments: 4(a) Biometric characteristics of 2 different users from the frequency spectrum are highly distinguishable in some frequencies; 4(b) Biometric characteristics of the same user have high consistency. 
</center>

### System

As shown in Fig. 4, after the leakage current detection and frequency domain transformation (FFT), the proposed system is implemented in two phases: registration phase and login phase.
In the registration phase, the system is responsible for collecting samples of legitimate users and training the identification system. After the server receives the leakage current, it preprocesses the current signal. First, we use the signal of idle time as a noise sample and denoise the signal using multi-band spectral subtraction. Second, more than 90% of the user features cannot be used for identification; therefore, LeakPrint uses DC-SIS to filter out the irrelevant features to reduce the computational burden. Finally, the system uses TCN and Triplet Loss to extract behavior-irrelevant features and produce these features as a dataset for each legitimate user.

In the login phase, the system identifies the user by leakage current. First, LeakPrint detects the touch behavior by signal amplitude and preprocesses the signal, including denoising and dimensionality reduction. Then the behavior-irrelevant features are extracted by TCN. Finally, the system compares the user features with those of legitimate users in the dataset to determine the identity of the current user.

<center><img src="{{ "/assets/img/leakprint/system.png" | absolute_url }}" alt="background" width = "600" height = "450" class="post-pic"/></center>

<center>Fig.4: System architecture of LeakPrint.</center>

<!-- #### Preprocess

#### User Identification -->

### Evaluation

LeakPrint was implemented on a MacBook Pro, and a desktop computer was used as the server, as shown in Fig.5. We chose the earphone with metal dust mesh (Meizu) to collect the leakage current. The MacBook was always on charge and placed on the desk. The user wore the earphone normally and touched the MacBook, and the earphone was connected to the server. 

<center><img src="{{ "/assets/img/leakprint/setup.png" | absolute_url }}" alt="background" width = "500" height = "375" class="post-pic"/></center>

<center>Fig.5: Experimental setup of LeakPrint. The unknown user touches the laptop with one hand, the server detects the leakage current via the earphone. We use the third party software Audacity to present the leakage current.</center>

The 15 legitimate users were denoted as (U1,U2,...,U15), and the attackers were denoted as A. The average accuracy of LeakPrint in identifying legitimate users was 92.8% and 93.6% respectively in the two environments. The FAR of attacks was 9.1% and 8.7%, the FRR was 7.2% and 6.4%, and the EER was around 8.6% and 7.1% in the two environments. As shown in Fig. 6(c), we plotted the ROC (Receiver Operator Characteristic) curves consisting of FAR and FRR for the two environments. These results demonstrate that LeakPrint can accurately identify the identity of legitimate users and detect attackers, even under the effects of other influence of other electrical appliances.

<table><tr>
<td><img src="{{ "/assets/img/leakprint/confusion_matrix.png" | absolute_url }}" alt="background" class="post-pic"/></td>
<td><img src="{{ "/assets/img/leakprint/confusion_matrix2.png" | absolute_url }}" alt="background" class="post-pic"/></td>
<td><img src="{{ "/assets/img/leakprint/ROC_paper.png" | absolute_url }}" alt="background" class="post-pic"/></td>
</tr></table>

<center>Fig.6: Micro Benchmarks of LeakPrint. </center>

For more details about *LeakPrint*, please refer to out paper [4].

### Reference

[1]. M. M. Jha, K. B. Naik, and S. P. Das, “Estimation of optimum value of y-capacitor for reducing emi in switch mode power supplies,” Electrical
Power Quality and Utilisation. Journal, 2009.

[2]. Christian Holz and Marius Knaust. 2015. Biometric Touch Sensing: Seamlessly Augmenting Each Touch with Continuous Authentication. In Proceedings of the 28th Annual ACM Symposium on User Interface Software amp; Technology (Charlotte, NC, USA) (UIST ’15). Association for Computing Machinery, New York, NY, USA, 303–312.

[3]. Ivan Martinovic, Kasper B. Rasmussen, Marc Roeschlin, and Gene Tsudik. 2017. Pulse-Response: Exploring Human Body Impedance for Biometric Recognition. Acm Transaction on Information System Security 20, 2 (2017), 6.1–6.31.

[4]. Dian Ding, Lanqing Yang, Yi-Chao Chen, and Guangtao Xue. 2022. Leakage or Identification: Behavior-irrelevant User Identification Leveraging Leakage Current on Laptops. <i>Proc. ACM Interact. Mob. Wearable Ubiquitous Technol.</i> 5, 4, Article 152 (Dec 2021), 23 pages. 