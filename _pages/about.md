---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='education'></span>

# 🎓 Education
- *Sep 2022 - Jun 2026*, <a href="https://www.njupt.edu.cn/"></a> B.Eng. in Internet of Things Engineering, Nanjing University of Posts and Telecommunications, Nanjing, Jiangsu

<span class='anchor' id='academic-awards'></span>

# 🏆 Academic Awards
- *Sep 2024* First-Class Scholarship And Merit Student, Nanjing University of Posts and Telecommunications
- *Feb 2023* Third Prize, "College Student Mental Health Education Short Video Competition", Nanjing University of Posts and Telecommunications
- *Sep 2023* Single Subject Academic Excellence Award, Nanjing University of Posts and Telecommunications

<span class='anchor' id='honors-awards'></span>

# 🏅 Honors And Competitions
- *Mar 2025* Second Prize (Preliminary Round), National College Mathematics Competition
- *Aug 2024* Third Prize (National Finals), "China Software Cup" College Student Software Design Competition
- *Aug 2024* Second Prize (Jiangsu Division), "Beidou Cup" National Youth Aerospace Technology Experience and Innovation Competition
- *Jul 2024* Second Prize (East China Division II), Engineering Practice, "Siemens Cup" China Intelligent Challenge
- *Apr 2024* Honorable Mention, Mathematical Contest in Modeling (MCM)

<span class='anchor' id='academic-conferences'></span>

# 🏛️ Academic Conferences
- *May 2025*, International Conference on Intelligent Computing (ICIC 2025), Ningbo, Zhejiang

<span class='anchor' id='photography'></span>

# 📷 Photography

<style>
.photography-section {
  margin: 3rem 0;
}

.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.photo-item {
  position: relative;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
  background: white;
  cursor: pointer;
}

.photo-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.15);
}

.photo-img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.photo-item:hover .photo-img {
  transform: scale(1.05);
}

.photo-info {
  padding: 1rem;
  background: white;
}

.photo-title {
  font-weight: 600;
  color: #333;
  margin-bottom: 0.5rem;
  font-size: 1.1rem;
}

.photo-desc {
  color: #666;
  font-size: 0.9rem;
  line-height: 1.4;
}

.photo-meta {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 0.8rem;
  padding-top: 0.8rem;
  border-top: 1px solid #f0f0f0;
}

.photo-date {
  color: #888;
  font-size: 0.8rem;
}

.photo-location {
  color: #666;
  font-size: 0.8rem;
}

.view-more {
  text-align: center;
  margin-top: 2rem;
}

.view-more-btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.8rem 1.5rem;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  text-decoration: none;
  border-radius: 25px;
  transition: all 0.3s ease;
  font-weight: 500;
}

.view-more-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
}

/* 模态框样式 */
.modal {
  display: none;
  position: fixed;
  z-index: 1000;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.9);
  animation: fadeIn 0.3s ease;
}

.modal-content {
  position: relative;
  margin: auto;
  display: block;
  width: 90%;
  max-width: 700px;
  max-height: 80vh;
  top: 50%;
  transform: translateY(-50%);
  border-radius: 10px;
  animation: zoomIn 0.3s ease;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes zoomIn {
  from { transform: translateY(-50%) scale(0.8); }
  to { transform: translateY(-50%) scale(1); }
}

.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #fff;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
  z-index: 1001;
}

.close:hover {
  color: #ccc;
}
</style>

<div class="photography-section">
  <p>Capturing moments and perspectives through my lens. Here are some of my favorite shots that showcase my passion for photography.</p>
  
  <div class="photo-grid">
    <!-- 照片1 -->
    <div class="photo-item" onclick="openModal('assets/images/DSC_0066.jpg')">
      <img src="assets/images/photo1.jpg" alt="Urban Landscape" class="photo-img">
      <div class="photo-info">
        <div class="photo-title">Urban Symphony</div>
        <div class="photo-desc">Cityscape captured during golden hour, showcasing urban architecture and lighting.</div>
        <div class="photo-meta">
          <span class="photo-date">2024.03</span>
          <span class="photo-location">Nanjing</span>
        </div>
      </div>
    </div>

    <!-- 照片2 -->
    <div class="photo-item" onclick="openModal('assets/images/DSC_0025.jpg')">
      <img src="assets/images/photo2.jpg" alt="Nature Scene" class="photo-img">
      <div class="photo-info">
        <div class="photo-title">Nature's Palette</div>
        <div class="photo-desc">Vibrant colors of nature captured in a peaceful garden setting.</div>
        <div class="photo-meta">
          <span class="photo-date">2024.05</span>
          <span class="photo-location">Suzhou</span>
        </div>
      </div>
    </div>

  <div class="view-more">
    <a href="/photo/" class="view-more-btn">
      View Full Gallery 
      <span style="font-size: 1.2em;">→</span>
    </a>
  </div>
</div>

<!-- 图片模态框 -->
<div id="imageModal" class="modal">
  <span class="close" onclick="closeModal()">&times;</span>
  <img class="modal-content" id="modalImage">
</div>

<script>
// 打开模态框
function openModal(src) {
  const modal = document.getElementById('imageModal');
  const modalImg = document.getElementById('modalImage');
  modal.style.display = 'block';
  modalImg.src = src;
}

// 关闭模态框
function closeModal() {
  document.getElementById('imageModal').style.display = 'none';
}

// 点击模态框背景关闭
document.getElementById('imageModal').addEventListener('click', function(e) {
  if (e.target === this) {
    closeModal();
  }
});

// ESC键关闭
document.addEventListener('keydown', function(e) {
  if (e.key === 'Escape') {
    closeModal();
  }
});

// 添加滚动动画
document.addEventListener('DOMContentLoaded', function() {
  const photoItems = document.querySelectorAll('.photo-item');
  
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.style.opacity = '1';
        entry.target.style.transform = 'translateY(0)';
      }
    });
  }, { threshold: 0.1 });
  
  photoItems.forEach(item => {
    item.style.opacity = '0';
    item.style.transform = 'translateY(30px)';
    item.style.transition = 'all 0.6s ease';
    observer.observe(item);
  });
});
</script>
