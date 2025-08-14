<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Happy Birthday Arpita — A Love Note</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
<style>
  :root{--accent:#ff6fb5;--accent2:#ffd36b;--soft:#ffd7ea;--nature-green:#a9cba4;--sakura-pink:#f7cac9;--glow-yellow:#ffe066;--star-white:#fff5e1;--anime-blue:#87ceeb;--anime-pink:#ffc0cb}
  *{box-sizing:border-box}
  html,body{height:100%;margin:0;background:linear-gradient(180deg, #1a2a44, #0d1b2a);font-family:Inter,system-ui,-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,'Helvetica Neue',Arial;color:#fff;overflow-x:hidden}
  .wrap{min-height:100vh;display:flex;align-items:center;justify-content:center;padding:20px 10px}
  .card{width:100%;max-width:1100px;border-radius:14px;position:relative;overflow:hidden;padding:20px;border:1px solid rgba(255,255,255,0.03);background:linear-gradient(180deg, rgba(26,42,68,0.8), rgba(13,27,42,0.6));box-shadow:0 20px 60px rgba(0,0,0,0.8);will-change:transform}
  .intro{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;background:linear-gradient(180deg, rgba(0,0,0,0.85), rgba(0,0,0,0.6));z-index:90;transition:opacity .5s ease-out,transform .5s ease-out;will-change:opacity, transform}
  .intro.hidden{opacity:0;pointer-events:none;transform:translateY(-20px)}
  .intro h1{font-family:'Playfair Display';font-size:clamp(28px, 8vw, 44px);letter-spacing:1px;margin:0 0 8px 0;color:var(--accent);text-shadow:0 4px 20px rgba(255,111,181,0.08)}
  .intro p{color:#d8bfd8;font-size:clamp(12px, 3vw, 16px);margin:0 0 15px 0}
  .tap{display:flex;gap:10px;align-items:center}
  .cta{background:linear-gradient(90deg,var(--accent),var(--accent2));border:none;padding:12px 18px;border-radius:999px;font-weight:700;cursor:pointer;color:#111;font-size:clamp(14px, 3vw, 16px);box-shadow:0 15px 40px rgba(255,111,181,0.12);transition:transform .2s ease-out;will-change:transform}
  .cta:hover{transform:scale(1.05)}
  .head{display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap}
  .brand{display:flex;gap:10px;align-items:center}
  .logo{width:clamp(40px, 6vw, 64px);height:clamp(40px, 6vw, 64px);border-radius:10px;background:linear-gradient(135deg,var(--accent),#ffb3d1);display:flex;align-items:center;justify-content:center;font-family:'Playfair Display';color:#111;font-weight:700;font-size:clamp(18px, 4vw, 28px)}
  .title h2{margin:0;font-family:'Playfair Display';font-size:clamp(16px, 3vw, 20px)}
  .title p{margin:4px 0 0 0;color:#c9a7c6;font-size:clamp(10px, 2vw, 13px)}
  .controls{display:flex;align-items:center;gap:10px;flex-wrap:wrap}
  .play-pill{display:flex;align-items:center;gap:8px;background:transparent;border:1px solid rgba(255,255,255,0.06);padding:8px 12px;border-radius:999px;cursor:pointer;color:var(--soft);backdrop-filter:blur(6px);transition:transform .2s ease-out}
  .play-pill:hover{transform:scale(1.05)}
  .play-pill .icon{width:10px;height:10px;border-radius:2px;background:var(--accent)}
  .song-links a{display:inline-block;padding:6px 10px;margin:4px 0;border-radius:6px;background:rgba(255,111,181,0.1);transition:background .2s ease-out, transform .2s ease-out}
  .song-links a:hover{background:rgba(255,111,181,0.3);transform:scale(1.05)}
  .content{display:grid;grid-template-columns:1fr;gap:20px;align-items:start;margin-top:15px}
  .photo-area{position:relative;display:flex;flex-direction:column;align-items:center;gap:15px;padding:10px}
  .center-wrap{width:100%;max-width:360px;height:clamp(200px, 50vw, 360px);border-radius:12px;overflow:hidden;display:flex;align-items:center;justify-content:center;border:1px solid rgba(255,255,255,0.04);box-shadow:0 30px 90px rgba(0,0,0,0.7);background:linear-gradient(180deg,rgba(255,255,255,0.02),rgba(255,255,255,0.01));position:relative;will-change:transform}
  .center-photo{width:100%;height:100%;object-fit:cover;display:block;transform:translateZ(0);transition:transform .4s ease-out;will-change:transform;z-index:2}
  .center-wrap:hover .center-photo{transform:scale(1.025)}
  .nature-bg{position:absolute;inset:0;pointer-events:none;opacity:0.8;background:linear-gradient(to bottom, var(--nature-green) 0%, #2f4f4f 50%, #1a2a44 100%), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><path d="M10 90 Q30 70, 50 90 T70 70 Q90 50, 70 30 T50 10 Q30 30, 10 10 T30 30 Q10 50, 30 70 T10 90" fill="none" stroke="%23a9cba4" stroke-width="1"/><path d="M20 80 Q40 60, 60 80 T80 60 Q100 40, 80 20 T60 0" fill="none" stroke="%23556677" stroke-width="1.5" opacity="0.7"/></svg>');z-index:1;animation:sway 10s infinite ease-in-out;will-change:transform}
  .firefly{position:absolute;width:6px;height:6px;background:var(--glow-yellow);border-radius:50%;opacity:0.7;animation:blink 2s infinite, float 6s infinite ease-in-out;z-index:3;will-change:opacity, transform}
  .bird{position:absolute;width:15px;height:10px;background:linear-gradient(45deg, #a9cba4, #ffe066);border-radius:50%;opacity:0.8;animation:fly 12s infinite ease-in-out;will-change:transform}
  .flower{position:absolute;width:12px;height:12px;background:var(--sakura-pink);border-radius:50%;opacity:0;animation:bloom 6s infinite ease-out;will-change:opacity, transform}
  .river-flow{position:absolute;bottom:0;left:0;width:100%;height:20px;background:linear-gradient(to right, transparent, #87ceeb, transparent);opacity:0.4;animation:flow 6s infinite linear;will-change:transform}
  .mountain{position:absolute;bottom:0;width:100%;height:30px;background:repeating-linear-gradient(to bottom, #5c4033, #5c4033 2px, transparent 2px, transparent 4px);z-index:1}
  @keyframes sway{0%{transform:translateX(0) rotate(0deg)}50%{transform:translateX(6px) rotate(0.5deg)}100%{transform:translateX(0) rotate(0deg)}}
  @keyframes blink{0%{opacity:0.7}50%{opacity:0.2}100%{opacity:0.7}}
  @keyframes float{0%{transform:translateY(0)}50%{transform:translateY(-10px)}100%{transform:translateY(0)}}
  @keyframes fly{0%{transform:translateX(-100%) rotate(0deg)}100%{transform:translateX(100%) rotate(360deg)}}
  @keyframes bloom{0%{opacity:0;transform:scale(0)}50%{opacity:1;transform:scale(1)}100%{opacity:0;transform:scale(0)}}
  @keyframes flow{0%{transform:translateX(0)}100%{transform:translateX(-100%)}}
  .glow{position:absolute;pointer-events:none;left:50%;top:50%;transform:translate(-50%,-50%);width:720px;height:720px;border-radius:50%;filter:blur(48px);opacity:0.05;background:radial-gradient(circle at center, rgba(255,111,181,0.4), transparent 40%);z-index:0;will-change:opacity}
  .outer-glow{position:absolute;inset:0;pointer-events:none;background:radial-gradient(circle at center, rgba(255,215,234,0.03), transparent 60%);z-index:-1;will-change:opacity}
  .poem{width:100%;max-width:680px;margin-top:10px;display:flex;flex-direction:column;gap:8px;align-items:center}
  .poem .line{font-size:clamp(14px, 3vw, 18px);color:#e6d6ea;opacity:0;transform:translateY(12px);transition:all .5s ease-out;will-change:opacity, transform;max-width:780px;text-align:center}
  .poem .line.show{opacity:1;transform:translateY(0)}
  .right{position:relative;width:100%;max-width:360px}
  .panel{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(0,0,0,0.05));padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.03)}
  .panel img{width:100%;height:clamp(150px, 40vw, 220px);object-fit:cover;border-radius:8px}
  .count{margin-top:10px;text-align:center;color:var(--soft);font-weight:600;font-size:clamp(12px, 2.5vw, 16px)}
  .thumbs{display:flex;gap:8px;margin-top:10px;flex-wrap:wrap;position:relative}
  .thumbs::after{content:"";position:absolute;bottom:-8px;left:0;width:100%;height:15px;background:linear-gradient(to bottom, transparent, var(--nature-green) 70%);opacity:0.2;border-radius:0 0 10px 10px}
  .thumbs img{width:clamp(50px, 12vw, 74px);height:clamp(50px, 12vw, 74px);border-radius:8px;object-fit:cover;cursor:pointer;border:2px solid transparent;opacity:0.9;transition:transform .2s ease-out}
  .thumbs img.active{border-color:var(--accent);transform:scale(1.03);opacity:1}
  .thumbs img:hover{transform:scale(1.05)}
  .confetti{position:absolute;inset:0;pointer-events:none;z-index:70}
  .sakura{position:absolute;inset:0;pointer-events:none;overflow:hidden;z-index:60}
  .sakura-petal{width:12px;height:12px;background:var(--sakura-pink);position:absolute;border-radius:50%;animation:fall 10s infinite ease-out;will-change:transform}
  .star{position:absolute;width:4px;height:4px;background:var(--star-white);border-radius:50%;opacity:0;animation:twinkle 3s infinite;will-change:opacity}
  .love-note{position:absolute;width:60px;height:40px;background:linear-gradient(45deg, var(--accent), var(--soft));border-radius:6px;opacity:0;animation:noteFloat 8s infinite ease-in-out;will-change:transform, opacity;font-size:10px;color:#111;text-align:center;padding-top:5px;pointer-events:none}
  .love-note::after{content:"I ♥ You";display:block}
  .anime-couple{position:absolute;bottom:40px;left:50%;transform:translateX(-50%);width:clamp(50px, 12vw, 70px);height:clamp(60px, 15vw, 80px);display:flex;gap:8px;align-items:center;pointer-events:none;z-index:5;animation:sway-couple 5s infinite ease-in-out;will-change:transform}
  .anime-char{width:clamp(20px, 5vw, 30px);height:clamp(30px, 8vw, 40px);background:linear-gradient(45deg, var(--anime-blue), var(--anime-pink));border:2px solid #fff;border-radius:50% 50% 40% 40%;position:relative;overflow:hidden}
  .anime-char::before{content:"";position:absolute;top:10%;left:20%;width:60%;height:60%;background:radial-gradient(circle at 30% 30%, #000, #000 20%, transparent);border-radius:50%} /* Eyes */
  .anime-char::after{content:"";position:absolute;bottom:10%;left:50%;transform:translateX(-50%);width:40%;height:20%;background:#ff69b4;border-radius:50%} /* Mouth */
  .anime-char:nth-child(1){transform:scaleX(-1)}
  .anime-char:nth-child(1)::before{left:20%;} /* Adjust eye for flipped character */
  @keyframes fall{0%{opacity:0;transform:translateY(-20vh) rotate(0deg)}20%{opacity:0.8}100%{opacity:0;transform:translateY(120vh) rotate(720deg)}}
  @keyframes twinkle{0%{opacity:0}50%{opacity:0.6}100%{opacity:0}}
  @keyframes noteFloat{0%{opacity:0;transform:translate(-50%, -20vh) rotate(0deg)}20%{opacity:0.9}80%{opacity:0.9}100%{opacity:0;transform:translate(-50%, 120vh) rotate(360deg)}}
  @keyframes glow{0%{box-shadow:0 0 3px var(--glow-yellow)}50%{box-shadow:0 0 8px var(--glow-yellow)}100%{box-shadow:0 0 3px var(--glow-yellow)}}
  @keyframes sway-couple{0%{transform:translateX(-50%) translateY(0)}50%{transform:translateX(-50%) translateY(-8px)}100%{transform:translateX(-50%) translateY(0)}}
  @media (min-width: 768px) {
    .content{grid-template-columns:1fr 360px}
    .center-wrap{max-width:360px;height:360px}
    .panel img{height:220px}
    .thumbs img{width:74px;height:74px}
    .anime-couple{width:70px;height:80px}
    .anime-char{width:30px;height:40px}
  }
  @media (max-width: 480px) {
    .center-wrap{height:clamp(180px, 50vw, 260px)}
    .panel img{height:clamp(120px, 30vw, 180px)}
    .thumbs img{width:clamp(40px, 10vw, 60px);height:clamp(40px, 10vw, 60px)}
    .anime-couple{width:clamp(40px, 10vw, 60px);height:clamp(50px, 12vw, 70px)}
    .anime-char{width:clamp(15px, 4vw, 25px);height:clamp(25px, 6vw, 35px)}
  }
</style>
</head>
<body>
<div class="wrap">
  <div class="card" id="card">
    <div class="intro" id="intro">
      <h1>Happy Birthday Arpita</h1>
      <p>A small world I made, so your smile has a home today.</p>
      <div class="tap"><button class="cta" id="revealBtn">Open Your Surprise</button></div>
    </div>
    <div class="glow" aria-hidden="true"></div>
    <div class="outer-glow" aria-hidden="true"></div>
    <div class="head">
      <div class="brand">
        <div class="logo">A</div>
        <div class="title"><h2>Forever Arpita</h2><p>15 August • A love-letter turned page</p></div>
      </div>
      <div class="controls">
        <button class="play-pill" id="playBtn"><div class="icon"></div><div id="playLabel">Play Song</div></button>
        <div style="color:#9f6a98;font-size:clamp(10px, 2vw, 13px)">From Harshit</div>
        <div class="song-links">
          <p style="color:#ffd7ea;font-size:clamp(12px, 2.5vw, 14px);margin:8px 0 4px 0;">More Songs for You:</p>
          <ul style="list-style:none;padding:0;margin:0;">
            <li><a href="https://youtu.be/wJ-rw35JEGI?si=1MkdWowG3c7AxYu1" target="_blank" style="color:#ff6fb5;text-decoration:none;">Song 1: Lo-Fi Song 1</a></li>
            <li><a href="https://youtu.be/zF6AsmQIPyc?si=KWWH5bQRSTpKl-_O" target="_blank" style="color:#ff6fb5;text-decoration:none;">Song 2: Lo-Fi Song 2</a></li>
            <li><a href="https://youtu.be/NH2EX1fbFwU?si=7yLXkdp2txjTk2XP" target="_blank" style="color:#ff6fb5;text-decoration:none;">Song 3: Lo-Fi Song 3</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="content">
      <div class="photo-area">
        <div class="center-wrap">
          <img id="centerPhoto" class="center-photo" src="/photo5.jpg" alt="Center">
          <div class="nature-bg"></div>
          <div class="mountain"></div>
          <div class="firefly" style="left:10%;top:20%"></div>
          <div class="firefly" style="left:70%;top:50%"></div>
          <div class="firefly" style="left:30%;top:80%"></div>
          <div class="bird" style="left:20%;top:10%"></div>
          <div class="bird" style="left:80%;top:30%"></div>
          <div class="flower" style="left:15%;top:70%"></div>
          <div class="flower" style="left:85%;top:80%"></div>
          <div class="river-flow"></div>
          <div class="anime-couple">
            <div class="anime-char"></div>
            <div class="anime-char"></div>
          </div>
        </div>
        <div class="poem" id="poem">
          <div class="line">Tere bina, meri subah adhoori lagti hai — jaise sur bina geet.</div>
          <div class="line">Teri muskaan mere din ka sur hai, aur teri hansi mere raaton ki roshni.</div>
          <div class="line">Pal pal tu mere saath hai — meri wadiyon ka geet, meri hawa ka ehsaas.</div>
          <div class="line">Aaj main dua karta hun: tere sapne phoolon ke jaise khilen, aur har leaf tujhe pyaar ka paigham laaye.</div>
          <div class="line">Meri zindagi, meri shuruaat, meri aakhri khushi — hamesha tera saath chahiye.</div>
        </div>
      </div>
      <div class="right">
        <div class="panel">
          <img id="panelPhoto" src="/photo2.jpg" alt="panel">
          <div class="count" id="countdown">⏳ Loading countdown...</div>
          <div class="thumbs" id="thumbs">
            <img src="/photo1.jpg" data-src="/photo1.jpg" class="active">
            <img src="/photo2.jpg" data-src="/photo2.jpg">
            <img src="/photo3.jpg" data-src="/photo3.jpg">
            <img src="/photo4.jpg" data-src="/photo4.jpg">
          </div>
        </div>
        <div class="foot">Keep this surprise private • Click any thumbnail to change the main photo</div>
      </div>
    </div>
    <div class="confetti" id="confetti"></div>
    <div class="sakura" id="sakura"></div>
  </div>
</div>

<audio id="bgAudio" preload="auto" muted>
  <source src="/palpal_lofi_reverb.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

<script>
const countdownEl = document.getElementById('countdown');
const target = new Date('August 15, 2025 00:00:00').getTime();
function updateCountdown(){
  const now = Date.now();
  const dist = target - now;
  if(dist<=0){countdownEl.innerHTML = "🎂 It's her Birthday! 🎂";clearInterval(countInterval);return}
  const d = Math.floor(dist/(1000*60*60*24));
  const h = Math.floor((dist%(1000*60*60*24))/(1000*60*60));
  const m = Math.floor((dist%(1000*60*60))/(1000*60));
  const s = Math.floor((dist%(1000*60))/1000);
  countdownEl.innerHTML = `⏳ ${d}d ${h}h ${m}m ${s}s left`;
}
const countInterval = setInterval(updateCountdown,1000); updateCountdown();

const lines = document.querySelectorAll('.poem .line');
lines.forEach((el,i)=> setTimeout(()=> el.classList.add('show'), 600 + i*500));

const thumbs = document.querySelectorAll('#thumbs img');
const center = document.getElementById('centerPhoto');
const panel = document.getElementById('panelPhoto');
thumbs.forEach(t=> t.addEventListener('click', ()=>{
  thumbs.forEach(x=> x.classList.remove('active'));
  t.classList.add('active');
  const src = t.getAttribute('data-src');
  center.src = src; panel.src = src;
}));

function spawnParticle(){
  const el = document.createElement('div'); el.className='spark';
  const size = Math.random()*8 + 6; el.style.width = size+'px'; el.style.height = size+'px';
  el.style.left = Math.random()*100 + '%'; el.style.top = Math.random()*100 + '%';
  el.style.background = ['rgba(169,203,164,0.9)','rgba(255,215,130,0.9)','rgba(199,249,255,0.9)'][Math.floor(Math.random()*3)];
  el.style.opacity = 0.8; el.style.filter = 'blur(6px)'; document.getElementById('card').appendChild(el);
  setTimeout(()=> el.remove(),3000);
}
setInterval(spawnParticle,400);

const intro = document.getElementById('intro');
const revealBtn = document.getElementById('revealBtn');
const audio = document.getElementById('bgAudio');
const playBtn = document.getElementById('playBtn');
let playing=false;

revealBtn.addEventListener('click', () => {
  intro.classList.add('hidden');
  burstConfetti();
  startHearts();
  startSakura();
  startStars();
  startLoveNotes();
  startBirds();
  startFlowers();
  startRiverFlow();
  startCoupleAnimation();
  audio.currentTime = 0;
  audio.muted = false;
});

playBtn.addEventListener('click', async () => {
  if (!playing) {
    try {
      await audio.play();
      playing = true;
      playBtn.querySelector('#playLabel').innerText = 'Pause Song';
    } catch (e) {
      console.error('Audio play failed:', e);
      playBtn.querySelector('#playLabel').innerText = 'Audio Error';
      alert('Failed to play audio. Please ensure the audio file is uploaded correctly to Netlify.');
    }
  } else {
    audio.pause();
    playing = false;
    playBtn.querySelector('#playLabel').innerText = 'Play Song';
  }
});

function burstConfetti(){
  const container = document.getElementById('confetti');
  const colors = ['#ff6fb5','#ffd36b','#c7f9ff','#a0ffb8'];
  for(let i=0;i<30;i++){
    const el = document.createElement('div'); el.style.position='absolute'; el.style.width='8px'; el.style.height='12px'; el.style.left = Math.random()*100 + '%'; el.style.top = '40%'; el.style.background = colors[Math.floor(Math.random()*colors.length)]; el.style.opacity=0.9; el.style.transform = `rotate(${Math.random()*360}deg)`; container.appendChild(el);
    const dx = (Math.random()-0.5)*700; const dy = - (Math.random()*700+150);
    el.animate([{transform:'translate(0,0) rotate(0deg)', opacity:1},{transform:`translate(${dx}px,${dy}px) rotate(${Math.random()*540}deg)`, opacity:0}],{duration:1000+Math.random()*700,easing:'ease-out'});
    setTimeout(()=>el.remove(),1700);
  }
}

let heartInt;
function startHearts(){
  heartInt = setInterval(()=>{
    const h = document.createElement('div'); h.textContent='❤'; h.style.position='absolute'; h.style.left = Math.random()*100 + '%'; h.style.fontSize = (Math.random()*18+10)+'px'; h.style.top = '-5%'; h.style.opacity=0.9; h.style.color = ['#ff6fb5','#ffb3d1','#ffd36b'][Math.floor(Math.random()*3)]; h.style.filter='drop-shadow(0 4px 12px rgba(0,0,0,0.5))'; document.getElementById('card').appendChild(h);
    const dur = 4000 + Math.random()*3000; h.animate([{transform:'translateY(0) rotate(0deg)', opacity:1},{transform:`translateY(${window.innerHeight*0.8}px) rotate(${Math.random()*180}deg)`, opacity:0}],{duration:dur,easing:'ease-out'});
    setTimeout(()=>h.remove(),dur+100);
  },250);
}

let sakuraInt;
function sta# Birthday-special-