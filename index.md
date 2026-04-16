---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
profile_picture:
  src: /assets/img/dian.png
  alt: website picture
cat_picture:
  src: /assets/img/life.png
  alt: website picture
sjtu_picture:
  src: /assets/img/title.png
  alt: website picture
---


<div class="bio-section">
  <h2 class="section-title">Biography</h2>
  
  <div class="bio-container">
    <div class="bio-text">
      <p>
        My name is <span class="highlight">Dian Ding</span>, I received the Ph.D in School of Computer Science at <span class="highlight">Shanghai Jiao Tong University</span> in 2023, under the supervision of Prof. Guangtao Xue and Assoc. Prof. Yi-Chao Chen. I am currently <span class="highlight">a postdoctoral researcher</span> in School of Computer Science and Engineering at <span class="highlight">Shanghai Jiao Tong University</span>. 
      </p>
      <p>
        My research focuses on <span class="highlight">IoT-based intelligent sensing and computing systems</span>, with applications in human–computer interaction and health monitoring. Mobile-device–based multimodal sensing systems are developed to integrate signals including audio, images, millimeter waves, Bluetooth, and human body capacitance. Collected multimodal data are analyzed using deep learning methods—such as convolutional networks, diffusion models, and large language models—for feature extraction, modeling, and system-level understanding, while resource scheduling, model compression, and quantization techniques enable efficient and scalable deployment of computing systems.
      </p>
  </div>
</div>

<style>
/* Bio Section Styles */
.bio-section {
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  line-height: 1.6;
  max-width: 1000px;
  margin: 0 auto 40px;
  padding: 20px;
}

.section-title {
  color: #2c3e50;
  font-size: 1.8em;
  font-weight: 600;
  margin-bottom: 25px;
  text-align: left;
}

.bio-container {
  display: flex;
  gap: 40px;
  align-items: flex-start;
}

.bio-text {
  flex: 1;
}

.bio-text p {
  margin-bottom: 18px;
  color: #4a5568;
  font-size: 1em;
  line-height: 1.7;
}

.highlight {
  color: #4a6ee0;
  font-weight: 600;
  font-style: italic;
}

.bio-photo {
  flex-shrink: 0;
  width: 280px;
  text-align: center;
}

.bio-photo img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  margin-bottom: 12px;
}

.photo-caption p {
  margin: 4px 0;
  color: #4a5568;
  font-size: 0.95em;
}

.photo-caption strong {
  font-size: 1.1em;
}

.contact-info {
  margin-top: 25px;
  padding-top: 20px;
  border-top: 1px solid #e2e8f0;
}

.contact-info p {
  margin-bottom: 10px;
  font-size: 0.95em;
}

.contact-info strong {
  color: #4a6ee0;
  font-weight: 600;
  margin-right: 8px;
}

.contact-info a {
  color: #4a6ee0;
  text-decoration: none;
  margin: 0 4px;
}

.contact-info a:hover {
  text-decoration: underline;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .bio-container {
    flex-direction: column;
    gap: 30px;
  }
  
  .bio-photo {
    width: 100%;
    max-width: 280px;
    margin: 0 auto;
  }
  
  .bio-text p {
    font-size: 0.95em;
  }
}
</style>



