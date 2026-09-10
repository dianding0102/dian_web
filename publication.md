---
layout: default
title: "Publications"
---

<style>
/* 整体页面宽度调整 */
.page-content {
  max-width: 1200px !important;
  width: 95% !important;
  margin: 10px auto !important;
  padding: 0 !important;
  background: transparent !important;
  border-radius: 0 !important;
  box-shadow: none !important;
}

.wrapper {
  max-width: 1200px !important;
  margin: 0 auto !important;
}

.home {
  max-width: 100% !important;
  margin: 0 auto !important;
  padding: 0 !important;
}

/* Publications Section Styles - 简洁紧凑设计 */
.publications-section {
  font-family: 'SF Pro Text', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif;
  line-height: 1.3;
  max-width: 100% !important;
  margin: 0 auto;
  padding: 8px;
  font-size: 1.02em;
  color: #111827;
}

.section-title {
  color: #1a1a1a;
  font-size: 1.55em;
  font-weight: 700;
  margin-bottom: 12px;
  padding-bottom: 4px;
  border-bottom: 1px solid #d1d5db;
  letter-spacing: -0.02em;
  font-family: 'SF Pro Display', -apple-system, BlinkMacSystemFont, sans-serif;
}

.publications-container {
  background: transparent !important;
  border-radius: 0 !important;
  box-shadow: none !important;
  border: none !important;
  padding: 0 !important;
}

.publications-year {
  margin-bottom: 12px;
}

.publications-year:last-child {
  margin-bottom: 0;
}

.publications-year h3 {
  color: #111827;
  font-size: 1.1em;
  font-weight: 650;
  margin-bottom: 8px;
  padding: 6px 10px;
  background: #f9fafb;
  border-radius: 4px;
  border-left: 2px solid #4a6ee0; /* 修改为 #4a6ee0 */
  font-family: 'SF Pro Display', -apple-system, BlinkMacSystemFont, sans-serif;
}

.publication-items {
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.publication-item {
  background: #ffffff;
  border-radius: 4px;
  padding: 10px 12px;
  border: 1px solid #e5e7eb;
  transition: all 0.1s ease;
  position: relative;
}

.publication-item:hover {
  border-color: #d1d5db;
}

.publication-item.award {
  border-left: 2px solid #d97706;
  background: #fff7ed;
}

.pub-content {
  display: flex;
  flex-direction: column;
  gap: 4px;
}

.pub-title {
  color: #1f2937;
  font-size: 1.02em;
  font-weight: 650;
  line-height: 1.35;
  margin-bottom: 0;
}

.pub-authors {
  color: #4b5563;
  font-size: 0.94em;
  line-height: 1.35;
  margin-bottom: 0;
}

.pub-author {
  color: #4b5563;
}

.pub-author.highlight {
  color: #4a6ee0; /* 修改为 #4a6ee0 */
  font-weight: 700;
  background: rgba(74, 110, 224, 0.08); /* 修改为 rgba(74, 110, 224, 0.08) */
  padding: 1px 4px;
  border-radius: 2px;
}

.pub-venue {
  display: flex;
  align-items: center;
  gap: 6px;
  color: #6b7280;
  font-size: 0.9em;
  margin-top: 2px;
  flex-wrap: wrap;
  padding: 4px 0;
  border-top: 1px solid #f3f4f6;
}

.venue-name {
  font-weight: 600;
  color: #374151;
}

.ccf-rank {
  font-weight: 600;
  padding: 1px 6px;
  border-radius: 10px;
  font-size: 0.8em;
  text-transform: uppercase;
  background: #f3f4f6;
  color: #4b5563;
  border: 1px solid #e5e7eb;
}

.pub-correspondence {
  display: flex;
  align-items: center;
  gap: 4px;
  margin-top: 4px;
  padding: 3px 6px;
  background: #f9fafb;
  border-radius: 3px;
  border-left: 1px solid #4a6ee0; /* 修改为 #4a6ee0 */
  font-size: 0.85em;
  color: #4b5563;
}

.corr-text {
  font-weight: 600;
  color: #4a6ee0; /* 修改为 #4a6ee0 */
}

.pub-award-info {
  display: flex;
  align-items: center;
  gap: 6px;
  margin-top: 4px;
  padding: 4px 8px;
  background: #fff7ed;
  border-radius: 3px;
  border-left: 1px solid #d97706;
}

.award-icon {
  font-size: 0.95em;
}

.award-text {
  color: #92400e;
  font-weight: 600;
  font-size: 0.86em;
}

/* 响应式设计 */
@media (max-width: 768px) {
  .page-content {
    max-width: 98% !important;
    margin: 8px auto !important;
  }
  
  .publications-section {
    padding: 6px;
    font-size: 1em;
  }
  
  .section-title {
    font-size: 1.35em;
    margin-bottom: 10px;
  }
  
  .publications-year h3 {
    font-size: 1.05em;
    padding: 5px 8px;
  }
  
  .pub-title {
    font-size: 0.98em;
  }
  
  .pub-authors {
    font-size: 0.92em;
  }
  
  .pub-venue {
    font-size: 0.88em;
    gap: 4px;
  }
  
  .pub-correspondence {
    font-size: 0.83em;
  }
  
  .award-text {
    font-size: 0.84em;
  }
}

@media (max-width: 480px) {
  .publications-section {
    padding: 4px;
  }
  
  .section-title {
    font-size: 1.3em;
    margin-bottom: 8px;
  }
  
  .publications-year h3 {
    font-size: 1em;
  }
  
  .publication-item {
    padding: 8px 10px;
  }
  
  .pub-title {
    font-size: 0.96em;
  }
  
  .pub-authors {
    font-size: 0.9em;
  }
  
  .pub-venue {
    flex-direction: column;
    align-items: flex-start;
    gap: 2px;
    padding: 3px 0;
  }
}
</style>

<div class="page-content">
  <div class="wrapper">
    <div class="home">
      
      <!-- Publications Section -->
      <div class="publications-section">
        <h2 class="section-title">Selected Publications</h2>
        
        <div class="publications-container">

          <!-- 2026年 -->
          <div class="publications-year">
            <h3>2026</h3>
            <div class="publication-items">    

              <!-- ClinBS -->
              <div class="publication-item award">
                <div class="pub-content">
                  <h4 class="pub-title">Listening Through the Noise: Cauchy-Driven Diffusion Bridges for Robust Gastrointestinal Auscultation and Clinical Benchmarking</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Liren Dong</span>, 
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author">Ran Wang</span>, 
                    <span class="pub-author">Peng Li</span>, 
                    <span class="pub-author">Zhenyi Jia</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ICML</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                  <div class="pub-award-info">
                    <span class="award-text">Spotlight Paper (Top 2.2% of all submissions)</span>
                  </div>
                </div>
              </div>

              <!-- Ventrilo -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">Ventrilo: From Mobile Bowel Sound to Precision Gastrointestinal Diagnostic</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author">Yutong Xue</span>, 
                    <span class="pub-author">Liren Dong</span>, 
                    <span class="pub-author">Zhuxi Chen</span>, 
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Qianfei Ren</span>, 
                    <span class="pub-author">Yida Wang</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Zhenyi Jia</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM MobiCom</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>

                            <!-- Ventrilo -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">Polarix: Monitoring Multi-Component Liquids via Polarized Light</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author">Longyuan Ge</span>, 
                    <span class="pub-author">Yi-Chao Chen*</span>, 
                    <span class="pub-author">Qianfei Ren</span>, 
                    <span class="pub-author">Yijie Li*</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>,
                    <span class="pub-author">Yida Wang</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author">Lili Qiu</span>, 
                    <span class="pub-author">Jiadi Yu</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM MobiCom</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* co-corresponding author</span>
                  </div>
                </div>
              </div>

              <!-- HyQuant -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">HyQuant: Hybrid-Precision Quantization for LLM Attention</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Jiatong Ding</span>, 
                    <span class="pub-author">Bingxin Xing</span>, 
                    <span class="pub-author">Yu Zhang</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Xiaodong Yi</span>, 
                    <span class="pub-author">Xianbin Ouyang</span>, 
                    <span class="pub-author">FeiHuZhou</span>, 
                    <span class="pub-author">Kun Zhang</span>, 
                    <span class="pub-author">ZHENYU GUO</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author">Guangtao Xue</span>, 
                    <span class="pub-author">Yiming Zhang</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">EMNLP</span>
                    <span class="ccf-rank">CCF-B</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>

              <!-- BIND -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">BIND: Enabling Continuous Transaction Processing During Account Migration in Sharded Blockchains</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Jiahao Qi</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Jie Li</span>, 
                    <span class="pub-author">Jiannong Cao</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>,
                    <span class="pub-author">Shengyun Liu</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM WWW</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>

              <!-- LLM4Load -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">LLM4Load-Turbo: A Prompt-Driven LLM Framework with Knowledge Distillation for Efficient Multi-Scale Workload Prediction</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Zeyuan Ding</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Jiannong Cao</span>, 
                    <span class="pub-author">Yiming Zhang</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE TSC</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>

            </div>
          </div>

          <!-- 2025年 -->
          <div class="publications-year">
            <h3>2025</h3>
            <div class="publication-items">
            
              <!-- MODepth -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">MODepth: Benchmarking Mobile Multi-frame Monocular Depth Estimation with Optical Image Stabilization</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Hao Pan*</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Jiatong Ding</span>, 
                    <span class="pub-author">Yongjian Fu</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Ju Ren</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM SigGraph Asia</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* co-corresponding author</span>
                  </div>
                </div>
              </div>

              <!-- AuCom -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">AuCom: Extreme Compression for Real-Time Edge-to-Server Universal Audio Streaming</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Ran Wang</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Longyuan Ge</span>, 
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Jiannong Cao</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE TMC</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>
              
              <!-- LeakThief TMC -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">Sniffing the Application Usage Information With the Leakage Current of Laptops</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Xiaoyu Ji</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE TMC</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                </div>
              </div>
              
              <!-- Fundamental Research -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">A Survey on Acoustic Sensing in the Metasurface Era: Challenges, Advances, and Applications</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Liheng Jiang</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Ting Chen</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author highlight">Dian Ding</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Fenghua Xu</span>, 
                    <span class="pub-author">Liwei Guo</span>, 
                    <span class="pub-author">Jingwei Li</span>, 
                    <span class="pub-author">Xiong Li</span>, 
                    <span class="pub-author">Jiguo Yu</span>, 
                    <span class="pub-author">Xiaosong Zhang</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">Fundamental Research</span>
                  </div>
                </div>
              </div>
              
              <!-- AnchorAttention -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">AnchorAttention: Difference-aware Sparse Attention with Stripe Granularity</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yu Zhang</span>, 
                    <span class="pub-author">Dong Guo</span>, 
                    <span class="pub-author">Fang Wu</span>, 
                    <span class="pub-author">Guoliang Zhu</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Yiming Zhang*</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">EMNLP</span>
                    <span class="ccf-rank">CCF-B</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* co-corresponding author</span>
                  </div>
                </div>
              </div>
              
              <!-- MMID -->
              <div class="publication-item award">
                <div class="pub-content">
                  <h4 class="pub-title">High-resolution mmWave Imaging using Metasurface and Diffusion</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yida Wang</span>, 
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Yuxuan Zhou</span>, 
                    <span class="pub-author">Yifei Shen</span>, 
                    <span class="pub-author">Lili Qiu</span>, 
                    <span class="pub-author">Zeyuan Lai</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author highlight">Dian Ding</span>, 
                    <span class="pub-author">Mei Wang</span>, 
                    <span class="pub-author">Guangtao Xue</span>, 
                    <span class="pub-author">Qian Zhang</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM MobiSys</span>
                    <span class="ccf-rank">CCF-B</span>
                  </div>
                  <div class="pub-award-info">
                    <span class="award-icon">🏅</span>
                    <span class="award-text">Best Artifact Runner-up</span>
                  </div>
                </div>
              </div>
              
              <!-- TouchHBC -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">TouchHBC: Touch-based Human Body Communication via Leakage Current</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE TMC</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                </div>
              </div>
              
              <!-- M2Silent -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">M2Silent: Enabling Multi-user Silent Speech Interactions via Multi-directional Speakers in Shared Spaces</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Yida Wang</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Yi-Chao Chen*</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM CHI</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* co-corresponding author</span>
                  </div>
                </div>
              </div>
              
              <!-- Bridge -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">Bridge: Enabling BLE Direction Finding Feature Compatible with All Bluetooth Devices</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Runting Zhang</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Yi-Chao Chen*</span>, 
                    <span class="pub-author">Yida Wang</span>, 
                    <span class="pub-author">Dongyao Chen</span>, 
                    <span class="pub-author">Jingxian Wang</span>, 
                    <span class="pub-author">Jiadi Yu</span>, 
                    <span class="pub-author">Ling Ma</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM MobiCom</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* co-corresponding author</span>
                  </div>
                </div>
              </div>
              
            </div>
          </div>
          
          <!-- 2024年 -->
          <div class="publications-year">
            <h3>2024</h3>
            <div class="publication-items">
              
              <!-- M3Cam -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">M3Cam: Extreme Super-resolution via Multi-Modal Optical Flow for Mobile Cameras</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author">Yongjian Fu</span>, 
                    <span class="pub-author">Liyun Zhang</span>, 
                    <span class="pub-author">Feitong Tan</span>, 
                    <span class="pub-author">Ran Wang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>, 
                    <span class="pub-author">Ju Ren</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM SenSys</span>
                    <span class="ccf-rank">CCF-B</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># co-first author</span>
                  </div>
                </div>
              </div>
              
              <!-- HandPad -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">HandPad: Make Your Hand an On-the-go Writing Pad via Human Capacitance</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author">Yongjian Fu</span>, 
                    <span class="pub-author">Yongzhao Zhang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM UIST</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>
              
              <!-- VISAR -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">VISAR: Projecting Virtual Sound Spots for Acoustic Augmented Reality Using Air Nonlinearity</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Yida Wang</span>, 
                    <span class="pub-author highlight">Dian Ding</span>, 
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM IMWUT</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                </div>
              </div>         
              
              <!-- HCMG -->
              <div class="publication-item award">
                <div class="pub-content">
                  <h4 class="pub-title">HCMG: Human-Capacitance based Micro Gesture for VR/AR</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yu Lu</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Ran Wang</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM UbiComp MIMSVAI</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-award-info">
                    <span class="award-icon">🏅</span>
                    <span class="award-text">Best Paper Award</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* corresponding author</span>
                  </div>
                </div>
              </div>
              
              <!-- MuDiS -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">MuDiS: An Audio-independent, Wide-angle, and Leak-free Multi-directional Speaker</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Yijie Li</span>, 
                    <span class="pub-author">Juntao Zhou</span>, 
                    <span class="pub-author highlight">Dian Ding*</span>, 
                    <span class="pub-author">Yi-Chao Chen*</span>, 
                    <span class="pub-author">Lili Qiu</span>, 
                    <span class="pub-author">Jiadi Yu</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM MobiCom</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text">* co-corresponding author</span>
                  </div>
                </div>
              </div>
              
            </div>
          </div>
          
          <!-- 2023年及以前 -->
          <div class="publications-year">
            <h3>2023 and Before</h3>
            <div class="publication-items">
              
              <!-- LeakThief SECON -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">LeakThief: Stealing the Behavior Information of Laptop via Leakage Current</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Xiaoyu Ji</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE SECON</span>
                    <span class="venue-year">2023</span>
                    <span class="ccf-rank">CCF-B</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                </div>
              </div>
              
              <!-- Handwriting TMC -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">Handwriting Recognition System Leveraging Vibration Signal on Smartphones</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Lanqing Yang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE TMC</span>
                    <span class="venue-year">2022</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                </div>
              </div>
              
              <!-- LeakPrint -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">Leakage or Identification: Behavior-irrelevant User Identification Leveraging Leakage Current on Laptops</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Lanqing Yang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">ACM IMWUT</span>
                    <span class="venue-year">2021</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                </div>
              </div>
              
              <!-- VibWriter -->
              <div class="publication-item">
                <div class="pub-content">
                  <h4 class="pub-title">VibWriter: Handwriting Recognition System Based on Vibration Signal</h4>
                  <div class="pub-authors">
                    <span class="pub-author highlight">Dian Ding#</span>, 
                    <span class="pub-author">Lanqing Yang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE SECON</span>
                    <span class="venue-year">2021</span>
                    <span class="ccf-rank">CCF-B</span>
                  </div>
                  <div class="pub-correspondence">
                    <span class="corr-text"># first author</span>
                  </div>
                </div>
              </div>
              
              <!-- Magprint -->
              <div class="publication-item award">
                <div class="pub-content">
                  <h4 class="pub-title">Magprint: Deep Learning Based User Fingerprinting Using Electromagnetic Signals</h4>
                  <div class="pub-authors">
                    <span class="pub-author">Lanqing Yang</span>, 
                    <span class="pub-author">Yi-Chao Chen</span>, 
                    <span class="pub-author">Hao Pan</span>, 
                    <span class="pub-author highlight">Dian Ding</span>, 
                    <span class="pub-author">Guangtao Xue</span>
                  </div>
                  <div class="pub-venue">
                    <span class="venue-name">IEEE INFOCOM</span>
                    <span class="venue-year">2020</span>
                    <span class="ccf-rank">CCF-A</span>
                  </div>
                  <div class="pub-award-info">
                    <span class="award-icon">🏅</span>
                    <span class="award-text">World Artificial Intelligence Conference Youth Outstanding Paper Nomination Award (2021)</span>
                  </div>
                </div>
              </div>
              
            </div>
          </div>
          
        </div>
      </div>
      
    </div>
  </div>
</div>