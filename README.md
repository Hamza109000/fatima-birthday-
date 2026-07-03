# fatima-birthday-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Fatima ❤️</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&family=Great+Vibes&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:linear-gradient(135deg,#ffd6e7,#ffeef5);
overflow-x:hidden;
color:#fff;
}

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
position:relative;
}

.hero h1{
font-size:55px;
font-family:'Great Vibes',cursive;
animation:fadeDown 2s ease;
text-shadow:0 0 15px #ff4f9d;
}

.hero h2{
margin-top:15px;
font-size:24px;
font-weight:300;
animation:fadeUp 2s ease;
}

.hero button{
margin-top:35px;
padding:15px 35px;
border:none;
border-radius:50px;
font-size:18px;
cursor:pointer;
background:#ff4f9d;
color:white;
box-shadow:0 10px 30px rgba(255,0,102,.4);
transition:.4s;
}

.hero button:hover{
transform:scale(1.08);
}

section{
padding:80px 25px;
}

.card{
background:white;
color:#444;
max-width:900px;
margin:auto;
padding:35px;
border-radius:25px;
box-shadow:0 15px 40px rgba(0,0,0,.15);
}

.card h2{
color:#ff3b88;
margin-bottom:20px;
font-family:'Great Vibes',cursive;
font-size:45px;
text-align:center;
}

.card p{
line-height:1.9;
font-size:18px;
text-align:center;
}

.gallery{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
gap:20px;
margin-top:40px;
}

.gallery img{
width:100%;
border-radius:20px;
box-shadow:0 10px 25px rgba(0,0,0,.2);
transition:.5s;
}

.gallery img:hover{
transform:scale(1.06);
}

footer{
padding:50px;
text-align:center;
font-size:20px;
}

@keyframes fadeDown{
from{
opacity:0;
transform:translateY(-80px);
}
to{
opacity:1;
transform:translateY(0);
}
}

@keyframes fadeUp{
from{
opacity:0;
transform:translateY(80px);
}
to{
opacity:1;
transform:translateY(0);
}
}

</style>
</head>

<body>

<div class="hero">

<h1>Happy Birthday Fatima ❤️</h1>

<h2>A little surprise made with love by Mahi 🌸</h2>

<button onclick="document.getElementById('letter').scrollIntoView({behavior:'smooth'})">
Open Surprise 🎁
</button>

</div>

<section id="letter">

<div class="card">

<h2>Dear Fatima 💌</h2>

<p>

Happy Birthday to the most beautiful soul. 🌸

Even though distance keeps us apart,
my prayers and best wishes are always with you.

Thank you for being such an amazing friend.

May Allah bless you with endless happiness,
good health, peace and success.

Never stop smiling because your smile makes
everyone around you happier.

I hope today becomes one of the most beautiful
days of your life.

Happy Birthday once again.

With lots of love ❤️

<b>— Mahi</b>

</p>

<div class="gallery">

<img src="photo1.jpg">
<img src="photo2.jpg">
<img src="photo3.jpg">
<img src="photo4.jpg">
<img src="photo5.jpg">
<img src="photo6.jpg">
<img src="photo7.jpg">
<img src="photo8.jpg">
<img src="photo9.jpg">
<img src="photo10.jpg">

</div>

</div>

</section>

<footer>

Made with ❤️ by Mahi

</footer>
<script>

// Floating Hearts
function createHeart() {
  const heart = document.createElement("div");
  heart.innerHTML = "💖";
  heart.style.position = "fixed";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.top = "100vh";
  heart.style.fontSize = (20 + Math.random() * 20) + "px";
  heart.style.zIndex = "9999";
  heart.style.pointerEvents = "none";
  heart.style.transition = "transform 6s linear, opacity 6s linear";
  document.body.appendChild(heart);

  setTimeout(() => {
    heart.style.transform = `translateY(-120vh) rotate(${Math.random()*360}deg)`;
    heart.style.opacity = "0";
  }, 100);

  setTimeout(() => {
    heart.remove();
  }, 6000);
}

setInterval(createHeart, 500);

// Surprise Button
const btn = document.querySelector("button");

btn.addEventListener("click", () => {

  for(let i=0;i<80;i++){

    const confetti=document.createElement("div");

    confetti.innerHTML="🎉";

    confetti.style.position="fixed";

    confetti.style.left=Math.random()*100+"vw";

    confetti.style.top="-20px";

    confetti.style.fontSize="24px";

    confetti.style.transition="4s linear";

    document.body.appendChild(confetti);

    setTimeout(()=>{

      confetti.style.top="110vh";

      confetti.style.transform="rotate(720deg)";

    },100);

    setTimeout(()=>{

      confetti.remove();

    },4000);

  }

});

</script>
</body>
</html>