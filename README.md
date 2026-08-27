<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<meta name="theme-color" content="#17050b">
<title>Для Багратика ❤️</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;500;600&display=swap');

:root{
  --wine:#551225;--wine2:#751d35;--deep:#17050b;
  --van:#fff2d3;--gold:#d8b66d;
  --vh:100vh;
}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
html,body{margin:0;width:100%;height:100%;overflow:hidden;background:var(--deep)}
body{
  color:var(--van);font-family:'Cormorant Garamond',serif;
  overscroll-behavior:none;-webkit-text-size-adjust:100%;
}
button{font:inherit}
.slides{
  position:fixed;inset:0;width:100%;height:100%;
  overflow:hidden;background:
  radial-gradient(circle at 50% 20%,#79213a45,transparent 42%),var(--deep);
}
.slides:before{
  content:"";position:absolute;inset:0;pointer-events:none;opacity:.16;
  background-image:radial-gradient(#fff 1px,transparent 1px);
  background-size:85px 85px;animation:drift 24s linear infinite;
}
@keyframes drift{to{transform:translateY(85px)}}

.slide{
  position:absolute;inset:0;width:100%;height:100%;
  min-height:100%;display:flex;align-items:center;justify-content:center;
  padding:calc(22px + env(safe-area-inset-top)) 
           calc(18px + env(safe-area-inset-right))
           calc(22px + env(safe-area-inset-bottom))
           calc(18px + env(safe-area-inset-left));
  opacity:0;visibility:hidden;pointer-events:none;
  transform:translate3d(0,0,0) scale(.985);
  transition:opacity .55s ease,transform .55s ease,visibility .55s;
  overflow:hidden;
}
.slide.active{opacity:1;visibility:visible;pointer-events:auto;transform:scale(1)}
.content{width:min(900px,100%);height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center}
.eyebrow{font-size:12px;letter-spacing:4px;text-transform:uppercase;color:var(--gold);margin-bottom:22px}
h1,h2,.subtitle,.btn,.lead,.game-text,.score,.small,.letter{font-family:'Cormorant Garamond',serif}
h1{font-weight:400;font-size:clamp(70px,18vw,165px);line-height:.72;margin:0}
h2{font-weight:400;font-size:clamp(46px,10vw,88px);line-height:.9;margin:0 0 22px}
.subtitle{font-size:clamp(29px,6vw,52px);font-weight:300;color:#f2d8a7;margin:28px 0}
.lead{font-size:clamp(21px,4vw,26px);line-height:1.45;color:#f1dfbdc9;max-width:650px;margin:0 auto 30px}
.btn{
  border:1px solid #d8b66d99;background:#64182d;color:var(--van);
  padding:12px 28px;border-radius:50px;font-size:21px;line-height:1;
  cursor:pointer;touch-action:manipulation;user-select:none;
}
.btn:active{transform:scale(.97);background:#81233c}
.small{font-size:17px;color:#d8b66daa;margin-top:12px}

.gamebox{
  width:min(720px,100%);padding:10px;
  border:1px solid #d8b66d35;border-radius:24px;background:#250812cc;
  box-shadow:0 20px 70px #0009;
}
#gameCanvas{
  display:block;width:100%;height:auto;aspect-ratio:3/2;
  background:#260914;border-radius:16px;border:1px solid #d8b66d35;
  touch-action:none;
}
.score{font-size:23px;color:var(--gold);margin:8px}
.game-text{font-size:19px;color:#f1dfbdcc;margin:3px 0 9px}
.controls{display:grid;grid-template-columns:48px 48px 48px;gap:6px;justify-content:center}
.controls button{
  width:48px;height:42px;border:1px solid #d8b66d55;border-radius:10px;
  background:#64182d99;color:var(--van);font-size:20px;touch-action:none;
}
.controls button:nth-child(1){grid-column:2}
.controls button:nth-child(2){grid-column:1}.controls button:nth-child(3){grid-column:2}.controls button:nth-child(4){grid-column:3}

.letter-wrap{
  width:min(820px,100%);height:min(78vh,780px);
  display:flex;flex-direction:column;
}
.letter{
  flex:1;min-height:0;overflow-y:auto;overflow-x:hidden;
  -webkit-overflow-scrolling:touch;overscroll-behavior:contain;
  touch-action:pan-y;text-align:left;padding:25px 22px;
  scrollbar-width:none;
}
.letter::-webkit-scrollbar{display:none}
.letter h2{text-align:center}
.letter p{font-size:clamp(21px,4vw,29px);line-height:1.45;margin:0 0 21px}
.signature{text-align:right;color:var(--gold);font-size:31px!important}

.final-heart{font-size:68px;animation:pulse 1.8s infinite}
@keyframes pulse{50%{transform:scale(1.1)}}
.nav{
 position:fixed;right:12px;top:50%;transform:translateY(-50%);z-index:20;
 display:flex;flex-direction:column;gap:9px;
}
.dot{
 width:7px;height:7px;border-radius:50%;border:1px solid #d8b66d99;
 background:transparent;cursor:pointer;padding:0;touch-action:manipulation;
}
.dot.active{background:var(--gold);box-shadow:0 0 12px #d8b66d88}

@media(max-width:600px){
 .slide{padding-top:calc(18px + env(safe-area-inset-top));padding-bottom:calc(18px + env(safe-area-inset-bottom))}
 .eyebrow{letter-spacing:3px;font-size:11px}
 .gamebox{padding:8px}
 .letter-wrap{height:min(76vh,720px)}
 .letter{padding:18px 10px}
 .letter p{font-size:22px;line-height:1.42}
 .letter h2{font-size:48px}
 .nav{right:7px}
}
@media(max-height:700px){
 h1{font-size:clamp(65px,17vw,110px)}
 h2{font-size:clamp(42px,9vw,70px)}
 .subtitle{font-size:31px;margin:18px 0}
 .lead{font-size:19px;margin-bottom:18px}
 .eyebrow{margin-bottom:14px}
 .letter-wrap{height:72vh}
}
</style>
</head>
<body>

<main class="slides" id="slides">

<section class="slide active">
 <div class="content">
  <div class="eyebrow">маленький подарок</div>
  <h1>Багратик</h1>
  <div class="subtitle">с днём рождения,<br>мой любимый ❤️</div>
  <button class="btn" type="button" onclick="go(1)">Дальше</button>
 </div>
</section>

<section class="slide">
 <div class="content">
  <div class="eyebrow">только для тебя</div>
  <h2>У меня есть<br>кое-что для тебя</h2>
  <p class="lead">Но прежде чем открыть подарок, тебя ждёт маленькое приключение.</p>
  <button class="btn" type="button" onclick="go(2)">Начать приключение ✨</button>
 </div>
</section>

<section class="slide">
 <div class="content">
  <div class="eyebrow">мини-игра</div>
  <h2>Поймай всё<br>хорошее</h2>
  <div class="gamebox">
   <canvas id="gameCanvas" width="900" height="600"></canvas>
   <div class="score">Собрано: <span id="score">0</span> / 12</div>
   <div class="game-text">Собирай сердечки и звёздочки ❤️</div>
   <div class="controls">
    <button type="button" data-key="ArrowUp">↑</button>
    <button type="button" data-key="ArrowLeft">←</button>
    <button type="button" data-key="ArrowDown">↓</button>
    <button type="button" data-key="ArrowRight">→</button>
   </div>
  </div>
  <div class="small">стрелки / WASD · на iPhone — кнопки</div>
 </div>
</section>

<section class="slide">
 <div class="content">
  <div class="eyebrow">победа</div>
  <div class="final-heart">❤️</div>
  <h2>Ты справился</h2>
  <p class="lead">Ну всё. Теперь можно открыть настоящий подарок.</p>
  <button class="btn" type="button" onclick="go(4)">Открыть письмо</button>
 </div>
</section>

<section class="slide" id="letterSlide">
 <div class="letter-wrap">
  <div class="letter" id="letter">
   <div class="eyebrow">для тебя</div>
   <h2>Мой любимый Багратик,<br>с днём рождения тебя! ❤️</h2>
   <p>Я хочу пожелать тебе самого главного — чтобы ты был счастлив. Чтобы рядом с тобой всегда были люди, которые любят тебя искренне, поддерживают и ценят таким, какой ты есть. Пусть у тебя получается всё, за что ты берёшься, пусть появляются новые возможности, а мечты постепенно становятся реальностью.</p>
   <p>Я очень рад, что однажды именно ты появился в моей жизни. За всё время, что мы вместе, ты стал для меня невероятно близким и важным человеком. Я люблю наши разговоры, наши моменты, твои слова, твои привычки и даже те мелочи, которые иногда меня бесят. Ты — это человек, которого мне хочется обнимать, целовать и просто иметь рядом.</p>
   <p>Спасибо тебе за то, что ты есть. За твою любовь, за тепло, за моменты, которые мы уже успели прожить вместе. Я надеюсь, что впереди у нас ещё очень много всего — смешного, красивого, безумного и только нашего.</p>
   <p>Пожалуйста, никогда не забывай, насколько ты особенный для меня. Я очень тебя люблю, Багратик. С твоим днём, мой родной. Будь счастлив. ❤️</p>
   <p class="signature">Твой человек. ❤️</p>
  </div>
 </div>
</section>

<section class="slide">
 <div class="content">
  <div class="final-heart">❤️</div>
  <div class="eyebrow">и напоследок</div>
  <h2>Будь счастлив,<br>мой родной.</h2>
  <p class="lead">И никогда не забывай, что ты особенный.</p>
  <div class="subtitle" style="font-size:38px">Я очень тебя люблю.</div>
 </div>
</section>

<nav class="nav" aria-label="Навигация">
 <button class="dot active" aria-label="Слайд 1" onclick="go(0)"></button>
 <button class="dot" aria-label="Слайд 2" onclick="go(1)"></button>
 <button class="dot" aria-label="Слайд 3" onclick="go(2)"></button>
 <button class="dot" aria-label="Слайд 4" onclick="go(3)"></button>
 <button class="dot" aria-label="Слайд 5" onclick="go(4)"></button>
 <button class="dot" aria-label="Слайд 6" onclick="go(5)"></button>
</nav>
</main>

<script>
/* ---------- SLIDES: iPhone-safe horizontal swipes ---------- */
const slides=[...document.querySelectorAll('.slide')];
const dots=[...document.querySelectorAll('.dot')];
const letter=document.getElementById('letter');
let current=0;
let sx=0,sy=0,swipeTarget=null;

function go(n){
  if(n<0||n>=slides.length||n===current)return;
  slides[current].classList.remove('active');
  dots[current].classList.remove('active');
  current=n;
  slides[current].classList.add('active');
  dots[current].classList.add('active');
  if(current===4) letter.scrollTop=0;
}

document.addEventListener('touchstart',e=>{
  const t=e.changedTouches[0];
  sx=t.clientX; sy=t.clientY;
  swipeTarget=e.target;
},{passive:true});

document.addEventListener('touchend',e=>{
  if(!swipeTarget)return;
  if(swipeTarget.closest('#letter'))return;
  const t=e.changedTouches[0];
  const dx=t.clientX-sx,dy=t.clientY-sy;
  if(Math.abs(dx)>65 && Math.abs(dx)>Math.abs(dy)){
    go(current+(dx<0?1:-1));
  }
},{passive:true});

document.addEventListener('keydown',e=>{
  if(['ArrowRight','ArrowDown'].includes(e.key)){e.preventDefault();go(current+1)}
  if(['ArrowLeft','ArrowUp'].includes(e.key)){e.preventDefault();go(current-1)}
});

/* ---------- GAME: touch controls, no keyboard required ---------- */
const c=document.getElementById('gameCanvas'),ctx=c.getContext('2d');
let p={x:450,y:300,r:22,s:6},keys={},score=0,items=[],won=false;

function spawn(){
  items.push({
    x:45+Math.random()*810,
    y:45+Math.random()*510,
    r:Math.random()>0.4?16:12,
    type:Math.random()>0.4?'heart':'star'
  });
}
for(let i=0;i<8;i++)spawn();

function heart(x,y,s){
 ctx.save();ctx.translate(x,y);ctx.beginPath();
 ctx.moveTo(0,s*.85);
 ctx.bezierCurveTo(-s*1.25,-s*.05,-s*.7,-s,-s*.38,-s*.58);
 ctx.bezierCurveTo(-s*.1,-s,0,-s*.55,0,-s*.35);
 ctx.bezierCurveTo(0,-s*.55,s*.1,-s,s*.38,-s*.58);
 ctx.bezierCurveTo(s*.7,-s,s*1.25,-s*.05,0,s*.85);
 ctx.closePath();ctx.fill();ctx.restore();
}
function star(x,y,r){
 ctx.save();ctx.translate(x,y);ctx.beginPath();
 for(let i=0;i<10;i++){
   const a=-Math.PI/2+i*Math.PI/5,rr=i%2?r:r*.42;
   ctx.lineTo(Math.cos(a)*rr,Math.sin(a)*rr);
 }
 ctx.closePath();ctx.fill();ctx.restore();
}
function draw(){
 ctx.clearRect(0,0,900,600);
 ctx.fillStyle='#260914';ctx.fillRect(0,0,900,600);
 ctx.strokeStyle='#d8b66d12';
 for(let x=0;x<900;x+=60){ctx.beginPath();ctx.moveTo(x,0);ctx.lineTo(x,600);ctx.stroke()}
 for(let y=0;y<600;y+=60){ctx.beginPath();ctx.moveTo(0,y);ctx.lineTo(900,y);ctx.stroke()}
 items.forEach((it,i)=>{
   ctx.globalAlpha=.7+.3*Math.sin(Date.now()/220+i);
   ctx.fillStyle=it.type==='heart'?'#dc91a2':'#d8b66d';
   it.type==='heart'?heart(it.x,it.y,it.r):star(it.x,it.y,it.r);
 });
 ctx.globalAlpha=1;ctx.fillStyle='#fff2d3';heart(p.x,p.y,p.r);
}
function update(){
 let dx=0,dy=0;
 if(keys.ArrowLeft||keys.a)dx--;
 if(keys.ArrowRight||keys.d)dx++;
 if(keys.ArrowUp||keys.w)dy--;
 if(keys.ArrowDown||keys.s)dy++;
 if(dx||dy){
   const l=Math.hypot(dx,dy);
   p.x+=dx/l*p.s;p.y+=dy/l*p.s;
 }
 p.x=Math.max(25,Math.min(875,p.x));
 p.y=Math.max(30,Math.min(570,p.y));
 for(let i=items.length-1;i>=0;i--){
   const it=items[i];
   if(Math.hypot(p.x-it.x,p.y-it.y)<p.r+it.r){
     score++;
     document.getElementById('score').textContent=score;
     items.splice(i,1);
     if(score<12)spawn();
     else if(!won){
       won=true;
       setTimeout(()=>go(3),500);
     }
   }
 }
 draw();requestAnimationFrame(update);
}
document.addEventListener('keydown',e=>{
 if(e.key.startsWith('Arrow'))e.preventDefault();
 keys[e.key]=true;
});
document.addEventListener('keyup',e=>keys[e.key]=false);

document.querySelectorAll('.controls button').forEach(btn=>{
 const k=btn.dataset.key;
 const down=e=>{e.preventDefault();keys[k]=true};
 const up=e=>{e.preventDefault();keys[k]=false};
 btn.addEventListener('touchstart',down,{passive:false});
 btn.addEventListener('touchend',up,{passive:false});
 btn.addEventListener('touchcancel',up,{passive:false});
 btn.addEventListener('mousedown',down);
 btn.addEventListener('mouseup',up);
 btn.addEventListener('mouseleave',up);
});

/* tap/click inside canvas moves the player; useful on iPhone */
c.addEventListener('pointerdown',e=>{
 const r=c.getBoundingClientRect();
 p.x=(e.clientX-r.left)/r.width*900;
 p.y=(e.clientY-r.top)/r.height*600;
},{passive:true});

update();
</script>
</body>
</html>
