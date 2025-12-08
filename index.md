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
<!-- <p>
<font size=4><b>Biography</b></font>
</p>
<p>
	My name is <i><b>Dian Ding</b></i>, I received the Ph.D in Department of Computer Science and Engineering at <i><b>Shanghai Jiao Tong University</b></i> in 2023, M.S. in the School of Automation Science and Electrical Engineering at <i><b>Beihang University</b></i> in 2019, and the B.S. degree in the School of Information Science and Technology at <i><b>Northwest University</b></i> in 2016. I am currently <i><b>a postdoctoral in the Department of Computer Science and Engineering at Shanghai Jiao Tong University</b></i>. 
</p> -->

<div class="bio-section">
  <h2 class="section-title">Biography</h2>
  
  <div class="bio-container">
    <div class="bio-text">
      <p>
        My name is <span class="highlight">Dian Ding</span>, I received the Ph.D in School of Computer Science at <span class="highlight">Shanghai Jiao Tong University</span> in 2023, under the supervision of Prof. Guangtao Xue and Assoc. Prof. Yichao Chen.
      </p>
      <p>
        I am currently <span class="highlight">a postdoctoral researcher</span> in School of Computer Science and Engineering at <span class="highlight">Shanghai Jiao Tong University</span>. My research focuses on <span class="highlight">intelligent sensing and computing systems for the Internet of Things</span>.
      </p>
  </div>
</div>

<style>
/* Bio Section Styles */
.bio-section {
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  line-height: 1.6;
  max-width: 1400px !important; /* 从1000px改为1400px */
  width: 95% !important; /* 添加响应式宽度 */
  margin: 0 auto 40px !important;
  padding: 30px !important; /* 增加内边距 */
  /* 去掉背景色和阴影，保持与Publications一致 */
  background: transparent !important;
  border-radius: 0 !important;
  box-shadow: none !important;
}

.section-title {
  color: #2c3e50;
  font-size: 1.8em;
  font-weight: 600;
  margin-bottom: 25px;
  text-align: left;
}

.bio-container {
  background: white;
  border-radius: 12px;
  box-shadow: 0 6px 25px rgba(0, 0, 0, 0.08);
  padding: 35px;
  border: 1px solid #e9ecef;
  max-width: 1300px;
  margin: 0 auto;
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
@media (max-width: 1400px) {
  .bio-section {
    max-width: 95% !important;
    margin: 20px auto 40px !important;
    padding: 25px !important;
  }
}

@media (max-width: 1200px) {
  .bio-section {
    max-width: 98% !important;
    padding: 20px !important;
  }
  
  .bio-container {
    padding: 25px;
  }
}

@media (max-width: 768px) {
  .bio-section {
    max-width: 100% !important;
    margin: 10px auto 30px !important;
    padding: 15px !important;
  }
  
  .bio-container {
    padding: 20px;
  }
  
  .bio-text p {
    font-size: 0.95em;
  }
}

@media (max-width: 480px) {
  .bio-section {
    padding: 10px !important;
  }
  
  .bio-container {
    padding: 15px;
  }
}
</style>






