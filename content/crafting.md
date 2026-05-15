---
title: "Crafting"
featured_image: "/pianezzo/images/crafting.jpg"
description: "雙手、材質與時間的落地實踐。"
layout: "single"
---

<div class="crafting-master-container">

<input type="radio" id="craft-tab-artifacts" name="craft-tabs" checked hidden>
<input type="radio" id="craft-tab-experiences" name="craft-tabs" hidden>

<nav class="crafting-nav">
<label for="craft-tab-artifacts">Selected Pieces</label>
<label for="craft-tab-experiences">Workshops</label>
</nav>

<div class="crafting-wrapper">

<section id="section-artifacts" class="craft-section">
<div class="artifacts-grid">

<div class="artifact-card">
<div class="artifact-image-wrapper">
<img src="/pianezzo/images/craft-chair.jpg" alt="Solid Wood Chair">
</div>
<div class="artifact-content">
<span class="artifact-tag">LARCH WOOD</span>
<h3>Solid Wood Chair</h3>
<p>Synthesis of T-spline digital modeling and artisanal hand-carving. Shaped from locally sourced alpine larch, preserving organic honesty.</p>
<div class="artifact-footer">
<span class="artifact-status">Bespoke</span>
<a href="/pianezzo/contact/" class="artifact-link">Inquire</a>
</div>
</div>
</div>

<div class="artifact-card">
<div class="artifact-image-wrapper">
<img src="/pianezzo/images/craft-utensils.jpg" alt="Kitchen Utensils">
</div>
<div class="artifact-content">
<span class="artifact-tag">BATCH 01</span>
<h3>Kitchen Utensils</h3>
<p>Each piece is individually carved from timber salvaged during seasonal orchard pruning. Finished with organic food-safe oil.</p>
<div class="artifact-footer">
<span class="artifact-status">3 Pieces Left</span>
<a href="/pianezzo/contact/" class="artifact-link">Inquire</a>
</div>
</div>
</div>

</div>
</section>

<section id="section-experiences" class="craft-section">
<div class="gallery-container">

<div class="project-card split-layout">
<div class="card-image"><img src="/pianezzo/images/walk-ecology.jpg" alt="Alpine Stewardship Walks"></div>
<div class="card-text">
<span class="project-time-tag">PERMANENT ｜ ECOLOGY</span>
<h3>Alpine Walks & Stewardship</h3>
<p>A deep immersion into the landscape of Alpe Pianezzo. Walks are centered around historical stone integration, orchard management, and local wildlife observation.</p>
<div class="acquisition-box">
<span class="status-tag available">Year-round ｜ By Appointment</span>
<a href="/pianezzo/contact/" class="inquire-btn">Book an Experience</a>
</div>
</div>
</div>

<div class="project-card split-layout">
<div class="card-image"><img src="/pianezzo/images/workshop-baking.jpg" alt="Seasonal Workshops"></div>
<div class="card-text">
<span class="project-time-tag">SEASONAL ｜ GATHERINGS</span>
<h3>The Seasonal Cycle Workshops</h3>
<div class="expand-container">
<input type="checkbox" id="workshop-expand" class="expand-toggle" hidden>
<div class="expand-content">
<p>Our gatherings honor the rhythm of the mountain. We host limited, small-scale immersive experiences tailored to each season's unique offering.</p>
<p class="more"><strong>🌸 Spring & Summer</strong>: Wild Yeast Baking & Meadow Picnics.<br><strong>🍂 Autumn</strong>: Foraging Walks for Chestnuts & Heritage Apples.<br><strong>❄️ Winter</strong>: Fireplace Woodcraft & Traditional Utensil Carving.</p>
</div>
<label for="workshop-expand" class="expand-btn"></label>
</div>
</div>
</div>

</div>
</section>

</div>
</div>

<style>
html { scroll-behavior: smooth; }
.crafting-master-container { width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; background: #f4f1ea; min-height: 100vh; padding-bottom: 150px; overflow-x: hidden; }
.crafting-nav { position: sticky; top: 20px; z-index: 100; width: max-content; margin: 40px auto 80px auto; background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(8px); padding: 6px 12px; border-radius: 50px; display: flex; gap: 5px; box-shadow: 0 4px 25px rgba(0,0,0,0.06); border: 1px solid rgba(166, 124, 82, 0.15); }
.crafting-nav label { font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; color: #777; padding: 10px 24px; border-radius: 30px; cursor: pointer; transition: all 0.3s ease; text-transform: uppercase; letter-spacing: 0.5px; }
.craft-section { display: none; animation: craftFadeIn 0.5s ease forwards; }
#craft-tab-artifacts:checked ~ .crafting-wrapper #section-artifacts, #craft-tab-experiences:checked ~ .crafting-wrapper #section-experiences { display: block; }
#craft-tab-artifacts:checked ~ .crafting-nav label[for="craft-tab-artifacts"], #craft-tab-experiences:checked ~ .crafting-nav label[for="craft-tab-experiences"] { background: #A67C52; color: #fff; }
@keyframes craftFadeIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: translateY(0); } }
.artifacts-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 35px; max-width: 1200px; margin: 0 auto; padding: 0 5%; }
.artifact-card { background: #fff; border-top: 3px solid #A67C52; box-shadow: 0 15px 40px rgba(0,0,0,0.03); display: flex; flex-direction: column; height: 100%; }
.artifact-image-wrapper { width: 100%; aspect-ratio: 3 / 4; overflow: hidden; background: #eae6df; }
.artifact-image-wrapper img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.6s cubic-bezier(0.25, 1, 0.5, 1); }
.artifact-card:hover .artifact-image-wrapper img { transform: scale(1.03); }
.artifact-content { padding: 25px; text-align: left; display: flex; flex-direction: column; flex-grow: 1; }
.artifact-tag { font-family: 'Lora', serif; font-size: 0.75rem; letter-spacing: 2px; color: #A67C52; margin-bottom: 8px; display: block; }
.artifact-card h3 { font-family: 'Lora', serif; font-size: 1.35rem; margin: 0 0 12px 0; color: #1a1a1a; text-align: left; }
.artifact-content p { font-family: 'Lora', serif; font-size: 0.95rem; line-height: 1.6; color: #555; margin: 0 0 20px 0; text-align: left; display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical; overflow: hidden; }
.artifact-footer { margin-top: auto; padding-top: 15px; border-top: 1px solid #f5f2eb; display: flex; justify-content: space-between; align-items: center; }
.artifact-status { font-family: 'Lora', serif; font-size: 0.8rem; font-style: italic; color: #777; }
.artifact-link { font-family: 'Lora', serif; font-size: 0.75rem; font-weight: bold; color: #A67C52; text-decoration: none; border: 1px solid #A67C52; padding: 6px 14px; border-radius: 2px; transition: all 0.3s; text-transform: uppercase; letter-spacing: 0.5px; }
.artifact-link:hover { background: #A67C52; color: #fff; }
.gallery-container { max-width: 1200px; margin: 0 auto; padding: 0 5%; }
.project-card { background: #fff; width: 100%; padding: 60px; border-radius: 2px; box-shadow: 0 20px 50px rgba(0,0,0,0.04); border-top: 3px solid #A67C52; box-sizing: border-box; margin-bottom: 60px; }
.split-layout { display: flex; gap: 50px; align-items: center; }
.card-image { flex: 1.3; }
.card-image img { width: 100%; max-height: 420px; object-fit: cover; border-radius: 2px; }
.card-text { flex: 1; text-align: left; }
.project-time-tag { font-family: 'Lora', serif; font-size: 0.8rem; letter-spacing: 2px; color: #A67C52; margin-bottom: 15px; display: block; }
.project-card h3 { font-family: 'Lora', serif; font-size: 2.2rem; margin-bottom: 25px; color: #1a1a1a; text-align: left; }
.project-card p { font-family: 'Lora', serif; font-size: 1.05rem; line-height: 1.8; color: #444; text-align: left; }
.acquisition-box { margin-top: 30px; padding-top: 20px; border-top: 1px solid #f0ede6; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 15px; }
.status-tag { font-family: 'Lora', serif; font-size: 0.85rem; font-style: italic; color: #666; }
.inquire-btn { font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; color: #A67C52; text-decoration: none; border: 1px solid #A67C52; padding: 10px 20px; border-radius: 2px; transition: all 0.3s; text-transform: uppercase; letter-spacing: 1px; }
.inquire-btn:hover { background: #A67C52; color: #fff; }
.expand-container { position: relative; text-align: left; }
.expand-content { max-height: 80px; overflow: hidden; transition: max-height 0.5s ease; position: relative; text-align: left; }
.expand-content::after { content: ""; position: absolute; bottom: 0; left: 0; width: 100%; height: 40px; background: linear-gradient(transparent, #fff); transition: opacity 0.3s; }
.expand-btn { display: inline-block; margin-top: 20px; color: #A67C52; font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; cursor: pointer; text-transform: uppercase; letter-spacing: 1px; }
.expand-btn::before { content: "Read Full Details"; }
.expand-toggle:checked + .expand-content { max-height: 800px; }
.expand-toggle:checked + .expand-content::after { opacity: 0; }
.expand-toggle:checked ~ .expand-btn::before { content: "Show Less"; }
@media (max-width: 1024px) { .artifacts-grid { grid-template-columns: repeat(2, 1fr); gap: 20px; } .project-card { padding: 40px 25px; } .split-layout { flex-direction: column; gap: 25px; } .card-image { width: 100%; } .acquisition-box { flex-direction: column; align-items: flex-start; } }
@media (max-width: 768px) { .artifacts-grid { grid-template-columns: 1fr; gap: 25px; } }
</style>