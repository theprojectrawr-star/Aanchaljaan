<!DOCTYPE html>  
  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>For You, My Love 💕</title>  
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300;1,400&display=swap" rel="stylesheet">  
<style>  
  * { margin: 0; padding: 0; box-sizing: border-box; }  
  
:root {  
–rose: #e8637a;  
–blush: #f9a8b8;  
–petal: #fde8ed;  
–gold: #c9956e;  
–deep: #3d1a24;  
–soft: #fff5f7;  
}  
  
body {  
background: var(–soft);  
min-height: 100vh;  
font-family: ‘Cormorant Garamond’, serif;  
overflow-x: hidden;  
cursor: url(“data:image/svg+xml,%3Csvg xmlns=‘http://www.w3.org/2000/svg’ width=‘24’ height=‘24’ viewBox=‘0 0 24 24’%3E%3Ctext y=‘20’ font-size=‘20’%3E❤️%3C/text%3E%3C/svg%3E”), auto;  
}  
  
/* Floating petals background */  
.petals-container {  
position: fixed;  
top: 0; left: 0;  
width: 100%; height: 100%;  
pointer-events: none;  
z-index: 0;  
overflow: hidden;  
}  
  
.petal {  
position: absolute;  
top: -60px;  
font-size: 1.5rem;  
animation: fall linear infinite;  
opacity: 0.7;  
}  
  
@keyframes fall {  
0%   { transform: translateY(-60px) rotate(0deg) translateX(0); opacity: 0; }  
10%  { opacity: 0.8; }  
90%  { opacity: 0.6; }  
100% { transform: translateY(110vh) rotate(720deg) translateX(60px); opacity: 0; }  
}  
  
/* Hero section */  
.hero {  
position: relative;  
z-index: 1;  
min-height: 100vh;  
display: flex;  
flex-direction: column;  
align-items: center;  
justify-content: center;  
padding: 40px 20px;  
text-align: center;  
}  
  
.hearts-top {  
font-size: 2.5rem;  
letter-spacing: 8px;  
animation: pulse 2s ease-in-out infinite;  
margin-bottom: 24px;  
}  
  
@keyframes pulse {  
0%, 100% { transform: scale(1); }  
50%       { transform: scale(1.15); }  
}  
  
.envelope {  
width: 120px; height: 90px;  
background: white;  
border: 2px solid var(–blush);  
border-radius: 4px;  
position: relative;  
margin: 0 auto 40px;  
box-shadow: 0 8px 32px rgba(232,99,122,0.2);  
animation: float 3s ease-in-out infinite;  
overflow: hidden;  
}  
  
.envelope::before {  
content: ‘’;  
position: absolute;  
top: 0; left: 0;  
width: 100%; height: 100%;  
background: linear-gradient(135deg, var(–blush) 50%, transparent 50%);  
opacity: 0.3;  
}  
  
.envelope::after {  
content: ‘💌’;  
font-size: 2.5rem;  
position: absolute;  
top: 50%; left: 50%;  
transform: translate(-50%, -55%);  
}  
  
@keyframes float {  
0%, 100% { transform: translateY(0px); }  
50%       { transform: translateY(-12px); }  
}  
  
.main-title {  
font-family: ‘Playfair Display’, serif;  
font-size: clamp(2.8rem, 8vw, 5.5rem);  
color: var(–deep);  
line-height: 1.1;  
font-style: italic;  
animation: fadeInUp 1.2s ease both;  
margin-bottom: 12px;  
}  
  
.subtitle {  
font-size: clamp(1rem, 3vw, 1.4rem);  
color: var(–rose);  
letter-spacing: 4px;  
text-transform: uppercase;  
animation: fadeInUp 1.2s 0.3s ease both;  
margin-bottom: 50px;  
font-weight: 300;  
}  
  
@keyframes fadeInUp {  
from { opacity: 0; transform: translateY(30px); }  
to   { opacity: 1; transform: translateY(0); }  
}  
  
/* Letter card */  
.letter-card {  
background: white;  
border: 1px solid #f5c5d0;  
border-radius: 2px;  
max-width: 680px;  
width: 100%;  
padding: 56px 48px;  
position: relative;  
box-shadow: 0 20px 60px rgba(232,99,122,0.12), 0 4px 16px rgba(0,0,0,0.05);  
animation: fadeInUp 1.2s 0.5s ease both;  
margin-bottom: 50px;  
}  
  
.letter-card::before {  
content: ‘’;  
position: absolute;  
top: 8px; left: 8px; right: 8px; bottom: 8px;  
border: 1px solid #fde0e8;  
pointer-events: none;  
}  
  
.letter-decoration {  
position: absolute;  
font-size: 3rem;  
opacity: 0.15;  
}  
.letter-decoration.tl { top: 16px; left: 20px; }  
.letter-decoration.tr { top: 16px; right: 20px; }  
.letter-decoration.bl { bottom: 16px; left: 20px; }  
.letter-decoration.br { bottom: 16px; right: 20px; }  
  
.dear-line {  
font-size: 1.2rem;  
color: var(–rose);  
font-style: italic;  
margin-bottom: 20px;  
display: block;  
}  
  
.letter-text {  
font-size: 1.15rem;  
line-height: 1.95;  
color: #5a3040;  
font-weight: 300;  
}  
  
.letter-text p + p { margin-top: 20px; }  
  
.signature {  
margin-top: 32px;  
text-align: right;  
font-family: ‘Playfair Display’, serif;  
font-style: italic;  
font-size: 1.4rem;  
color: var(–rose);  
}  
  
/* Distance section */  
.distance-section {  
position: relative;  
z-index: 1;  
padding: 60px 20px;  
text-align: center;  
}  
  
.distance-display {  
display: flex;  
align-items: center;  
justify-content: center;  
gap: 24px;  
flex-wrap: wrap;  
margin: 40px 0;  
}  
  
.location-badge {  
background: white;  
border: 1px solid var(–blush);  
border-radius: 50px;  
padding: 14px 28px;  
font-size: 1rem;  
color: var(–deep);  
box-shadow: 0 4px 20px rgba(232,99,122,0.12);  
animation: float 3s ease-in-out infinite;  
}  
  
.location-badge:nth-child(3) { animation-delay: 1.5s; }  
  
.heart-line {  
font-size: 2rem;  
animation: pulse 1.5s ease-in-out infinite;  
color: var(–rose);  
}  
  
.section-title {  
font-family: ‘Playfair Display’, serif;  
font-size: clamp(1.8rem, 5vw, 3rem);  
color: var(–deep);  
font-style: italic;  
margin-bottom: 16px;  
}  
  
/* Flower row */  
.flower-row {  
display: flex;  
justify-content: center;  
gap: 8px;  
font-size: 2rem;  
margin: 30px 0;  
animation: fadeInUp 1s ease both;  
}  
  
.flower-row span {  
display: inline-block;  
animation: sway 2s ease-in-out infinite;  
}  
  
.flower-row span:nth-child(even) { animation-direction: reverse; }  
.flower-row span:nth-child(3n)   { animation-delay: 0.5s; }  
  
@keyframes sway {  
0%, 100% { transform: rotate(-8deg); }  
50%       { transform: rotate(8deg); }  
}  
  
/* Reasons section */  
.reasons-section {  
position: relative;  
z-index: 1;  
padding: 60px 20px;  
max-width: 900px;  
margin: 0 auto;  
}  
  
.reasons-grid {  
display: grid;  
grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));  
gap: 20px;  
margin-top: 40px;  
}  
  
.reason-card {  
background: white;  
border: 1px solid #f5c5d0;  
border-radius: 2px;  
padding: 32px 24px;  
text-align: center;  
box-shadow: 0 4px 20px rgba(232,99,122,0.08);  
transition: transform 0.3s ease, box-shadow 0.3s ease;  
animation: fadeInUp 0.8s ease both;  
}  
  
.reason-card:hover {  
transform: translateY(-6px);  
box-shadow: 0 12px 40px rgba(232,99,122,0.18);  
}  
  
.reason-card:nth-child(2) { animation-delay: 0.15s; }  
.reason-card:nth-child(3) { animation-delay: 0.3s; }  
.reason-card:nth-child(4) { animation-delay: 0.45s; }  
.reason-card:nth-child(5) { animation-delay: 0.6s; }  
.reason-card:nth-child(6) { animation-delay: 0.75s; }  
  
.reason-icon { font-size: 2.5rem; margin-bottom: 14px; }  
.reason-title {  
font-family: ‘Playfair Display’, serif;  
font-size: 1.1rem;  
color: var(–deep);  
margin-bottom: 8px;  
}  
.reason-text {  
font-size: 0.95rem;  
color: #7a5060;  
line-height: 1.7;  
font-weight: 300;  
}  
  
/* Countdown / promise section */  
.promise-section {  
position: relative;  
z-index: 1;  
background: var(–deep);  
color: white;  
padding: 80px 20px;  
text-align: center;  
overflow: hidden;  
}  
  
.promise-section::before {  
content: ‘’;  
position: absolute;  
inset: 0;  
background: radial-gradient(ellipse at center, rgba(232,99,122,0.2) 0%, transparent 70%);  
}  
  
.promise-title {  
font-family: ‘Playfair Display’, serif;  
font-size: clamp(2rem, 6vw, 4rem);  
font-style: italic;  
color: var(–blush);  
margin-bottom: 24px;  
position: relative;  
}  
  
.promise-text {  
font-size: 1.2rem;  
line-height: 1.9;  
color: rgba(255,255,255,0.8);  
max-width: 580px;  
margin: 0 auto 40px;  
font-weight: 300;  
position: relative;  
}  
  
.big-heart {  
font-size: 5rem;  
animation: heartbeat 1.5s ease-in-out infinite;  
display: block;  
position: relative;  
}  
  
@keyframes heartbeat {  
0%, 100% { transform: scale(1); }  
14%       { transform: scale(1.2); }  
28%       { transform: scale(1); }  
42%       { transform: scale(1.15); }  
56%       { transform: scale(1); }  
}  
  
/* Footer */  
footer {  
position: relative;  
z-index: 1;  
text-align: center;  
padding: 40px 20px;  
color: var(–rose);  
font-style: italic;  
font-size: 1rem;  
}  
  
/* Sparkle cursor trail effect */  
.sparkle {  
position: fixed;  
pointer-events: none;  
font-size: 1.2rem;  
animation: sparkle-fade 1s ease forwards;  
z-index: 9999;  
}  
  
@keyframes sparkle-fade {  
0%   { opacity: 1; transform: translateY(0) scale(1); }  
100% { opacity: 0; transform: translateY(-40px) scale(0.3); }  
}  
  
@media (max-width: 600px) {  
.letter-card { padding: 36px 24px; }  
}  
</style>  
  
</head>  
<body>  
  
<!-- Floating petals -->  
  
<div class="petals-container" id="petals"></div>  
  
<!-- Hero -->  
  
<section class="hero">  
  <div class="hearts-top">🌸 💕 🌸</div>  
  <div class="envelope"></div>  
  <h1 class="main-title">My Heart Is Yours</h1>  
  <p class="subtitle">Across every mile, every moment</p>  
  
  <div class="letter-card">  
    <div class="letter-decoration tl">🌹</div>  
    <div class="letter-decoration tr">🌷</div>  
    <div class="letter-decoration bl">🌺</div>  
    <div class="letter-decoration br">💐</div>  
  
```  
<span class="dear-line">My dearest love,</span>  
<div class="letter-text">  
  <p>  
    There are miles between us — roads and skies and time zones — and yet somehow,  
    every single morning, the very first thing I feel is <em>you</em>. Not distance.  
    Not absence. Just you, like a warmth that doesn't need proximity to be real.  
  </p>  
  <p>  
    I am so deeply, completely in love with you. The kind of love that doesn't  
    quiet down when things get hard, that doesn't shrink when the wait stretches long.  
    It just grows — quietly, stubbornly, beautifully — like a flower that blooms  
    even through the coldest season because it simply can't help itself.  
  </p>  
  <p>  
    You make me want to be better, feel more, laugh louder, and dream bigger.  
    You are the reason I look forward to every tomorrow. Every call, every message,  
    every small moment we share across the distance feels like the whole world  
    compressed into something precious and just ours.  
  </p>  
  <p>  
    I want you to know — truly know — that you are never far from me.  
    You live in my thoughts, in the songs I hear, in quiet evenings and in everything  
    that is good. I am yours, fully and without question.  
    And I cannot wait for the day when distance is just a story we tell.  
  </p>  
</div>  
<div class="signature">Forever yours 💕</div>  
```  
  
  </div>  
</section>  
  
<!-- Flowers -->  
  
<div class="distance-section">  
  <div class="flower-row">  
    <span>🌸</span><span>🌺</span><span>🌷</span><span>🌹</span><span>💐</span>  
    <span>🌼</span><span>🌸</span><span>🌺</span><span>🌷</span><span>🌹</span>  
    <span>🌸</span><span>🌼</span><span>💐</span>  
  </div>  
  
  <h2 class="section-title">Two hearts, one love</h2>  
  <p style="color:#7a5060;font-size:1.1rem;margin-bottom:8px;font-weight:300;">  
    No matter how far apart we are...  
  </p>  
  
  <div class="distance-display">  
    <div class="location-badge">💙 Me, right here</div>  
    <div class="heart-line">❤️ ——— ❤️</div>  
    <div class="location-badge">💕 You, my everything</div>  
  </div>  
</div>  
  
<!-- Reasons -->  
  
<section class="reasons-section">  
  <h2 class="section-title" style="text-align:center;">Little reasons I love you</h2>  
  
  <div class="reasons-grid">  
    <div class="reason-card">  
      <div class="reason-icon">😂</div>  
      <div class="reason-title">Your laugh</div>  
      <div class="reason-text">It's the most beautiful sound I know. It makes everything lighter.</div>  
    </div>  
    <div class="reason-card">  
      <div class="reason-icon">💬</div>  
      <div class="reason-title">The way you talk</div>  
      <div class="reason-text">I could listen to you for hours and never get enough. Every word matters.</div>  
    </div>  
    <div class="reason-card">  
      <div class="reason-icon">🌙</div>  
      <div class="reason-title">Goodnight texts</div>  
      <div class="reason-text">Falling asleep knowing you thought of me is the coziest feeling.</div>  
    </div>  
    <div class="reason-card">  
      <div class="reason-icon">🧠</div>  
      <div class="reason-title">Your mind</div>  
      <div class="reason-text">The way you think, your ideas, your perspective — endlessly fascinating.</div>  
    </div>  
    <div class="reason-card">  
      <div class="reason-icon">🤗</div>  
      <div class="reason-title">Your kindness</div>  
      <div class="reason-text">You have the warmest heart. It radiates through everything you do.</div>  
    </div>  
    <div class="reason-card">  
      <div class="reason-icon">✨</div>  
      <div class="reason-title">Just you</div>  
      <div class="reason-text">All of you, exactly as you are. I wouldn't change a single thing.</div>  
    </div>  
  </div>  
</section>  
  
<!-- Promise section -->  
  
<section class="promise-section">  
  <span class="big-heart">❤️</span>  
  <h2 class="promise-title" style="margin-top:24px;">I promise you this</h2>  
  <p class="promise-text">  
    I will choose you, every single day. I will be patient through the distance,  
    grateful for every moment, and loyal with every heartbeat. This love is not temporary —  
    it is the realest, truest thing I have. And one day soon, we won't need to say goodbye  
    at the end of a call. Until then, I am right here. Always.  
  </p>  
  <div class="flower-row" style="color:white;opacity:0.6;">  
    <span>🌸</span><span>🌷</span><span>🌹</span><span>🌺</span>  
    <span>💐</span><span>🌸</span><span>🌷</span>  
  </div>  
</section>  
  
<footer>  
  Made with every bit of love I have 🌹 Just for you 💕  
</footer>  
  
<script>  
  // Generate floating petals  
  const petalsContainer = document.getElementById('petals');  
  const petalEmojis = ['🌸', '🌺', '🌷', '💕', '🌹', '✨', '💖'];  
  
  for (let i = 0; i < 28; i++) {  
    const petal = document.createElement('div');  
    petal.className = 'petal';  
    petal.textContent = petalEmojis[Math.floor(Math.random() * petalEmojis.length)];  
    petal.style.left = Math.random() * 100 + 'vw';  
    petal.style.fontSize = (Math.random() * 1.2 + 0.8) + 'rem';  
    petal.style.animationDuration = (Math.random() * 8 + 7) + 's';  
    petal.style.animationDelay = (Math.random() * 10) + 's';  
    petal.style.opacity = Math.random() * 0.5 + 0.3;  
    petalsContainer.appendChild(petal);  
  }  
  
  // Sparkle on click  
  const sparkleEmojis = ['💕', '✨', '🌸', '💖', '🌷', '⭐'];  
  document.addEventListener('click', (e) => {  
    for (let i = 0; i < 5; i++) {  
      const sparkle = document.createElement('div');  
      sparkle.className = 'sparkle';  
      sparkle.textContent = sparkleEmojis[Math.floor(Math.random() * sparkleEmojis.length)];  
      sparkle.style.left = (e.clientX + (Math.random() - 0.5) * 60) + 'px';  
      sparkle.style.top  = (e.clientY + (Math.random() - 0.5) * 60) + 'px';  
      sparkle.style.animationDelay = (Math.random() * 0.3) + 's';  
      document.body.appendChild(sparkle);  
      setTimeout(() => sparkle.remove(), 1200);  
    }  
  });  
</script>  
  
</body>  
</html>  
