---
title: "Habitant"
featured_image: "/pianezzo/images/habitant.jpg"
description: "與我們共同棲居於此的生命群像。"
layout: "single"
---

<div class="habitant-master-container">

<input type="radio" id="hab-flora" name="hab-deck" checked hidden>
<input type="radio" id="hab-birds" name="hab-deck" hidden>
<input type="radio" id="hab-mammals" name="hab-deck" hidden>
<input type="radio" id="hab-amphibians" name="hab-deck" hidden>

<div class="deck-wrapper">

<div class="habitant-card card-flora">
<div class="card-inner">
<span class="card-category">FLORA ｜ 常見草木</span>
<h3>Flora & Timber</h3>
<p>落葉松、歐洲雲杉與百年栗樹構成了這片山林的古老骨架。初春時節，野韭菜與阿爾卑斯高山草本在果園邊緣悄然甦醒，為酸種麵包與日常採集提供了最純淨的季節滋味。</p>
<div class="deck-nav">
<label for="hab-birds" class="next-btn">Next: Birds ｜ 鳥類 →</label>
</div>
</div>
</div>

<div class="habitant-card card-birds">
<div class="card-inner">
<span class="card-category">FAUNA ｜ 鳥類居民</span>
<h3>Avian Residents</h3>
<p>黑啄木鳥的規律敲擊聲是工坊最天然的背景音樂。金雕偶爾在晴朗的高空盤旋，而盤踞在灌木叢中的黑頭鶯與紅尾鴝，則用靈動的鳴叫聲宣告著山谷的晨昏更迭。</p>
<div class="deck-nav">
<label for="hab-mammals" class="next-btn">Next: Mammals ｜ 哺乳類 →</label>
</div>
</div>
</div>

<div class="habitant-card card-mammals">
<div class="card-inner">
<span class="card-category">FAUNA ｜ 哺乳動物</span>
<h3>Mountain Mammals</h3>
<p>野鹿與歐洲野兔常在清晨或薄霧中造訪果園，品嚐散落的遺傳品種蘋果。石貂與狐狸則在石牆縫隙間留下一條條神祕的蹤跡，牠們是這片土地上最安靜的守護者。</p>
<div class="deck-nav">
<label for="hab-amphibians" class="next-btn">Next: Amphibians ｜ 兩棲類 →</label>
</div>
</div>
</div>

<div class="habitant-card card-amphibians">
<div class="card-inner">
<span class="card-category">FAUNA ｜ 兩棲與其它</span>
<h3>Amphibians & Micro-fauna</h3>
<p>在苔蘚溪流與古老石溝的陰影下，阿爾卑斯高山蠑螈在雨後緩慢爬行。獨角仙與各式授粉昆蟲則在腐木與花叢間穿梭，默默維持著工坊周邊微小而關鍵的生態循環。</p>
<div class="deck-nav">
<label for="hab-flora" class="next-btn">Back to First: Flora ｜ 草木 ↺</label>
</div>
</div>
</div>

</div>

<div class="deck-dots">
<label for="hab-flora" class="dot-flora"></label>
<label for="hab-birds" class="dot-birds"></label>
<label for="hab-mammals" class="dot-mammals"></label>
<label for="hab-amphibians" class="dot-amphibians"></label>
</div>

</div>

<style>
html { scroll-behavior: smooth; }
.habitant-master-container { width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; background: #f4f1ea; min-height: 100vh; padding-top: 80px; padding-bottom: 150px; overflow-x: hidden; display: flex; flex-direction: column; align-items: center; justify-content: center; }
.deck-wrapper { position: relative; width: 90%; max-width: 650px; aspect-ratio: 4 / 3; margin: 0 auto; perspective: 1000px; }
.habitant-card { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: #fff; border-top: 4px solid #A67C52; box-shadow: 0 30px 60px rgba(0,0,0,0.05); border-radius: 2px; transition: all 0.6s cubic-bezier(0.25, 1, 0.5, 1); opacity: 0; pointer-events: none; transform: translateZ(-100px) translateY(20px) rotateX(-4deg); z-index: 1; box-sizing: border-box; }
.card-inner { padding: 50px; height: 100%; display: flex; flex-direction: column; justify-content: space-between; text-align: left; box-sizing: border-box; }
.card-category { font-family: 'Lora', serif; font-size: 0.8rem; letter-spacing: 2px; color: #A67C52; font-weight: bold; text-transform: uppercase; }
.card-inner h3 { font-family: 'Lora', serif; font-size: 2.2rem; margin: 15px 0 20px 0; color: #1a1a1a; }
.card-inner p { font-family: 'Lora', serif; font-size: 1.05rem; line-height: 1.8; color: #444; flex-grow: 1; margin: 0 0 30px 0; }
.deck-nav { margin-top: auto; display: flex; justify-content: flex-end; }
.next-btn { font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; color: #A67C52; border: 1px solid #A67C52; padding: 10px 22px; border-radius: 2px; cursor: pointer; transition: all 0.3s; text-transform: uppercase; letter-spacing: 1px; }
.next-btn:hover { background: #A67C52; color: #fff; }

/* 核心切換邏輯：當前被選中的卡片翻到最前面 */
#hab-flora:checked ~ .deck-wrapper .card-flora,
#hab-birds:checked ~ .deck-wrapper .card-birds,
#hab-mammals:checked ~ .deck-wrapper .card-mammals,
#hab-amphibians:checked ~ .deck-wrapper .card-amphibians { opacity: 1; pointer-events: auto; transform: translateZ(0) translateY(0) rotateX(0); z-index: 10; }

/* 後一層卡片的微幅露出版式 (製造層疊堆疊感) */
#hab-flora:checked ~ .deck-wrapper .card-birds,
#hab-birds:checked ~ .deck-wrapper .card-mammals,
#hab-mammals:checked ~ .deck-wrapper .card-amphibians,
#hab-amphibians:checked ~ .deck-wrapper .card-flora { opacity: 0.5; transform: translateZ(-40px) translateY(15px) scale(0.96); z-index: 5; }

/* 後兩層卡片的微幅沉底版式 */
#hab-flora:checked ~ .deck-wrapper .card-mammals,
#hab-birds:checked ~ .deck-wrapper .card-amphibians,
#hab-mammals:checked ~ .deck-wrapper .card-flora,
#hab-amphibians:checked ~ .deck-wrapper .card-birds { opacity: 0.15; transform: translateZ(-80px) translateY(30px) scale(0.92); z-index: 2; }

/* 底部進度點樣式 */
.deck-dots { display: flex; gap: 12px; margin-top: 50px; justify-content: center; }
.deck-dots label { width: 9px; height: 9px; border-radius: 50%; background: rgba(166, 124, 82, 0.2); cursor: pointer; transition: all 0.3s; }
#hab-flora:checked ~ .deck-dots .dot-flora,
#hab-birds:checked ~ .deck-dots .dot-birds,
#hab-mammals:checked ~ .deck-dots .dot-mammals,
#hab-amphibians:checked ~ .deck-dots .dot-amphibians { background: #A67C52; transform: scale(1.3); }

/* 行動裝置極致自適應 */
@media (max-width: 768px) { .deck-wrapper { aspect-ratio: auto; height: 460px; } .card-inner { padding: 35px 25px; } .card-inner h3 { font-size: 1.8rem; } .card-inner p { font-size: 1rem; line-height: 1.7; } }
</style>
