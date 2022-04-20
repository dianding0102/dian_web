---
layout: post
title:  Handwriting recognition system based on vibration signal
date:   2022-04-20 
categories: jekyll update
---

### Abstract

The efficiency of human-computer interaction is greatly hindered by the small size of the touchscreens on mobile devices, such as smart phones and watches. This has prompted widespread interest in handwriting recognition systems, which can be divided into active and passive systems. Active systems require additional hardware devices to perceive movements of handwriting or the tracking accuracy is not adequate for hand- writing recognition. Passive methods use the acoustic signal of pen rubbing and are susceptible to environmental noise (above 60dB). This paper presents a novel handwriting recognition system based on vibration signals detected by the built-in accelerometer of smart phones. *VibWriter* is highly resistant to interference since the normal environmental noise will not cause the vibration of the accelerometer. Extensive experiments demonstrated the efficacy of the system in terms of accuracy in letter recognition (76.15%) and word recognition (88.14%) when dealing with words of various lengths written by various users in a variety of writing positions under a variety of environmental conditions.


<br />

### Contents
1. [System](#System)
    * [Letter Segmentation](#letter-segmentation)
    * [Letter Recognition](#letter-recognition)
    * [Word Suggestion](#word-suggestion)
2. [Presentation](#presentation)
2. [Reference](#Reference)

### System 

*VibWriter* comprises three modules: letter segmentation, letter recognition, and word suggestion. Vibration signal detected by the built-in accelerometer is first sent to the letter segmentation module to be divided into discrete segments. The letter recognition module identifies the different segments. Finally, the word suggestion module combines the letters into words. 

#### Letter Segmentation

#### Letter Recognition

#### Word Suggestion

### Presentation 

### Reference