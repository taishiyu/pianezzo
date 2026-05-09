---
title: "The Seasons"
featured_image: "/pianezzo/images/season-cover.jpg"
description: "The breathing rhythm of Alpe Pianezzo."
layout: "single"
---

<nav class="season-quick-nav">
<a href="#spring">Spring</a>
<a href="#summer">Summer</a>
<a href="#autumn">Autumn</a>
<a href="#winter">Winter</a>
</nav>

<div class="seasons-wrapper">

<section id="spring" class="season-deck-container">
<div class="sticky-bg">
<img src="/pianezzo/images/spring-bg.jpg" alt="Spring Atmosphere">
<div class="bg-overlay"></div>
</div>

<div class="cards-deck" onclick="flipCard(this)">
<div class="content-card active-card text-only">
<span class="season-tag">Spring 01</span>
<h3>The Sequence of Life</h3>
<p>When spring quietly arrives at 1,100 meters, a delicate sequence of life begins to unfold. From the damp earth, resilient wild nettles emerge first.</p>
<div class="flip-hint">Click to flip →</div>
</div>

<div class="content-card split-layout">
<div class="card-image"><img src="/pianezzo/images/spring-vibe-1.jpg" alt="Spring detail"></div>
<div class="card-text">
<span class="season-tag">Spring 02</span>
<h3>The Return of Birds</h3>
<p>The canopy fills with the industrious sounds of nest-building. Parent birds weave dried grass and moss into safe havens.</p>
<div class="flip-hint">Click to flip →</div>
</div>
</div>

<div class="content-card split-layout">
<div class="card-image"><img src="/pianezzo/images/spring-vibe-2.jpg" alt="Spring detail"></div>
<div class="card-text">
<span class="season-tag">Spring 03</span>
<h3>The Nettle Harvest</h3>
<p>Nettles provide our first fresh nutrients. We gather them while the morning dew still clings to the leaves.</p>
<div class="flip-hint">Click to flip →</div>
</div>
</div>

<div class="content-card split-layout">
<div class="card-image"><img src="/pianezzo/images/spring-vibe-3.jpg" alt="Spring detail"></div>
<div class="card-text">
<span class="season-tag">Spring 04</span>
<h3>Emerging Blooms</h3>
<p>By late spring, the alpine flora reaches its peak. Every corner of the land is a nursery for new life.</p>
<div class="flip-hint">Click to flip →</div>
</div>
</div>
</div>
</section>

</div>

<script>
function flipCard(deck) {
const cards = deck.querySelectorAll('.content-card');
if (cards.length < 2) return;
const topCard = cards[0];
topCard.style.transform = 'translate(-120%, -20%) rotate(-15deg)';
topCard.style.opacity = '0';
setTimeout(() => {
topCard.style.transform = '';
topCard.style.opacity = '1';
deck.appendChild(topCard);
updateCardZIndex(deck);
}, 500);
}
function updateCardZIndex(deck) {
const cards = deck.querySelectorAll('.content-card');
cards.forEach((card, index) => {
card.style.zIndex = cards.length - index;
if (index === 0) {
card.style.transform = 'translate(0, 0)';
card.classList.add('active-card');
} else {
card.style.transform = `translate(${index * 5}px, ${index * 5}px)`;
card.classList.remove('active-card');
}
});
}
document.querySelectorAll('.cards-deck').forEach(updateCardZIndex);
</script>

<style>
.seasons-wrapper { width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; background: #f4f1ea; overflow: hidden; }
.season-deck-container { position: relative; height: 100vh; width: 100%; overflow: hidden; display: flex; align-items: center; justify-content: flex-start; }
.sticky-bg { position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 1; }
.sticky-bg img { width: 100%; height: 100%; object-fit: cover; }
.bg-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.15); }
.cards-deck { position: relative; z-index: 10; margin-left: 8%; width: 950px; height: 600px; cursor: pointer; }
.content-card { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: #f4f1ea; padding: 60px 80px; border-radius: 2px; box-shadow: 0 10px 40px rgba(0,0,0,0.1); display: flex; flex-direction: column; justify-content: center; transition: all 0.5s cubic-bezier(0.23, 1, 0.32, 1); border-left: 4px solid #A67C52; }
.split-layout { flex-direction: row; gap: 50px; text-align: left; }
.card-image { flex: 1.2; }
.card-image img { width: 100%; height: auto; border-radius: 2px; }
.card-text { flex: 1; text-align: left; }
.season-tag { font-family: 'Lora', serif; font-size: 0.8rem; letter-spacing: 2px; color: #A67C52; margin-bottom: 15px; display: block; text-align: left; }
.content-card h3 { font-family: 'Lora', serif; font-size: 2.8rem; margin-bottom: 20px; color: #1a1a1a; text-align: left; }
.content-card p { font-family: 'Lora', serif; font-size: 1.2rem; line-height: 1.8; color: #333; text-align: left; }
.flip-hint { margin-top: auto; font-size: 0.8rem; color: #A67C52; font-style: italic; opacity: 0.6; text-align: left; }
.season-quick-nav { position: fixed; top: 30px; right: 4%; z-index: 1000; background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(8px); padding: 10px 25px; border-radius: 50px; display: flex; gap: 20px; box-shadow: 0 4px 20px rgba(0,0,0,0.05); }
.season-quick-nav a { font-family: 'Lora', serif; color: #3e2723; text-decoration: none; font-size: 0.9rem; font-weight: bold; }
@media (max-width: 1024px) {
.cards-deck { width: 92%; margin-left: 4%; height: 70vh; }
.split-layout { flex-direction: column; padding: 40px; }
}
</style>
