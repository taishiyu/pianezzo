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
        <img src="/pianezzo/images/spring-bg.jpg" alt="Spring Atmosphere">
        <div class="bg-overlay"></div>
    </div>

    <div class="cards-track">
        
        <div class="content-card text-only">
            <span class="season-tag">Spring 01</span>
            <h3>The Sequence of Life</h3>
            <p>When spring quietly arrives at 1,100 meters, a delicate sequence of life begins to unfold. From the damp earth, resilient wild nettles are the first to emerge, closely followed by the tender shoots of wild berries.</p>
        </div>

        <div class="content-card split-layout">
            <div class="card-image"><img src="/pianezzo/images/spring-vibe-1.jpg" alt="Spring detail"></div>
            <div class="card-text">
                <span class="season-tag">Spring 02</span>
                <h3>The Return of Birds</h3>
                <p>The canopy fills with the industrious sounds of nest-building, with parent birds weaving dried grass and moss. Soon, the crisp sounds of hatching echo through the branches.</p>
            </div>
        </div>

        <div class="content-card split-layout">
            <div class="card-image"><img src="/pianezzo/images/spring-vibe-2.jpg" alt="Spring detail"></div>
            <div class="card-text">
                <span class="season-tag">Spring 03</span>
                <h3>The Nettle Harvest</h3>
                <p>Nettles provide our first fresh nutrients of the year. We gather them while the morning dew still clings to the leaves, preparing for the first alpine ferments.</p>
            </div>
        </div>

        <div class="content-card split-layout">
            <div class="card-image"><img src="/pianezzo/images/spring-vibe-3.jpg" alt="Spring detail"></div>
            <div class="card-text">
                <span class="season-tag">Spring 04</span>
                <h3>Emerging Blooms</h3>
                <p>By late spring, the alpine flora reaches its peak. Every corner of the land is a nursery for new life, gathering strength for the high summer sun.</p>
            </div>
        </div>

    </div>
</section>

<section id="summer" class="season-container">
    <div class="sticky-bg">
        <img src="/pianezzo/images/summer-bg.jpg" alt="Summer Atmosphere">
        <div class="bg-overlay"></div>
    </div>
    <div class="cards-track">
        <div class="content-card text-only">
            <span class="season-tag">Summer 01</span>
            <h3>Sunlight & Abundance</h3>
            <p>The mountain enters the fullness of summer. The massive canopy deepens into a rich, dense green, weaving a shaded sanctuary across the land.</p>
        </div>
    </div>
</section>

</div>

<style>
html { scroll-behavior: smooth; }

.seasons-wrapper {
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
    background-color: #f4f1ea;
}

.season-quick-nav {
    position: fixed; top: 30px; right: 4%; z-index: 1000;
    background: rgba(255, 255, 255, 0.9);
    backdrop-filter: blur(8px); padding: 10px 25px; border-radius: 50px;
    display: flex; gap: 20px; box-shadow: 0 4px 20px rgba(0,0,0,0.05);
}
.season-quick-nav a { font-family: 'Lora', serif; color: #3e2723; text-decoration: none; font-size: 0.9rem; font-weight: bold; }

.season-container { position: relative; width: 100%; }

.sticky-bg {
    position: sticky;
    top: 0;
    width: 100vw;
    height: 100vh;
    z-index: 1;
}
.sticky-bg img { width: 100%; height: 100%; object-fit: cover; }
.bg-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.15); }

.cards-track {
    position: relative;
    z-index: 2;
    margin-top: -100vh;
    padding-bottom: 50px;
}

/* 字卡樣式：全數向左對齊 */
.content-card {
    background: rgba(244, 241, 234, 0.98);
    margin: 150px 0 150px 8%; /* 關鍵：卡片本身靠左對齊，留 8% 左邊距 */
    padding: 80px;
    max-width: 900px;
    min-height: 500px;
    border-radius: 2px;
    box-shadow: 0 20px 50px rgba(0,0,0,0.1);
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: left; /* 文字向左對齊 */
}

/* 移除原本的置中樣式 */
.text-only { text-align: left; }
.winter-card { text-align: left; }

/* 分欄佈局：圖片在左，文字在右（本身就是左對齊趨向） */
.split-layout {
    flex-direction: row;
    gap: 60px;
    align-items: center;
}
.card-image { flex: 1.2; }
.card-image img { width: 100%; height: auto; border-radius: 2px; }
.card-text { flex: 1; }

/* 文字樣式 */
.season-tag { font-family: 'Lora', serif; font-size: 0.8rem; letter-spacing: 3px; color: #A67C52; margin-bottom: 20px; display: block; text-transform: uppercase; }
.content-card h3 { font-family: 'Lora', serif; font-size: 2.8rem; color: #1a1a1a; margin-bottom: 30px; line-height: 1.1; }
.content-card p { font-family: 'Lora', serif; font-size: 1.2rem; line-height: 1.9; color: #333; }

/* 手機版適配：回歸單欄且靠左 */
@media (max-width: 1024px) {
    .split-layout { flex-direction: column; align-items: flex-start; padding: 40px; }
    .content-card { 
        margin: 80px auto; /* 手機版還是建議稍微置中或維持小間距 */
        max-width: 92%; 
        padding: 40px;
    }
}
</style>
