---
title: "The Land"
featured_image: "/pianezzo/images/land.jpg"
description: "A walk through the ten realms of Alpe Pianezzo."
layout: "single"
---

<div class="land-exploration">

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/cabin.jpg" alt="The First Shelter"></div>
<div class="land-text">
<h3>The First Shelter</h3>
<p>Where the dream took its first shape. Built stone by stone by Thomas Gorner in the late 1970s, this cabin marks the beginning of a lifelong bond with the Antrona Valley.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/main-house.jpg" alt="The Alpine Homestead"></div>
<div class="land-text">
<h3>The Alpine Homestead</h3>
<p>The evolving heart of our mountain life at 1,100 meters. A sanctuary that has witnessed decades of seasons, overlooking the vastness of Val d'Ossola.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/workshop.jpg" alt="The Maker’s Atelier"></div>
<div class="land-text">
<h3>The Maker’s Atelier</h3>
<p>The space of precision and craft. Here, mountain timber is transformed into functional art, and the 100% hydroelectric power is managed.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/lawn.jpg" alt="The Dancing Green"></div>
<div class="land-text">
<h3>The Dancing Green</h3>
<p>A vast, open meadow that transitioned from a short-cropped pasture for goats to a wild, flourishing sanctuary for mountain flora.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/buddha.jpg" alt="The Sanctuary of Stillness"></div>
<div class="land-text">
<h3>The Sanctuary of Stillness</h3>
<p>A quiet corner for meditation tucked within the peaks, where the silence of the Alps harmonizes with Eastern philosophical roots.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/persimmon.jpg" alt="The Golden Orchard"></div>
<div class="land-text">
<h3>The Golden Orchard</h3>
<p>Proof of resilience against the high-altitude chill. Every autumn, these trees offer a burst of honey-like sweetness to the cooling air.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/flower-path.jpg" alt="The Pollinator’s Trail"></div>
<div class="land-text">
<h3>The Pollinator’s Trail</h3>
<p>A vibrant corridor of life, carefully curated to ensure that bees, butterflies, and birds thrive within the garden’s ecosystem.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/chestnut.jpg" alt="The Ancient Bank"></div>
<div class="land-text">
<h3>The Ancient Bank</h3>
<p>The sloping forest of chestnuts, which once provided essential sustenance and now forms the foundation of our ecological oasis.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/pond.jpg" alt="The Sky Mirror"></div>
<div class="land-text">
<h3>The Sky Mirror</h3>
<p>A biodiverse haven reflecting the changing alpine clouds and the sharp silhouette of Pizzo Ton in its calm waters.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/water-path.jpg" alt="The Alpine Current"></div>
<div class="land-text">
<h3>The Alpine Current</h3>
<p>Our source of life and power. Descending from 1,800 meters, this pure water fuels our home and breathes life into the soil.</p>
</div>
</section>

</div>

<style>
/* 底色統一 */
:root { --bg-color: #f4f1ea; }
body { background-color: var(--bg-color); }

.land-exploration { 
    max-width: 80%; /* 佔滿 75% 版面 */
    margin: 0 auto; 
    padding: 0; 
}

.land-section { 
    display: flex; 
    align-items: flex-start; /* 讓內容靠頂部對齊 */
    gap: 60px; 
    padding: 120px 0; 
    border-bottom: 1px solid rgba(62, 39, 35, 0.1); 
}

.land-section:nth-child(even) { flex-direction: row-reverse; }
.land-section:last-child { border-bottom: none; }

/* 修正照片比例：移除固定高度，改用寬度控制 */
.land-image { 
    flex: 6; /* 圖片佔比 (你可以試試 1.5 或 2) */
}
.land-image img { 
    width: 100%; 
    height: 300px; /* 讓高度隨比例自動增長，不再細長 */
    display: block;
    border-radius: 2px; 
    box-shadow: 0 10px 30px rgba(0,0,0,0.08); 
}

/* 文字區域 */
.land-text { 
    flex: 1; 
}

.land-text h3 { 
    font-family: 'Tangerine', cursive; 
    font-size: 4.5rem; 
    color: #3e2723; 
    /* 關鍵：使用負邊距將文字往上拉到圖片的上緣 (黃線) */
    margin-top: -12px; 
    margin-bottom: 25px; 
    line-height: 1;
    white-space: nowrap; /* 保持單行 */
}

.land-text p { 
    font-family: 'Lora', serif; 
    font-size: 1.25rem; 
    line-height: 1.8; 
    color: #333; 
}

/* 行動裝置適配 */
@media (max-width: 1024px) {
    .land-text h3 { font-size: 3.5rem; margin-top: -20px; }
}

@media (max-width: 768px) {
    .land-exploration { max-width: 90%; }
    .land-section, .land-section:nth-child(even) { 
        flex-direction: column; 
        padding: 60px 0; 
        gap: 20px; 
    }
    .land-text h3 { margin-top: 0; white-space: normal; }
}
</style>
