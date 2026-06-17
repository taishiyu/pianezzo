---
title: "Projects"
featured_image: "/pianezzo/images/cover2.jpg"
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
<label for="expand-1" class="expand-btn"></label>
</div>
</div>
</div>
</div>

<div class="timeline-item">
<div class="timeline-dot"></div>
<div class="project-card split-layout">
<div class="card-image"><img src="/pianezzo/images/project-birdhouse.jpg" alt="Nesting Boxes Stewardship"></div>
<div class="card-text">
<span class="project-time-tag">MAR - MAY ｜ WILDLIFE</span>
<h3>Nesting Boxes</h3>
<div class="expand-container">
<input type="checkbox" id="expand-2" class="expand-toggle" hidden>
<div class="expand-content">
<p>To support local biodiversity, hand-carved nesting boxes are securely placed throughout the larch and chestnut canopy.</p>
<p class="more">Carefully proportioned entry holes protect native tits and finches from larger alpine predators. We use locally sourced timber that naturally weathers to match the surrounding trees, minimizing our visual footprint while providing vital nesting sanctuaries for high-altitude avian residents.</p>
</div>
<label for="expand-2" class="expand-btn"></label>
</div>
</div>
</div>
</div>

</div>
</section>

<section id="section-architecture" class="project-section">
<div class="static-gallery-container">
<div class="project-card split-layout static-layout">
<div class="card-image"><img src="/pianezzo/images/project-arch.jpg" alt="Architecture"></div>
<div class="card-text">
<span class="project-time-tag">ARCHITECTURE ｜ STRUCTURE</span>
<h3>Stone & Timber Integration</h3>
<p>Ongoing restoration of traditional dry-stone walls and spatial staging of the mountain property.</p>
</div>
</div>
</div>
</section>

<section id="section-woodcraft" class="project-section">
<div class="static-gallery-container">
<div class="project-card split-layout static-layout">
<div class="card-image"><img src="/pianezzo/images/project-wood.jpg" alt="Woodcraft"></div>
<div class="card-text">
<span class="project-time-tag">WOODCRAFT ｜ ARTISANAL</span>
<h3>Organic Curves</h3>
<p>Synthesis of traditional carving techniques and precision CNC machinery on locally sourced larch.</p>
</div>
</div>
</div>
</section>

<section id="section-future" class="project-section">
<div class="static-gallery-container">
<div class="project-card split-layout static-layout future-layout">
<div class="card-image"><img src="/pianezzo/images/project-future.jpg" alt="Future"></div>
<div class="card-text">
<span class="project-time-tag">FUTURE ｜ BLUEPRINTS</span>
<h3>Closed-Loop Living</h3>
<p>Visions for small-scale water loops, soil regeneration, and artisanal sourdough infrastructures.</p>
</div>
</div>
</div>
</section>

</div>
</div>

<style>
html { scroll-behavior: smooth; }
.projects-master-container { width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; background: #f4f1ea; min-height: 100vh; padding-bottom: 150px; overflow-x: hidden; }
.projects-nav { position: sticky; top: 20px; z-index: 100; width: max-content; margin: 40px auto 80px auto; background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(8px); padding: 8px 15px; border-radius: 50px; display: flex; gap: 10px; box-shadow: 0 4px 25px rgba(0,0,0,0.06); border: 1px solid rgba(166, 124, 82, 0.15); }
.projects-nav label { font-family: 'Lora', serif; font-size: 0.9rem; font-weight: bold; color: #666; padding: 10px 22px; border-radius: 30px; cursor: pointer; transition: all 0.3s ease; text-transform: uppercase; letter-spacing: 1px; }
.project-section { display: none; animation: fadeIn 0.5s ease forwards; }
#tab-stewardship:checked ~ .projects-wrapper #section-stewardship,
#tab-architecture:checked ~ .projects-wrapper #section-architecture,
#tab-woodcraft:checked ~ .projects-wrapper #section-woodcraft,
#tab-future:checked ~ .projects-wrapper #section-future { display: block; }
#tab-stewardship:checked ~ .projects-nav label[for="tab-stewardship"],
#tab-architecture:checked ~ .projects-nav label[for="tab-architecture"],
#tab-woodcraft:checked ~ .projects-nav label[for="tab-woodcraft"],
#tab-future:checked ~ .projects-nav label[for="tab-future"] { background: #A67C52; color: #fff; }
@keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }
.timeline-container { position: relative; max-width: 1200px; margin: 0 auto; padding: 0 5%; }
.timeline-line { position: absolute; top: 0; bottom: 0; left: 12%; width: 2px; background: rgba(166, 124, 82, 0.2); }
.timeline-item { position: relative; margin-bottom: 120px; display: flex; align-items: center; }
.timeline-dot { position: absolute; left: 12%; transform: translateX(-50%); width: 12px; height: 12px; background: #A67C52; border-radius: 50%; border: 3px solid #f4f1ea; z-index: 2; }
.project-card { background: #fff; margin-left: 18%; width: 82%; padding: 60px; border-radius: 2px; box-shadow: 0 20px 50px rgba(0,0,0,0.05); border-top: 3px solid #A67C52; box-sizing: border-box; }
.split-layout { display: flex; gap: 50px; align-items: center; }
.card-image { flex: 1.4; }
.card-image img { width: 100%; max-height: 450px; object-fit: cover; border-radius: 2px; }
.card-text { flex: 1; text-align: left; }
.project-time-tag { font-family: 'Lora', serif; font-size: 0.8rem; letter-spacing: 2px; color: #A67C52; margin-bottom: 15px; display: block; }
.project-card h3 { font-family: 'Lora', serif; font-size: 2.2rem; margin-bottom: 25px; }
.project-card p { font-family: 'Lora', serif; font-size: 1.1rem; line-height: 1.8; color: #444; }
.static-gallery-container { max-width: 1200px; margin: 0 auto; padding: 0 5%; }
.static-layout { margin-left: 0; width: 100%; padding: 80px; }

/* 展開功能 CSS */
.expand-container { position: relative; }
.expand-content { max-height: 100px; overflow: hidden; transition: max-height 0.6s ease; position: relative; }
.expand-content::after { content: ""; position: absolute; bottom: 0; left: 0; width: 100%; height: 50px; background: linear-gradient(transparent, #fff); transition: opacity 0.3s; }
.expand-btn { display: inline-block; margin-top: 20px; color: #A67C52; font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; cursor: pointer; text-transform: uppercase; letter-spacing: 1px; }
.expand-btn::before { content: "Read Full Story"; }
.expand-toggle:checked + .expand-content { max-height: 1200px; }
.expand-toggle:checked + .expand-content::after { opacity: 0; }
.expand-toggle:checked ~ .expand-btn::before { content: "Show Less"; }

@media (max-width: 1024px) {
.project-card { margin-left: 15%; width: 85%; padding: 40px 30px; }
.timeline-line, .timeline-dot { left: 8%; }
.split-layout { flex-direction: column; gap: 25px; }
.card-image { width: 100%; }
}
</style>
