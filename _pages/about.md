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

<span class='anchor' id='photo'></span>

# 📷 Photography

<style>
.photography-section {
  margin: 0.5rem 0;
}

.photo-carousel-container {
  position: relative;
  margin: 0.5rem 0;
}

.photo-carousel {
  display: flex;
  gap: 1.5rem;
  overflow-x: auto;
  scroll-behavior: smooth;
  padding: 1rem 0.5rem;
  scrollbar-width: thin;
  scrollbar-color: #ccc transparent;
}

.photo-carousel::-webkit-scrollbar {
  height: 6px;
}

.photo-carousel::-webkit-scrollbar-track {
  background: #f1f1f1;
  border-radius: 3px;
}

.photo-carousel::-webkit-scrollbar-thumb {
  background: #ccc;
  border-radius: 3px;
}

.photo-carousel::-webkit-scrollbar-thumb:hover {
  background: #999;
}

.photo-item {
  flex: 0 0 300px;
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

.carousel-nav {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-top: 1rem;
}

.nav-btn {
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 0.9rem;
}

.nav-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
}

.nav-btn:disabled {
  background: #ccc;
  cursor: not-allowed;
  transform: none;
  box-shadow: none;
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
  position: absolute;
  margin: auto;
  display: block;
  max-width: 90vw;
  max-height: 90vh;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  animation: zoomIn 0.3s ease;
  object-fit: contain;
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

.photo-counter {
  text-align: center;
  color: #666;
  font-size: 0.9rem;
  margin-top: 0.5rem;
}
.photo-intro {
  font-weight: 600;
  font-size: 1.1rem;
  color: #333;
  margin-bottom: 1.5rem;
  line-height: 1.5;
}
</style>

<p class="photo-intro">
  🫶 Embrace The Life 🫶
</p>
<div class="photography-section">
  <div class="">
    <div class="photo-carousel" id="photoCarousel">
      <!-- 照片1 -->
      <div class="photo-item" onclick="openModal('/images/DSC_0066.jpg')">
        <img src="/images/DSC_0066.jpg" alt="NJUPT's cat" class="photo-img">
        <div class="photo-info">
          <div class="photo-title">NJUPT's cat</div>
          <div class="photo-meta">
            <span class="photo-date">2025.10</span>
            <span class="photo-location">Nanjing</span>
          </div>
        </div>
      </div>

      <!-- 照片2 -->
      <div class="photo-item" onclick="openModal('/images/DSC_0025.jpg')">
        <img src="/images/DSC_0025.jpg" alt="Reflection" class="photo-img">
        <div class="photo-info">
          <div class="photo-title">Reflection</div>
          <div class="photo-meta">
            <span class="photo-date">2025.10</span>
            <span class="photo-location">Nanjing</span>
          </div>
        </div>
      </div>


      <!-- 可以继续添加更多照片 -->
    </div>

  </div>
</div>

<!-- 图片模态框 -->
<div id="imageModal" class="modal">
  <span class="close" onclick="closeModal()">&times;</span>
  <img class="modal-content" id="modalImage">
</div>

<script>
let currentScroll = 0;
const carousel = document.getElementById('photoCarousel');
const photoItems = document.querySelectorAll('.photo-item');
const itemWidth = 300 + 24; // 300px width + 24px gap
const visibleItems = 3;
const totalItems = photoItems.length;

function updateCounter() {
  const start = Math.floor(currentScroll / itemWidth) + 1;
  const end = Math.min(start + visibleItems - 1, totalItems);
  document.getElementById('photoCounter').textContent = `${start}-${end} of ${totalItems}`;
}

function scrollCarousel(direction) {
  const maxScroll = (totalItems - visibleItems) * itemWidth;
  
  currentScroll += direction * itemWidth * visibleItems;
  currentScroll = Math.max(0, Math.min(currentScroll, maxScroll));
  
  carousel.scrollTo({
    left: currentScroll,
    behavior: 'smooth'
  });
  
  updateCounter();
}

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

// 初始化计数器
updateCounter();

// 监听滚动事件（用户手动滚动时更新计数器）
carousel.addEventListener('scroll', function() {
  currentScroll = carousel.scrollLeft;
  updateCounter();
});
</script>




