---
title: "The Land"
featured_image: "/pianezzo/images/land.jpg"
description: "A walk through the ten realms of Alpe Pianezzo."
layout: "single"
---

<div class="land-exploration">

<!-- 1. 小木屋 -->
<section class="land-section">
<div class="land-image"><img src="/pianezzo/images/cabin.jpg" alt="The First Shelter"></div>
<div class="land-text">
<h3>The First Shelter</h3>
<p>Where the dream took its first shape. Built stone by stone by Thomas Gorner in the late 1970s, this cabin marks the beginning of a lifelong bond with the Antrona Valley.</p>
</div>
</section>

<!-- 這裡省略其餘 9 個 section 以節省空間，你在本機端維持原狀即可 -->

</div>

<style>
/* 1. 修改背景色：請在這段程式碼修改顏色 */
:root {
    --bg-color: #f4f1ea; 
}

body {
    background-color: var(--bg-color);
}

.land-exploration { 
    max-width: 85%; 
    margin: 0 auto; 
    padding: 0;
    background-color: var(--bg-color); 
}

.land-section { 
    display: flex; 
    align-items: flex-start; 
    gap: 70px; 
    padding: 100px 0; 
    border-bottom: 1px solid rgba(62, 39, 35, 0.1); 
}

.land-section:nth-child(even) { flex-direction: row-reverse; }
.land-section:last-child { border-bottom: none; }

/* 2. 修改大小比例：請在這兩段程式碼調整數值 */
.land-image { 
    flex: 3; /* 這是圖片的佔比 (數值越大圖片越寬) */
}

.land-text { 
    flex: 2; /* 這是文字的佔比 (目前圖片是文字的兩倍大) */
}

.land-image img { 
    width: 100%; 
    height: 600px;
    object-fit: cover; 
    border-radius: 2px; 
    box-shadow: 0 10px 30px rgba(0,0,0,0.08); 
}

.land-text h3 { 
    font-family: 'Tangerine', cursive; 
    font-size: 3.8rem; 
    color: #3e2723; 
    margin-top: -10px; 
    margin-bottom: 20px; 
    white-space: nowrap; 
}

.land-text p { 
    font-family: 'Lora', serif; 
    font-size: 1.2rem; 
    line-height: 1.7; 
    color: #444; 
}

@media (max-width: 1400px) { .land-exploration { max-width: 85%; } }
@media (max-width: 768px) {
    .land-exploration { max-width: 92%; }
    .land-section, .land-section:nth-child(even) { flex-direction: column; padding: 50px 0; gap: 30px; }
    .land-text h3 { white-space: normal; font-size: 3rem; }
}
</style>
