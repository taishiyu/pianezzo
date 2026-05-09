---
title: "The Seasons"
featured_image: "/pianezzo/images/season-cover.jpg"
description: "The breathing rhythm of Alpe Pianezzo: An ecological transition."
layout: "single"
---

<nav class="season-quick-nav">
<a href="#spring">Spring</a>
<a href="#summer">Summer</a>
<a href="#autumn">Autumn</a>
<a href="#winter">Winter</a>
</nav>

<div class="seasons-wrapper">

<section id="spring" class="season-container">
<div class="sticky-bg">
<img src="/pianezzo/images/spring-bg.jpg" alt="Spring Awakening">
<div class="bg-overlay"></div>
</div>
<div class="scroll-content">
<div class="content-card">
<span class="season-tag">Spring Awakening</span>
<h3>The Sequence of Life</h3>
<p>When spring quietly arrives at 1,100 meters, a delicate sequence of life begins to unfold. From the damp earth, resilient wild nettles are the first to emerge, closely followed by the tender shoots of wild berries, painting the slopes in a fresh, vibrant green.</p>
<br>
<p>As the alpine breeze warms, migratory birds return from afar. The canopy fills with the industrious sounds of nest-building, with parent birds weaving dried grass and moss. Soon, the crisp sounds of hatching echo through the branches, and the calls of newborn chicks harmonize with the blooming alpine flora, announcing the awakening of the entire forest.</p>
</div>
</div>
</section>

<section id="summer" class="season-container">
<div class="sticky-bg">
<img src="/pianezzo/images/summer-bg.jpg" alt="Summer Fullness">
<div class="bg-overlay"></div>
</div>
<div class="scroll-content">
<div class="content-card">
<span class="season-tag">Summer Fullness</span>
<h3>Sunlight & Abundance</h3>
<p>Under the brilliant sun, the mountain enters the fullness of summer, pulsing with vibrant energy. To capture the abundant light, the massive canopy deepens into a rich, dense green, weaving a shaded, cool sanctuary across the land.</p>
<br>
<p>Nourished by intense alpine sunshine and pure mountain currents, the fruit on the branches swells and ripens. A faint, honeyed sweetness fills the air as every piece of fruit silently gathers weight and abundance in the warm summer breeze.</p>
</div>
</div>
</section>

<section id="autumn" class="season-container">
<div class="sticky-bg">
<img src="/pianezzo/images/autumn-bg.jpg" alt="Autumn Resonance">
<div class="bg-overlay"></div>
</div>
<div class="scroll-content">
<div class="content-card">
<span class="season-tag">Autumn Resonance</span>
<h3>Colors & Echoes</h3>
<p>As the days shorten, the forest undergoes a magnificent transition, shifting from lush green to deep russets, bronzes, and golds. Beneath the thick carpet of fallen leaves, a quiet micro-world comes alive as clusters of wild mushrooms emerge with the autumn dampness.</p>
<br>
<p>Across the crisp, cooling air, the deep, resonant calls of mating animals break the silence. These powerful echoes pierce through the copper forest, becoming the most raw and vibrant resonance of the alpine autumn.</p>
</div>
</div>
</section>

<section id="winter" class="season-container">
<div class="sticky-bg">
<img src="/pianezzo/images/winter-bg.jpg" alt="Winter Silence">
<div class="bg-overlay"></div>
</div>
<div class="scroll-content">
<div class="content-card winter-card">
<span class="season-tag">Winter Silence</span>
<h3>The Great Rest</h3>
<p>Eventually, a great silence falls over the land.</p>
<br>
<p>Heavy snow descends, blanketing all colors and movement. The forest quiets, and both flora and fauna enter a deep, restful slumber. This is not an end, but a deep breath for Alpe Pianezzo—sleeping soundly beneath a white blanket of snow, quietly gathering strength for the next awakening.</p>
</div>
</div>
</section>

</div>

<style>
html { scroll-behavior: smooth; }

/* 破框全螢幕設定 */
.seasons-wrapper {
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
    background-color: #f4f1ea;
}

/* 懸浮導覽列 */
.season-quick-nav {
    position: fixed;
    top: 30px;
    right: 4%;
    z-index: 1000;
    background: rgba(255, 255, 255, 0.9);
    backdrop-filter: blur(8px);
    padding: 10px 25px;
    border-radius: 50px;
    display: flex;
    gap: 20px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.05);
}

.season-quick-nav a {
    font-family: 'Lora', serif;
    color: #3e2723;
    text-decoration: none;
    font-size: 0.9rem;
    font-weight: bold;
    letter-spacing: 1px;
}

/* 季節容器：行程增長確保翻動感 */
.season-container {
    position: relative;
    min-height: 250vh; 
}

/* 固定背景層 */
.sticky-bg {
    position: sticky;
    top: 0;
    width: 100vw;
    height: 100vh;
    z-index: 1;
    overflow: hidden;
}

.sticky-bg img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.bg-overlay {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: rgba(0,0,0,0.25);
}

/* 內容層：改為雙向置中佈局 */
.scroll-content {
    position: relative;
    z-index: 2;
    height: 100vh;
    margin-top: -100vh; /* 讓內容回到背景上方 */
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 5%;
    pointer-events: none; /* 讓滾動能穿透到下層 */
}

/* 加大後的字卡樣式 */
.content-card {
    pointer-events: auto; /* 恢復卡片內的互動 */
    background-color: rgba(244, 241, 234, 0.96); /* 帶點透明更有呼吸感 */
    padding: 80px;
    border-radius: 4px;
    box-shadow: 0 30px 100px rgba(0,0,0,0.3);
    max-width: 850px; /* 加大範圍 */
    width: 100%;
    border-top: 4px solid #A67C52;
    text-align: left;
    transition: transform 0.5s ease;
}

.winter-card {
    text-align: center;
    border-top: none;
}

.season-tag {
    display: block;
    font-family: 'Lora', serif;
    font-size: 0.9rem;
    text-transform: uppercase;
    letter-spacing: 3px;
    color: #A67C52;
    margin-bottom: 20px;
}

.content-card h3 {
    font-family: 'Lora', serif;
    font-size: 3rem;
    color: #1a1a1a;
    margin-bottom: 35px;
    line-height: 1.1;
}

.content-card p {
    font-family: 'Lora', serif;
    font-size: 1.25rem;
    line-height: 1.9;
    color: #333;
    text-align: justify;
}

/* 手機版適配 */
@media (max-width: 768px) {
    .content-card {
        padding: 40px 30px;
    }
    .content-card h3 { font-size: 2rem; }
    .content-card p { font-size: 1.1rem; }
    .season-quick-nav { top: 15px; right: 50%; transform: translateX(50%); width: max-content; padding: 8px 15px; }
}
</style>
