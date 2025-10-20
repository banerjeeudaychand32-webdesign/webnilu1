<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Happy Diwali</title>
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
  height:100vh;
  background:radial-gradient(circle at bottom,#10002b 0%,#03001c 100%);
  overflow:hidden;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  color:#fff;
  font-family:'Poppins',sans-serif;
}
h1{
  font-size:3rem;
  text-align:center;
  color:#ffd700;
  text-shadow:0 0 20px #ffb300,0 0 40px #ff9100,0 0 80px #ff9100;
  animation:glow 2s ease-in-out infinite alternate;
}
@keyframes glow{
  from{text-shadow:0 0 10px #ff9100,0 0 20px #ff6a00;}
  to{text-shadow:0 0 20px #ffd700,0 0 40px #ffb300,0 0 80px #ff6a00;}
}

/* diya lamp */
.diya{
  position:relative;
  width:80px;
  height:40px;
  background:linear-gradient(to top,#a0522d,#8b4513);
  border-radius:0 0 40px 40px;
  margin-top:2rem;
  box-shadow:0 5px 15px rgba(0,0,0,0.5);
}
.flame{
  position:absolute;
  top:-40px;
  left:50%;
  transform:translateX(-50%);
  width:20px;
  height:40px;
  background:radial-gradient(circle at 50% 80%,#fff 0%,#ff0 40%,#ff6a00 70%,transparent 100%);
  border-radius:50% 50% 50% 50%;
  animation:flicker 0.2s infinite;
}
@keyframes flicker{
  0%,100%{transform:translateX(-50%) scale(1);}
  50%{transform:translateX(-50%) scale(0.9);}
}

/* fireworks */
.firework{
  position:absolute;
  border-radius:50%;
  pointer-events:none;
}
</style>
</head>
<body>
  <h1>🎆 Happy Diwali 2025 🎇</h1>
  <div class="diya"><div class="flame"></div></div>

<script>
// fireworks
function createFirework(){
  const f=document.createElement("div");
  f.classList.add("firework");
  const size=Math.random()*8+4;
  f.style.width=f.style.height=size+"px";
  f.style.background=`hsl(${Math.random()*360},100%,60%)`;
  f.style.left=Math.random()*100+"vw";
  f.style.top=Math.random()*80+"vh";
  document.body.appendChild(f);
  const duration=1000+Math.random()*1000;
  f.animate([
    {transform:scale(0),opacity:1},
    {transform:scale(1.5),opacity:0}
  ],{duration,easing:"ease-out"});
  setTimeout(()=>f.remove(),duration);
}
setInterval(createFirework,200);

// diya glow
setInterval(()=>{
  document.querySelector('.flame').style.filter = `hue-rotate(${Math.random()*60-30}deg)`;
},150);
</script>
</body>
</html>
