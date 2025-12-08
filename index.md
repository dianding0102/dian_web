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
<p>
<font size=4><b>Biography</b></font>
</p>
<p>
	My name is <i><b>Dian Ding</b></i>, I received the Ph.D in Department of Computer Science and Engineering at <i><b>Shanghai Jiao Tong University</b></i> in 2023, M.S. in the School of Automation Science and Electrical Engineering at <i><b>Beihang University</b></i> in 2019, and the B.S. degree in the School of Information Science and Technology at <i><b>Northwest University</b></i> in 2016. I am currently <i><b>a postdoctoral in the Department of Computer Science and Engineering at Shanghai Jiao Tong University</b></i>. 
</p>

<div class="bio-section">
  <h2 class="section-title">Biography</h2>
  
  <div class="bio-container">
    <div class="bio-text">
      <p>
        My name is <span class="highlight">Dian Ding</span>, I received the Ph.D in Department of Computer Science and Engineering at <span class="highlight">Shanghai Jiao Tong University</span> in 2023, M.S. in the School of Automation Science and Electrical Engineering at <span class="highlight">Beihang University</span> in 2019, and the B.S. degree in the School of Information Science and Technology at <span class="highlight">Northwest University</span> in 2016. 
      </p>
      <p>
        I am currently <span class="highlight">a postdoctoral researcher in the Department of Computer Science and Engineering at Shanghai Jiao Tong University</span>.
      </p>
      
      <div class="contact-info">
        <p><strong>Email:</strong> dian.ding@sjtu.edu.cn</p>
        <p><strong>Office:</strong> Department of Computer Science and Engineering, Shanghai Jiao Tong University</p>
        <p><strong>Links:</strong> 
          <a href="#">Google Scholar</a> | 
          <a href="#">GitHub</a> | 
          <a href="#">CV/Resume</a>
        </p>
      </div>
    </div>
    
    <div class="bio-photo">
      <img src="/assets/img/dian.png" alt="Dian Ding">
      <div class="photo-caption">
        <p><strong>Dian Ding, Ph.D.</strong></p>
        <p>Postdoctoral Researcher</p>
        <p>Shanghai Jiao Tong University</p>
      </div>
    </div>
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






