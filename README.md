# Drama-queen
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Bas kr drama queen</title>
<style>
  body {
    margin: 0;
    font-family: 'Comic Sans MS', cursive, sans-serif;
    background: linear-gradient(270deg, #ff9a9e, #fad0c4, #fbc2eb, #a1c4fd, #c2e9fb);
    background-size: 1000% 1000%;
    animation: gradientBG 15s ease infinite;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
  }
  @keyframes gradientBG {
    0% {background-position: 0% 50%;}
    50% {background-position: 100% 50%;}
    100% {background-position: 0% 50%;}
  }
  .screen {
    text-align: center;
    padding: 20px;
    background-color: rgba(255, 255, 255, 0.75);
    border-radius: 20px;
    animation: fadeIn 0.8s ease-in-out;
    max-width: 85%;
  }
  h1 {
    font-size: 2em;
    margin-bottom: 20px;
  }
  p {
    font-size: 1.2em;
    margin-bottom: 30px;
  }
  button {
    padding: 10px 20px;
    font-size: 1em;
    margin: 10px;
    background-color: #ff4081;
    color: white;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    position: relative;
  }
  img {
    max-width: 250px;
    margin-top: 20px;
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: scale(0.9); }
    to { opacity: 1; transform: scale(1); }
  }
</style>
</head>
<body>

<audio autoplay loop>
  <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3" type="audio/mpeg">
</audio>

<!-- Slide 1 -->
<div class="screen" id="screen1">
  <h1>Mard apni pasandida aurat ke liye hi itni mehnat krta hai 😩❤️💻</h1>
  <p>Do you love me?</p>
  <button onclick="goTo(2)">Yes 😍</button>
  <button id="no1" onmouseover="moveButton('no1')">No 😒</button>
</div>

<!-- Slide 2 -->
<div class="screen" id="screen2" style="display:none;">
  <h1>Mere ko pta tha 😂</h1>
  <p>Mai to check kr rha tha tera bhool bhal to nhi gyii tu mere ko 😏</p>
  <button onclick="goTo(3)">Next ➡️</button>
</div>

<!-- Slide 3 -->
<div class="screen" id="screen3" style="display:none;">
  <h1>Tu kyaa mere se gussa hai kya? 😯</h1>
  <button id="no2" onclick="goTo(4)">No 😇</button>
  <button id="yes2" onmouseover="moveButton('yes2')">Yes 😡</button>
</div>

<!-- Slide 4 -->
<div class="screen" id="screen4" style="display:none;">
  <h1>😂 Yha sirf meri marzi chelegi madam hahaha...</h1>
  <button onclick="goTo(5)">Next ➡️</button>
</div>

<!-- Slide 5 -->
<div class="screen" id="screen5" style="display:none;">
  <h1>Itna gussa kuuu kr rhi hai 😅<br>Sach mai Angry Bird hai kya? 🐦</h1>
  <p>(Isme tu apna choice kr)</p>
  <button onclick="goTo(6)">Yes 😤</button>
  <button id="no3" onmouseover="moveButton('no3')">No 🙄</button>
</div>

<!-- Slide 6 -->
<div class="screen" id="screen6" style="display:none;">
  <h1>Angry Bird Confirmed! 😂</h1>
  <img src="https://upload.wikimedia.org/wikipedia/en/0/0b/RedAngryBird.png" alt="Angry Bird">
  <button onclick="goTo(9)">Next ➡️</button>
</div>

<!-- Slide 9 -->
<div class="screen" id="screen9" style="display:none;">
  <h1>Ese aloo ki trah fool mt... tikki bnaa ke khaa jaunga 😏🥔</h1>
  <button onclick="goTo(10)">Next ➡️</button>
</div>

<!-- Slide 10 -->
<div class="screen" id="screen10" style="display:none;">
  <h1>Tu digitally ese molest kr rhi hai mere ko 😨💀<br>Physically toh maar degi kya? RIP ☠️</h1>
  <button onclick="goTo(11)">Yes 😆 Tu mera hi toh mard hai, kuch bhi krungi mai to pgl hu 🤣</button>
  <button id="no10" onmouseover="moveButton('no10')">Nhi mai bhut achii hu 😇</button>
</div>

<!-- Slide 11 -->
<div class="screen" id="screen11" style="display:none;">
  <h1>Bhai mere dil ki battery is fight ke baad low ho gyi hai 🔋💔<br>Charge kr degi kya?</h1>
  <button onclick="goTo(12)">Yes 🔌</button>
  <button id="no11" onmouseover="moveButton('no11')">No 😏</button>
</div>

<!-- Slide 12 -->
<div class="screen" id="screen12" style="display:none;">
  <h1>Sunn... ab jagda krne ke baad meri face ke muscles bhut weak ho gyii hai 😩<br>Sukk gya hai... ek Vit. U ke sath pappi de de 😘<br>(Doctor ne bola hai... tu hi toh bolti hai doctor ki baat sunni chiye)</h1>
  <button onclick="goTo(8)">Yes Jrur 😍</button>
  <button onclick="goTo(8)">No 💄 Lipstick lga ke dungi 😉</button>
</div>

<!-- Slide 8 -->
<div class="screen" id="screen8" style="display:none;">
  <h1>I Love You ❤️</h1>
  <img src="https://cdn.pixabay.com/photo/2017/08/06/00/05/teddy-bear-2589971_1280.jpg" alt="Teddy with chocolates and flowers">
  <button onclick="goTo(13)">Next ➡️</button>
</div>

<!-- Slide 13 (Final) -->
<div class="screen" id="screen13" style="display:none;">
  <h1>Bhut mehnt krra hai Noto 😅<br>Koi ladka itna pyaar nhi krega ❤️🤗<br>Challenge hai saab ko — koi mere se jda pyaar kr ke dikha de...<br>Aur koi mil bhi gya toh nali mai fek dunga usko 😘🤗</h1>
  <p>Mannn jaa... sunnnaa... bhut miss kr rha hu ❤️</p>
</div>

<script>
  function goTo(num) {
    document.querySelectorAll('.screen').forEach(s => s.style.display = 'none');
    document.getElementById('screen' + num).style.display = 'block';
  }
  function moveButton(id) {
    const btn = document.getElementById(id);
    const maxX = window.innerWidth - btn.offsetWidth - 50;
    const maxY = window.innerHeight - btn.offsetHeight - 50;
    const x = Math.floor(Math.random() * maxX);
    const y = Math.floor(Math.random() * maxY);
    btn.style.position = 'absolute';
    btn.style.left = x + 'px';
    btn.style.top = y + 'px';
  }
</script>

</body>
</html>
