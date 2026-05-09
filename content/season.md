---
title: "The Seasons"
featured_image: "/pianezzo/images/season-cover.jpg"
description: "時間的呼吸：Alpe Pianezzo 的四季生態演替。"
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
        <div class="scroll-content layout-left">
            <div class="content-card">
                <span class="season-tag">Spring Awakening</span>
                <h3>萬物甦醒</h3>
                <p>當春意微透，生命的次序在海拔 1,100 公尺處悄然展開。濕潤的地表上，堅韌的蕁麻率先破土而出，隨後野莓的嫩芽也紛紛綻放，為整片山坡染上初生的翠綠。</p>
                <br>
                <p>隨著微風漸暖，遠道而來的候鳥陸續抵達。林間開始響起築巢的忙碌拍打聲，親鳥銜著乾草與苔蘚穿梭其中。不久後，清脆的破殼聲響起，幼鳥的啼鳴與先後盛開的高山花卉交織在一起，宣告著整座森林的甦醒。</p>
            </div>
        </div>
    </section>

    <section id="summer" class="season-container">
        <div class="sticky-bg">
            <img src="/pianezzo/images/summer-bg.jpg" alt="Summer Atmosphere">
            <div class="bg-overlay"></div>
        </div>
        <div class="scroll-content layout-right">
            <div class="content-card">
                <span class="season-tag">Summer Fullness</span>
                <h3>豔陽與繁盛</h3>
                <p>當豔陽高照，整座山林進入了生命力最為旺盛的極致盛夏。為了捕捉最充足的光線，龐大的樹冠層將葉片轉為濃郁的深綠，交織成一片遮天蔽日的清涼畫布。</p>
                <br>
                <p>在充沛的日照與山泉滋養下，枝頭上的果實逐漸膨大。空氣中開始瀰漫著微甜的氣息，每一顆果實都在溫暖的微風中默默累積著重量與豐饒。</p>
            </div>
        </div>
    </section>

    <section id="autumn" class="season-container">
        <div class="sticky-bg">
            <img src="/pianezzo/images/autumn-bg.jpg" alt="Autumn Atmosphere">
            <div class="bg-overlay"></div>
        </div>
        <div class="scroll-content layout-left">
            <div class="content-card">
                <span class="season-tag">Autumn Resonance</span>
                <h3>斑斕與共鳴</h3>
                <p>隨著日照漸短，森林的色調開始發生壯麗的過渡，整片翠綠逐漸轉為深邃的紅褐色與古銅色。在厚厚的落葉層下，微觀世界正悄悄熱鬧起來，各式各樣的野生香菇與蕈類依循著秋氣靜靜冒出。</p>
                <br>
                <p>冷冽清脆的空氣中，不時傳來高山動物發情求偶的深沉鳴叫。那渾厚的迴響穿透整片紅褐色的樹林，成為秋季山野裡最充滿原始張力的生命共鳴。</p>
            </div>
        </div>
    </section>

    <section id="winter" class="season-container">
        <div class="sticky-bg">
            <img src="/pianezzo/images/winter-bg.jpg" alt="Winter Atmosphere">
            <div class="bg-overlay"></div>
        </div>
        <div class="scroll-content layout-center">
            <div class="content-card winter-card">
                <span class="season-tag">Winter Silence</span>
                <h3>極致寂靜</h3>
                <p>萬物最終安靜下來。</p>
                <br>
                <p>大雪落下，覆蓋了所有的色彩與動態。森林不再喧嘩，昆蟲與植物進入了深沉的蟄伏。這並非終結，而是整座 Alpe Pianezzo 在無邊的寂靜中深呼吸，於白色的被褥下安穩沉睡，靜靜積蓄著等待下一次破土的力量。</p>
            </div>
        </div>
    </section>

</div>

<style>
/* 啟用全域平滑滾動，讓點擊導覽列時擁有過場加速感 */
html {
    scroll-behavior: smooth;
}

/* 破框設定：強制撐滿整個瀏覽器視窗 */
.seasons-wrapper {
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
    background-color: #f4f1ea;
    box-sizing: border-box;
}

/* 懸浮快速導覽列 */
.season-quick-nav {
    position: fixed;
    top: 30px;
    right: 4%;
    z-index: 1000;
    background: rgba(244, 241, 234, 0.85);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    padding: 8px 24px;
    border-radius: 50px;
    display: flex;
    gap: 20px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.08);
    border: 1px solid rgba(62, 39, 35, 0.1);
}

.season-quick-nav a {
    font-family: 'Lora', serif;
    color: #3e2723;
    text-decoration: none;
    font-size: 0.95rem;
    font-weight: bold;
    letter-spacing: 1px;
    transition: color 0.3s ease;
}

.season-quick-nav a:hover {
    color: #A67C52;
}

/* 獨立季節區塊：設定足夠的高度讓粘性滾動發生 */
.season-container {
    position: relative;
    min-height: 220vh; /* 提供足夠的滾動行程 */
    scroll-margin-top: 0px; /* 確保錨點跳轉時頂部精準對齊 */
}

#winter {
    min-height: 150vh; /* 冬季內容少，行程縮短以配合寂靜感 */
}

/* 粘性背景設定 */
.sticky-bg {
    position: sticky;
    top: 0;
    width: 100vw;
    height: 100vh;
    height: 100svh; /* 優先使用 svh 避開手機網址列縮放干擾 */
    z-index: 1;
    overflow: hidden;
    will-change: transform;
}

.sticky-bg img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

/* 漸層暗色遮罩：確保任何亮度的背景圖都不會吃掉文字 */
.bg-overlay {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: linear-gradient(to bottom, rgba(0,0,0,0.1) 0%, rgba(0,0,0,0.35) 100%);
}

/* 滾動內容層 */
.scroll-content {
    position: relative;
    z-index: 2;
    padding-top: 80vh; /* 讓第一眼完整展現背景，往下滑才帶出文字卡片 */
    padding-bottom: 40vh;
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    box-sizing: border-box;
    padding-left: 5%;
    padding-right: 5%;
}

/* 錯落排版配置 */
.layout-left { justify-content: flex-start; }
.layout-right { justify-content: flex-end; }
.layout-center { justify-content: center; align-items: center; padding-top: 50vh; }

/* 實體文字卡片設計 (延續底色與中文字體美學) */
.content-card {
    background-color: #f4f1ea;
    padding: 70px 60px;
    border-radius: 2px;
    box-shadow: 0 20px 60px rgba(0,0,0,0.2);
    max-width: 550px;
    border-top: 3px solid #A67C52;
}

.winter-card {
    max-width: 650px;
    text-align: center;
    border-top: none;
    background-color: rgba(244, 241, 234, 0.95);
}

.season-tag {
    display: block;
    font-family: 'Lora', serif;
    font-size: 0.85rem;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: #A67C52;
    margin-bottom: 15px;
}

.content-card h3 {
    font-family: 'Noto Serif TC', serif;
    font-size: 2.5rem;
    color: #3e2723;
    margin-top: 0;
    margin-bottom: 25px;
    line-height: 1.2;
    font-weight: bold;
}

.content-card p {
    font-family: 'Noto Serif TC', serif;
    font-size: 1.15rem;
    line-height: 2.1;
    color: #2b2b2b;
    margin: 0;
    text-align: justify;
}

.winter-card p {
    text-align: center;
}

/* 行動裝置適配 */
@media (max-width: 768px) {
    .season-quick-nav {
        top: 15px;
        right: 50%;
        transform: translateX(50%);
        padding: 6px 18px;
        gap: 12px;
        width: max-content;
    }
    .season-quick-nav a { font-size: 0.85rem; }
    
    .scroll-content {
        padding-top: 65vh;
        padding-bottom: 25vh;
    }
    
    .content-card {
        padding: 40px 30px;
        max-width: 100%;
    }
    
    .content-card h3 { font-size: 2rem; }
    .content-card p { font-size: 1.05rem; line-height: 1.9; }
}
</style>
