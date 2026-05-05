---
title: "The Land"
featured_image: "images/land.jpg"
description: "A walk through the ten realms of Alpe Pianezzo."
layout: "single"
---

<div class="land-exploration">

<!-- 1. 小木屋 -->
<section class="land-section">
<div class="land-image"><img src="/images/cabin.jpg" alt="The First Shelter"></div>
<div class="land-text">
<h3>The First Shelter</h3>
<p>Where the dream took its first shape. Built stone by stone by Thomas Gorner in the late 1970s.</p>
</div>
</section>

<!-- 2. 大屋 -->
<section class="land-section reverse">
<div class="land-image"><img src="/images/main-house.jpg" alt="The Alpine Homestead"></div>
<div class="land-text">
<h3>The Alpine Homestead</h3>
<p>The evolving heart of our mountain life at 1,100 meters, overlooking the vastness of Val d'Ossola.</p>
</div>
</section>

<!-- 3. 工具坊 -->
<section class="land-section">
<div class="land-image"><img src="/images/workshop.jpg" alt="The Maker’s Atelier"></div>
<div class="land-text">
<h3>The Maker’s Atelier</h3>
<p>The space of precision and craft, where timber is transformed and energy is captured.</p>
</div>
</section>

<!-- 4. 大草坪 -->
<section class="land-section reverse">
<div class="land-image"><img src="/images/lawn.jpg" alt="The Dancing Green"></div>
<div class="land-text">
<h3>The Dancing Green</h3>
<p>A vast, open meadow that has transitioned from a grazing pasture to a wild sanctuary.</p>
</div>
</section>

<!-- 5. 佛園 -->
<section class="land-section">
<div class="land-image"><img src="/images/buddha.jpg" alt="The Sanctuary of Stillness"></div>
<div class="land-text">
<h3>The Sanctuary of Stillness</h3>
<p>A quiet corner for meditation, where the silence of the Alps meets Eastern wisdom.</p>
</div>
</section>

<!-- 6. 柿園 -->
<section class="land-section reverse">
<div class="land-image"><img src="/images/persimmon.jpg" alt="The Golden Orchard"></div>
<div class="land-text">
<h3>The Golden Orchard</h3>
<p>Bearing fruit against the high-altitude chill, these trees are a testament to resilience.</p>
</div>
</section>

<!-- 7. 花徑 -->
<section class="land-section">
<div class="land-image"><img src="/images/flower-path.jpg" alt="The Pollinator’s Trail"></div>
<div class="land-text">
<h3>The Pollinator’s Trail</h3>
<p>A vibrant corridor of life, ensuring the buzz of bees and the flutter of wings across the land.</p>
</div>
</section>

<!-- 8. 栗坡 -->
<section class="land-section reverse">
<div class="land-image"><img src="/images/chestnut.jpg" alt="The Ancient Bank"></div>
<div class="land-text">
<h3>The Ancient Bank</h3>
<p>The sloping forest of chestnuts, providing shade and sustenance for generations.</p>
</div>
</section>

<!-- 9. 池塘 -->
<section class="land-section">
<div class="land-image"><img src="/images/pond.jpg" alt="The Sky Mirror"></div>
<div class="land-text">
<h3>The Sky Mirror</h3>
<p>A biodiverse haven reflecting the changing clouds and the peak of Pizzo Ton.</p>
</div>
</section>

<!-- 10. 水徑 -->
<section class="land-section reverse">
<div class="land-image"><img src="/images/water-path.jpg" alt="The Alpine Current"></div>
<div class="land-text">
<h3>The Alpine Current</h3>
<p>Our source of life and power, channeling the 100% hydroelectric descent of water from 1,800 meters.</p>
</div>
</section>

</div>

<style>
.land-exploration { 
    max-width: 90%; /* 縮小兩旁空白，讓內容寬度增加 */
    margin: 0 auto; 
    padding: 40px 0; 
}

.land-section { 
    display: flex; 
    align-items: flex-start; /* 圖片與文字頂部對齊 */
    gap: 40px; 
    margin-bottom: 80px; 
}

.land-section.reverse { flex-direction: row-reverse; }

.land-image { 
    flex: 1; /* 圖片佔 1 份比例 */
}

.land-image img { 
    width: 100%; 
    height: auto; 
    border-radius: 4px; 
    box-shadow: 0 5px 15px rgba(0,0,0,0.1); 
}

.land-text { 
    flex: 2; /* 文字佔 2 份比例 */
}

.land-text h3 { 
    font-family: 'Tangerine', cursive; 
    font-size: 3.5rem; 
    color: #5d4037; 
    margin-top: 0; /* 確保標題頂部與圖片切齊 */
    margin-bottom: 15px; 
}

.land-text p { 
    font-family: 'Lora', serif; 
    font-size: 1.1rem; 
    line-height: 1.7; 
    color: #333; 
}

@media (max-width: 768px) {
    .land-exploration { max-width: 95%; }
    .land-section, .land-section.reverse { flex-direction: column; gap: 20px; }
    .land-text { text-align: left; }
}
</style>
