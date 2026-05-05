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
<p>Where the dream took its first shape. Built stone by stone by Thomas Gorner in the late 1970s.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/main-house.jpg" alt="The Alpine Homestead"></div>
<div class="land-text">
<h3>The Alpine Homestead</h3>
<p>The evolving heart of our mountain life at 1,100 meters, overlooking the vastness of Val d'Ossola.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/workshop.jpg" alt="The Maker’s Atelier"></div>
<div class="land-text">
<h3>The Maker’s Atelier</h3>
<p>The space of precision and craft, where timber is transformed and energy is captured.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/lawn.jpg" alt="The Dancing Green"></div>
<div class="land-text">
<h3>The Dancing Green</h3>
<p>A vast, open meadow that has transitioned from a grazing pasture to a wild sanctuary.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/buddha.jpg" alt="The Sanctuary of Stillness"></div>
<div class="land-text">
<h3>The Sanctuary of Stillness</h3>
<p>A quiet corner for meditation, where the silence of the Alps meets Eastern wisdom.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/persimmon.jpg" alt="The Golden Orchard"></div>
<div class="land-text">
<h3>The Golden Orchard</h3>
<p>Bearing fruit against the high-altitude chill, these trees are a testament to resilience.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/flower-path.jpg" alt="The Pollinator’s Trail"></div>
<div class="land-text">
<h3>The Pollinator’s Trail</h3>
<p>A vibrant corridor of life, ensuring the buzz of bees and the flutter of wings across the land.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/chestnut.jpg" alt="The Ancient Bank"></div>
<div class="land-text">
<h3>The Ancient Bank</h3>
<p>The sloping forest of chestnuts, providing shade and sustenance for generations.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/pond.jpg" alt="The Sky Mirror"></div>
<div class="land-text">
<h3>The Sky Mirror</h3>
<p>A biodiverse haven reflecting the changing clouds and the peak of Pizzo Ton.</p>
</div>
</section>

<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/water-path.jpg" alt="The Alpine Current"></div>
<div class="land-text">
<h3>The Alpine Current</h3>
<p>Our source of life and power, channeling the 100% hydroelectric descent of water from 1,800 meters.</p>
</div>
</section>

</div>

<style>
/* 全域容器設定 */
.land-exploration { 
    width: 100%;
    margin: 0;
    padding: 0;
}

/* 每個區塊的基礎設定 */
.land-section { 
    display: flex; 
    align-items: flex-start; 
    gap: 80px; 
    padding: 100px 5%; /* 使用內距產生左右空白，並增加上下間距 */
    border-bottom: 1px solid rgba(93, 64, 55, 0.1); /* 淡淡的棕色橫線 */
    transition: background-color 0.3s ease;
}

/* 偶數區塊：改變背景色、反轉方向 */
.land-section:nth-child(even) { 
    background-color: #faf8f5; /* 極淡的奶油色 */
    flex-direction: row-reverse; 
}

/* 移除最後一個區塊的底線 */
.land-section:last-child { border-bottom: none; }

.land-image { flex: 1; }
.land-image img { 
    width: 100%; 
    height: auto; 
    border-radius: 2px; 
    box-shadow: 0 8px 25px rgba(0,0,0,0.1); 
}

.land-text { flex: 1; }
.land-text h3 { 
    font-family: 'Tangerine', cursive; 
    font-size: 4rem; 
    color: #5d4037; 
    margin-top: 0; 
    margin-bottom: 25px; 
}

.land-text p { 
    font-family: 'Lora', serif; 
    font-size: 1.25rem; 
    line-height: 1.9; 
    color: #444; 
}

/* 行動裝置適配 */
@media (max-width: 1024px) {
    .land-section { gap: 40px; padding: 60px 5%; }
}

@media (max-width: 768px) {
    .land-section, .land-section:nth-child(even) { 
        flex-direction: column; 
        padding: 40px 5%; 
        gap: 30px; 
    }
    .land-text { text-align: left; }
    .land-text h3 { font-size: 3.2rem; }
}
</style>
