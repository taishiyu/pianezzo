---
title: "Contact"
featured_image: "/pianezzo/images/contact.jpg"
description: "聽見山林與工坊的迴響。"
layout: "single"
---

<div class="contact-master-container">

<div class="contact-layout">

<div class="contact-info-section">
<h3>Inquire & Connect</h3>
<p class="contact-intro">Whether you are inquiring about acquiring our handcrafted pieces, discussing a bespoke furniture commission, or booking our permanent walks and seasonal workshops, please feel free to reach out through the form below or via email. And if you happen to find yourself passing through the Antrona Valley, you are always welcome to wander up the mountain, brush off the sawdust, and share a cup of tea with us.</p>

<form class="pure-contact-form" id="alpine-contact-form" action="https://formspree.io/f/mqenrapr" method="POST">
<div class="form-group">
<label>Name</label>
<input type="text" name="name" required>
</div>
<div class="form-group">
<label>Email</label>
<input type="email" name="email" required>
</div>
<div class="form-group">
<label>Purpose</label>
<select name="purpose">
<option value="artifacts">Selected Pieces</option>
<option value="bespoke">Bespoke Commission</option>
<option value="gatherings">Workshops & Walks</option>
<option value="other">Collaboration</option>
</select>
</div>
<div class="form-group">
<label>Message</label>
<textarea name="message" rows="6" required></textarea>
</div>
<button type="submit" id="submit-btn" class="contact-submit-btn">Send Message</button>
</form>

<div id="form-success-status" style="display:none;padding:40px;background:#fff;border-top:3px solid #A67C52;box-shadow:0 20px 50px rgba(0,0,0,0.04);font-family:'Lora',serif;text-align:left;">
<h4 style="color:#A67C52;font-size:1.5rem;margin:0 0 15px 0;">Thank You!</h4>
<p style="color:#444;font-size:1.05rem;line-height:1.8;margin:0;">Your message has been sent successfully. We will brush off the sawdust and get back to you within 24-48 hours.</p>
</div>

<script>
var form = document.getElementById("alpine-contact-form");
var statusDiv = document.getElementById("form-success-status");
var btn = document.getElementById("submit-btn");
async function handleSubmit(event) {
event.preventDefault();
btn.disabled = true;
btn.innerText = "Sending...";
var data = new FormData(event.target);
fetch(event.target.action, {
method: form.method,
body: data,
headers: { 'Accept': 'application/json' }
}).then(response => {
if (response.ok) {
form.style.display = "none";
statusDiv.style.display = "block";
form.reset();
} else {
alert("Oops! There was a problem. Please try again.");
btn.disabled = false;
btn.innerText = "Send Message";
}
}).catch(error => {
alert("Connection error. Please check your network.");
btn.disabled = false;
btn.innerText = "Send Message";
});
}
form.addEventListener("submit", handleSubmit);
</script>
</form>

<div class="contact-meta-box">
<div class="meta-item">
<h4>Response Time</h4>
<p>24-48 hr (English, Italiano, Traditional Chinese OK)</p>
</div>
<div class="meta-item">
<h4>Welcome Drop-ins</h4>
<p>Walk-ins Welcome.Take a coffee with us.</p>
</div>
</div>
</div>

<div class="contact-map-section">
<h3>Location</h3>
<span class="location-tag">Val d'Ossola, Piedmont, Italy</span>
<p class="map-desc">Near by Domodossola, around 1.5 hr from Milan by train。</p>

<div class="google-map-wrapper">
<iframe src="https://www.google.com/maps/embed?pb=!1m13!1m8!1m3!1d7334.831581346374!2d8.179756786160343!3d46.05332525804184!3m2!1i1024!2i768!4f13.1!3m2!1m1!2zNDbCsDAzJzIyLjAiTiA4wrAxMCc1My42IkU!5e0!3m2!1szh-TW!2sit!4v1778854926074!5m2!1szh-TW!2sit" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
</div>
</div>

</div>

</div>

<style>
html { scroll-behavior: smooth; }
.contact-master-container { width: 100vw; position: relative; left: 50%; right: 50%; margin-left: -50vw; margin-right: -50vw; background: #f4f1ea; min-height: 100vh; padding-bottom: 150px; overflow-x: hidden; }
.contact-layout { max-width: 1200px; margin: 60px auto 0 auto; padding: 0 5%; display: flex; gap: 80px; }
.contact-info-section { flex: 1.2; text-align: left; }
.contact-map-section { flex: 1; text-align: left; position: sticky; top: 40px; height: max-content; }
.contact-info-section h3, .contact-map-section h3 { font-family: 'Lora', serif; font-size: 2.2rem; margin-bottom: 25px; color: #1a1a1a; }
.contact-intro, .map-desc { font-family: 'Lora', serif; font-size: 1.05rem; line-height: 1.8; color: #555; margin-bottom: 40px; }
.location-tag { font-family: 'Lora', serif; font-size: 0.9rem; letter-spacing: 2px; color: #A67C52; font-weight: bold; text-transform: uppercase; display: block; margin-bottom: 15px; }
.pure-contact-form { display: flex; flex-direction: column; gap: 25px; margin-bottom: 50px; }
.form-group { display: flex; flex-direction: column; gap: 8px; }
.form-group label { font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; color: #444; text-transform: uppercase; letter-spacing: 0.5px; }
.form-group input, .form-group select, .form-group textarea { font-family: 'Lora', serif; padding: 14px; border: 1px solid rgba(166, 124, 82, 0.2); background: #fff; border-radius: 2px; font-size: 1rem; color: #333; outline: none; transition: border 0.3s; }
.form-group input:focus, .form-group select:focus, .form-group textarea:focus { border: 1px solid #A67C52; }
.contact-submit-btn { font-family: 'Lora', serif; font-size: 0.85rem; font-weight: bold; color: #fff; background: #A67C52; border: none; padding: 15px 30px; border-radius: 2px; cursor: pointer; transition: background 0.3s; text-transform: uppercase; letter-spacing: 1px; width: max-content; }
.contact-submit-btn:hover { background: #8e653f; }
.contact-meta-box { border-top: 1px solid #e2ded5; padding-top: 35px; display: flex; flex-direction: column; gap: 25px; }
.meta-item h4 { font-family: 'Lora', serif; font-size: 1rem; color: #A67C52; margin: 0 0 8px 0; }
.meta-item p { font-family: 'Lora', serif; font-size: 0.95rem; line-height: 1.6; color: #666; margin: 0; }
.google-map-wrapper { width: 100%; aspect-ratio: 1 / 1; border-radius: 2px; overflow: hidden; box-shadow: 0 20px 50px rgba(0,0,0,0.04); border-top: 3px solid #A67C52; background: #eae6df; }
.google-map-wrapper iframe { display: block; width: 100%; height: 100%; }
@media (max-width: 1024px) { .contact-layout { flex-direction: column; gap: 6px; } .contact-map-section { position: relative; top: 0; margin-top: 60px; } .google-map-wrapper { aspect-ratio: 16 / 9; } }
</style>
