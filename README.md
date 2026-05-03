<!-- 🌙 NIGHT SKY GITHUB README (PASTEL AESTHETIC) -->

<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap');
*{box-sizing:border-box;margin:0;padding:0;}
.wrap{font-family:'DM Sans',sans-serif;max-width:680px;background:#060914;border-radius:20px;overflow:hidden;position:relative;color:#e8e0f0;}
canvas#sky{position:absolute;top:0;left:0;width:100%;height:100%;pointer-events:none;z-index:0;}
.content{position:relative;z-index:1;}
.hero{padding:3rem 2.5rem 2rem;border-bottom:0.5px solid rgba(180,150,220,0.15);}
.hero-name{font-family:'Cormorant Garamond',serif;font-size:3.4rem;font-weight:300;color:#f0eaff;}
.hero-name em{font-style:italic;color:#c8a8f0;}
.hero-tagline{font-size:0.8rem;color:#7a6890;margin-top:0.6rem;}
.pill{font-size:0.65rem;color:#9a7ec0;border:0.5px solid rgba(154,126,192,0.35);padding:4px 12px;border-radius:99px;}
.section{padding:1.5rem 2rem;}
.card{background:rgba(255,255,255,0.025);border-radius:14px;padding:1rem;}
</style>

<div class="wrap">
<canvas id="sky"></canvas>
<div class="content">

<div class="hero">
  <div class="hero-name">Tanya <em>Chaurasia</em></div>
  <div class="hero-tagline">✨ navigating data like stars — finding patterns in the dark</div>
</div>

<div class="section">
  <div class="card">
    💜 Data Science | Machine Learning | AI  
    🌙 Soft intuition meets sharp logic  
  </div>
</div>

<div class="section">
  <div class="card">
    📊 GitHub Stats  
    <img src="https://github-readme-stats.vercel.app/api?username=tanu-1403&show_icons=true&hide_border=true&bg_color=060914&title_color=c8a8f0&text_color=8a78a8"/>
  </div>
</div>

<div class="section">
  <div class="card">
    🌸 Connect  
    🔗 <a href="https://www.linkedin.com/in/tanya-chaurasia-3580b2250">LinkedIn</a>  
    💌 tanyachaurasia1403@gmail.com  
  </div>
</div>

</div>
</div>

<script>
const canvas = document.getElementById('sky');
const ctx = canvas.getContext('2d');
canvas.width = 680;
canvas.height = 400;

const stars = Array.from({length:120},()=>({
  x:Math.random()*canvas.width,
  y:Math.random()*canvas.height,
  r:Math.random()*1.2,
  a:Math.random()
}));

function draw(){
  ctx.clearRect(0,0,canvas.width,canvas.height);
  stars.forEach(s=>{
    ctx.beginPath();
    ctx.arc(s.x,s.y,s.r,0,Math.PI*2);
    ctx.fillStyle=`rgba(220,210,255,${s.a})`;
    ctx.fill();
  });
  requestAnimationFrame(draw);
}
draw();
</script>
