---
title: "Projects"
featured_image: "/pianezzo/images/projects-cover.jpg"
description: "人與山的深度介入與對話。"
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

<div class="expand-container">
<input type="checkbox" id="expand-1" class="expand-toggle" hidden>
<div class="expand-content">
<p>As the sap begins to rise in early spring, we practice the ancient craft of grafting. By joining fresh scions to established rootstocks, we introduce resilient heritage fruit varieties.</p>
<p class="more">Beyond the technical skill, grafting at Alpe Pianezzo is a form of temporal bridge-building. We are currently experimenting with high-altitude varieties that can withstand late frosts, ensuring the food forest remains productive even as mountain climates shift. Each successful bond is a testament to the resilience of these slopes.</p>
</div>
<label for="expand-1" class="expand-btn">Read More</label>
</div>

</div>
</div>
</div>

</div>
</section>

</div>
</div>

<style>
/* 核心展開邏輯 */
.expand-container { position: relative; }

.expand-content {
max-height: 100px; /* 初始預覽高度 */
overflow: hidden;
position: relative;
transition: max-height 0.5s ease;
}

/* 漸層遮罩：只有在未展開時顯示 */
.expand-content::after {
content: "";
position: absolute;
bottom: 0; left: 0;
width: 100%; height: 50px;
background: linear-gradient(transparent, #ffffff);
transition: opacity 0.3s;
}

.expand-btn {
display: inline-block;
margin-top: 15px;
color: #A67C52;
font-family: 'Lora', serif;
font-size: 0.85rem;
font-weight: bold;
cursor: pointer;
text-transform: uppercase;
letter-spacing: 1px;
}

.expand-btn::before { content: "View Full Story"; }

/* 展開後的狀態 */
.expand-toggle:checked + .expand-content {
max-height: 1000px; /* 展開後的足夠高度 */
}

.expand-toggle:checked + .expand-content::after {
opacity: 0; /* 隱藏漸層 */
}

.expand-toggle:checked ~ .expand-btn::before {
content: "Show Less"; /* 切換按鈕文字 */
}

/* 保持原本的 60/40 與時間軸 CSS ... (略，請保留之前設定好的樣式) */
.projects-master-container { width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; background: #f4f1ea; padding-bottom: 100px; }
.projects-nav { position: sticky; top: 20px; z-index: 100; display: flex; justify-content: center; gap: 10px; margin-bottom: 50px; }
.project-card { background: #fff; margin-left: 15%; width: 80%; padding: 50px; border-radius: 2px; box-shadow: 0 10px 30px rgba(0,0,0,0.05); }
.split-layout { display: flex; gap: 40px; }
.card-image { flex: 1.4; }
.card-text { flex: 1; text-align: left; }
</style>
