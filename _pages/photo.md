
---
permalink: /photo/
title: "Photo Gallery"
excerpt: "My Photography Collection"
author_profile: true
---

<style>
.photo-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.photo-card {
  position: relative;
  border-radius: 15px;
  overflow: hidden;
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  background: white;
  cursor: pointer;
}

.photo-card:hover {
  transform: translateY(-10px) scale(1.02);
  box-shadow: 0 15px 35px rgba(0,0,0,0.15);
}

.photo-image {
  width: 100%;
  height: 250px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.photo-card:hover .photo-image {
  transform: scale(1.1);
}

.photo-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0,0,0,0.8));
  color: white;
  padding: 2rem 1rem 1rem;
  transform: translateY(100%);
  transition: transform 0.3s ease;
}

.photo-card:hover .photo-overlay {
  transform: translateY(0);
}

.photo-title {
  font-size: 1.2rem;
  font-weight: bold;
  margin-bottom: 0.5rem;
}

.photo-description {
  font-size: 0.9rem;
  opacity: 0;
  transition: opacity 0.3s ease 0.1s;
}

.photo-card:hover .photo-description {
  opacity: 1;
}

.back-btn {
  display: inline-block;
  padding: 0.8rem 2rem;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  text-decoration: none;
  border-radius: 25px;
  transition: all 0.3s ease;
  border: none;
  font-size: 1rem;
  margin-top: 2rem;
}

.back-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.gallery-header {
  text-align: center;
  margin-bottom: 3rem;
}

.gallery-header h1 {
  font-size: 2.5rem;
  background: linear-gradient(135deg, #667eea, #764ba2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 1rem;
}

.gallery-intro {
  font-size: 1.1rem;
  color: #666;
  max-width: 600px;
  margin: 0 auto;
}
</style>

<div class="gallery-header">
  <h1>📸 My Gallery</h1>
  <p class="gallery-intro">A collection of my favorite moments and creative works. Hover over images to see details.</p>
</div>

<div class="photo-gallery">
  <!-- Photo 1 -->
  <div class="photo-card">
    <img src="/assets/images/倒影.png" alt="Academic Life" class="photo-image">
    <div class="photo-overlay">
      <div class="photo-title">Campus Moments</div>
      <div class="photo-description">Life at Nanjing University of Posts and Telecommunications</div>
    </div>
  </div>

  <!-- Photo 2 -->
  <div class="photo-card">
    <img src="/assets/images/鸡鸣寺.png" alt="Competition" class="photo-image">
    <div class="photo-overlay">
      <div class="photo-title">Competition Journey</div>
      <div class="photo-description">Moments from various academic competitions and events</div>
    </div>
  </div>

  <!-- Photo 3 -->
  <div class="photo-card">
    <img src="/assets/images/鸡鸣寺树.png" alt="Projects" class="photo-image">
    <div class="photo-overlay">
      <div class="photo-title">Project Work</div>
      <div class="photo-description">Working on IoT engineering projects and research</div>
    </div>
  </div>

  <!-- Photo 4 -->
  <div class="photo-card">
    <img src="/assets/images/路牌.png" alt="Awards" class="photo-image">
    <div class="photo-overlay">
      <div class="photo-title">Achievement Celebration</div>
      <div class="photo-description">Celebrating academic awards and honors</div>
    </div>
  </div>

  <!-- Photo 5 -->
  <div class="photo-card">
    <img src="/assets/images/猫.png" alt="Conference" class="photo-image">
    <div class="photo-overlay">
      <div class="photo-title">Conference Experience</div>
      <div class="photo-description">Participating in academic conferences and seminars</div>
    </div>
  </div>

  <!-- Photo 6 -->
  <div class="photo-card">
    <img src="/assets/images/猫2.png" alt="Teamwork" class="photo-image">
    <div class="photo-overlay">
      <div class="photo-title">Team Collaboration</div>
      <div class="photo-description">Working with teammates on various projects</div>
    </div>
  </div>
</div>

<div style="text-align: center; margin-top: 3rem;">
  <a href="/" class="back-btn">← Back to Homepage</a>
</div>

<script>
// 添加加载动画效果
document.addEventListener('DOMContentLoaded', function() {
  const photoCards = document.querySelectorAll('.photo-card');
  
  photoCards.forEach((card, index) => {
    // 初始设置卡片透明
    card.style.opacity = '0';
    card.style.transform = 'translateY(30px)';
    
    // 延迟加载动画
    setTimeout(() => {
      card.style.transition = 'all 0.6s ease';
      card.style.opacity = '1';
      card.style.transform = 'translateY(0)';
    }, index * 200);
  });
});
</script>


<!-- 可以添加返回首页的链接 -->
<p style="margin-top: 2rem;">
  <a href="/">← Back to Home</a>
</p>
