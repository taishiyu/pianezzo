---
title: "Projects"
featured_image: "/pianezzo/images/projects-cover.jpg"
description: "人與山的深度介入與對話：Alpe Pianezzo 的專案與勞動紀實。"
layout: "single"
---

<div class="projects-master-container">

<input type="radio" id="tab-stewardship" name="project-tabs" checked hidden>
<input type="radio" id="tab-architecture" name="project-tabs" hidden>
<input type="radio" id="tab-woodcraft" name="project-tabs" hidden>
<input type="radio" id="tab-future" name="project-tabs" hidden>

<nav class="projects-nav">
<label for="tab-stewardship">Stewardship</label>
<label for="tab-architecture">Architecture</label>
<label for="tab-woodcraft">Woodcraft</label>
<label for="tab-future">Future</label>
</nav>

<div class="projects-wrapper">

<section id="section-stewardship" class="project-section">
<div class="timeline-container">
<div class="timeline-line"></div>

<div class="timeline-item">
<div class="timeline-dot"></div>
<div class="project-card split-layout">
<div class="card-image"><img src="/pianezzo/images/project-grafting.jpg" alt="Fruit Tree Grafting"></div>
<div class="card-text">
<span class="project-time-tag">MAR - APR ｜ ECOLOGY</span>
<h3>Fruit Tree Grafting</h3>
<p>As the sap begins to rise in early spring, we practice the ancient craft of grafting. By joining fresh scions to established rootstocks, we introduce resilient heritage fruit varieties while honoring the deep root systems that have anchored these slopes for decades.</p>
</div>
</div>
</div>

<div class="timeline-item">
<div class="timeline-dot"></div>
<div class="project-card split-layout">
<div class="card-image"><img src="/pianezzo/images/project-birdhouse.jpg" alt="Nesting Boxes Stewardship"></div>
<div class="card-text">
<span class="project-time-tag">MAR - MAY ｜ WILDLIFE</span>
<h3>Nesting Boxes Stewardship</h3>
<p>To support local biodiversity, hand-carved nesting boxes are securely placed throughout the larch and chestnut canopy. Carefully proportioned entry holes protect native tits and finches from larger alpine predators, transforming our quiet timber into active seasonal sanctuaries.</p>
</div>
</div>
</div>

<div class="timeline-item">
<div class="timeline-dot"></div>
<div class="project-card split-layout">
<div class="card-image"><img src="/pianezzo/images/project-forestry.jpg" alt="Autumn Forest Care"></div>
<div class="card-text">
<span class="project-time-tag">OCT - NOV ｜ FORESTRY</span>
<h3>Coppicing & Timber Reserve</h3>
<p>Seasonal thinning of the surrounding woodland ensures adequate light reaches the forest floor for spring flora. Selectively harvested wood is processed and naturally cured to fuel both the winter hearth and upcoming carving endeavors.</p>
</div>
</div>
</div>

</div>
</section>

<section id="section-architecture" class="project-section">
<div class="static-gallery-container">
<div class="project-card split-layout static-layout">
<div class="card-image"><img src="/pianezzo/images/project-arch.jpg" alt="Architecture Overview"></div>
<div class="card-text">
<span class="project-time-tag">ARCHITECTURE ｜ STRUCTURE</span>
<h3>Stone & Timber Integration</h3>
<p>Dedicated to the structural integrity and spatial staging of the mountain property. Future updates will showcase the careful restoration of traditional dry-stone walls and the ongoing symbiosis between internal layouts and external micro-climates.</p>
</div>
</div>
</div>
</section>

<section id="section-woodcraft" class="project-section">
<div class="static-gallery-container">
<div class="project-card split-layout static-layout">
<div class="card-image"><img src="/pianezzo/images/project-wood.jpg" alt="Woodcraft Exploration"></div>
<div class="card-text">
<span class="project-time-tag">WOODCRAFT ｜ ARTISANAL</span>
<h3>Organic Curves & Tooling</h3>
<p>Showcasing the synthesis of traditional carving knives and precision CNC machinery. Here, locally sourced larch wood is slowly transformed into tactile daily artifacts, ergonomically curved chair seats, and functional utility tools.</p>
</div>
</div>
</div>
</section>

<section id="section-future" class="project-section">
<div class="static-gallery-container">
<div class="project-card split-layout static-layout future-layout">
<div class="card-image"><img src="/pianezzo/images/project-future.jpg" alt="Future Blueprints"></div>
<div class="card-text">
<span class="project-time-tag">FUTURE VISIONS ｜ BLUEPRINTS</span>
<h3>Closed-Loop Alpine Living</h3>
<p>Experimental blueprints and philosophical reflections on self-sustaining ecology. Upcoming notes will explore small-scale spring-fed water loops, localized soil regeneration cycles, and advanced sourdough fermentation infrastructures.</p>
</div>
</div>
</div>
</section>

</div>

</div>

<style>
html { scroll-behavior: smooth; }

/* 破框滿版底色 */
.projects-master-container {
width: 100vw;
position: relative;
left: 50%; right: 50%;
margin-left: -50vw; margin-right: -50vw;
background: #f4f1ea;
min-height: 100vh;
padding-bottom: 150px;
box-sizing: border-box;
overflow-x: hidden;
}

/* 頂部導覽列樣式 */
.projects-nav {
position: sticky;
top: 20px;
z-index: 100;
width: max-content;
max-width: 90%;
margin: 40px auto 80px auto;
background: rgba(255, 255, 255, 0.9);
backdrop-filter: blur(8px);
padding: 8px 15px;
border-radius: 50px;
display: flex;
gap: 10px;
box-shadow: 0 4px 25px rgba(0,0,0,0.06);
border: 1px solid rgba(166, 124, 82, 0.15);
}

.projects-nav label {
font-family: 'Lora', serif;
font-size: 0.9rem;
font-weight: bold;
color: #666;
padding: 10px 22px;
border-radius: 30px;
cursor: pointer;
transition: all 0.3s ease;
text-transform: uppercase;
letter-spacing: 1px;
}

.projects-nav label:hover {
color: #A67C52;
}

/* 純 CSS 頁籤切換顯示邏輯 */
.project-section {
display: none;
animation: fadeIn 0.5s ease forwards;
}

#tab-stewardship:checked ~ .projects-wrapper #section-stewardship,
#tab-architecture:checked ~ .projects-wrapper #section-architecture,
#tab-woodcraft:checked ~ .projects-wrapper #section-woodcraft,
#tab-future:checked ~ .projects-wrapper #section-future {
display: block;
}

/* 導覽列按鈕高亮聯動 */
#tab-stewardship:checked ~ .projects-nav label[for="tab-stewardship"],
#tab-architecture:checked ~ .projects-nav label[for="tab-architecture"],
#tab-woodcraft:checked ~ .projects-nav label[for="tab-woodcraft"],
#tab-future:checked ~ .projects-nav label[for="tab-future"] {
background: #A67C52;
color: #ffffff;
box-shadow: 0 2px 10px rgba(166, 124, 82, 0.3);
}

@keyframes fadeIn {
from { opacity: 0; transform: translateY(15px); }
to { opacity: 1; transform: translateY(0); }
}

/* ================= 時間軸專屬排版 ================= */
.timeline-container {
position: relative;
max-width: 1200px;
margin: 0 auto;
padding: 0 5%;
}

/* 垂直時間線：靠左側放置 */
.timeline-line {
position: absolute;
top: 0; bottom: 0;
left: 12%;
width: 2px;
background: rgba(166, 124, 82, 0.25);
}

.timeline-item {
position: relative;
margin-bottom: 120px;
display: flex;
align-items: center;
}

/* 時間軸發光定位點 */
.timeline-dot {
position: absolute;
left: 12%;
transform: translateX(-50%);
width: 14px; height: 14px;
background: #A67C52;
border-radius: 50%;
border: 4px solid #f4f1ea;
box-shadow: 0 0 0 3px rgba(166, 124, 82, 0.2);
z-index: 2;
}

/* ================= 通用卡片美學 (延續 60/40) ================= */
.project-card {
background: #ffffff;
margin-left: 20%; /* 讓出左側時間軸空間 */
width: 80%;
padding: 60px;
border-radius: 2px;
box-shadow: 0 20px 60px rgba(0,0,0,0.08);
border-top: 3px solid #A67C52;
box-sizing: border-box;
}

.split-layout {
display: flex;
flex-direction: row;
gap: 50px;
align-items: center;
}

.card-image { flex: 1.4; } /* 60% 視覺佔比 */
.card-image img { width: 100%; max-height: 450px; object-fit: cover; border-radius: 2px; display: block; }
.card-text { flex: 1; text-align: left; } /* 40% 敘事佔比 */

.project-time-tag { font-family: 'Lora', serif; font-size: 0.8rem; letter-spacing: 2px; color: #A67C52; margin-bottom: 15px; display: block; font-weight: bold; }
.project-card h3 { font-family: 'Lora', serif; font-size: 2.2rem; color: #1a1a1a; margin-bottom: 20px; line-height: 1.2; }
.project-card p { font-family: 'Lora', serif; font-size: 1.1rem; line-height: 1.9; color: #444; margin: 0; text-align: justify; }

/* 靜態板塊展示容器 */
.static-gallery-container {
max-width: 1200px;
margin: 40px auto 0 auto;
padding: 0 5%;
}

.static-layout {
margin-left: 0; /* 靜態頁面不需讓位給時間軸，全幅置中 */
width: 100%;
padding: 80px;
}

.future-layout {
border-top-style: dashed; /* 未來規劃用虛線展現實驗感 */
background: rgba(255, 255, 255, 0.6);
}

/* 行動裝置極致適配 */
@media (max-width: 1024px) {
.projects-nav { max-width: 95%; padding: 6px 10px; gap: 4px; margin-bottom: 50px; flex-wrap: wrap; justify-content: center; }
.projects-nav label { padding: 8px 15px; font-size: 0.8rem; }
.timeline-line { left: 8%; }
.timeline-dot { left: 8%; width: 12px; height: 12px; }
.project-card { margin-left: 16%; width: 84%; padding: 35px 25px; }
.static-layout { width: 100%; margin-left: 0; }
.split-layout { flex-direction: column; gap: 25px; align-items: flex-start; }
.card-image { width: 100%; }
.card-image img { max-height: 250px; }
.project-card h3 { font-size: 1.8rem; }
.project-card p { font-size: 1.05rem; }
.timeline-item { margin-bottom: 70px; }
}
</style>
