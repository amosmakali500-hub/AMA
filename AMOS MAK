<!DOCTYPE html>
<html lang="sw">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AMA FM RADIO</title>
<style>
  /* Global Styles */
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin:0; padding:0;
    background: url('images/background.jpg') no-repeat center center fixed;
    background-size: cover;
    color: #fff;
  }
  header {
    background: rgba(13,27,42,0.85);
    padding:20px; text-align:center;
  }
  header .logo {
    width:120px;
    border-radius:10px;
  }
  nav {
    background: rgba(27,38,59,0.9);
    padding:10px;
    text-align:center;
  }
  nav a {
    color:white; margin:0 20px; text-decoration:none;
    font-weight:bold; font-size:16px;
    transition: 0.3s;
  }
  nav a:hover { color:#ff8800; }
  section {
    padding:50px 20px; max-width:1000px; margin:auto;
    background: rgba(0,0,0,0.5); border-radius:10px; margin-bottom:30px;
  }
  h2 { color:#ff8800; margin-bottom:15px; }
  .btn-radio {
    padding:15px 25px; font-size:18px;
    background:#ff8800; border:none; cursor:pointer;
    border-radius:8px; margin-top:20px;
    transition:0.3s;
  }
  .btn-radio:hover { background:#e66b00; }
  #playerBox { margin-top:20px; }
  footer {
    background: rgba(13,27,42,0.85);
    text-align:center; padding:20px;
  }
  /* Language Switcher */
  .lang-switch { position: fixed; top:20px; right:20px; z-index:999; }
  .lang-switch button {
    padding: 8px 14px; margin-left:5px;
    border:none; cursor:pointer;
    background:#333; color:#fff; border-radius:6px;
    transition:0.3s;
  }
  .lang-switch button.active { background:#ff8800; }

  /* Table Styles */
  table {
    width:100%; border-collapse:collapse; margin-top:20px;
    background: rgba(27,38,59,0.8);
  }
  th, td { padding:12px; border:1px solid #fff; text-align:left; }
  th { background:#ff8800; color:#fff; }

  /* Responsive */
  @media(max-width:768px){
    nav a { display:block; margin:10px 0; }
  }
</style>
</head>
<body>

<!-- Language Switcher -->
<div class="lang-switch">
  <button id="swBtn" class="active">SW</button>
  <button id="enBtn">EN</button>
</div>

<header>
  <img src="images/logo.png" alt="AMA FM Logo" class="logo">
  <h1>AMA FM RADIO</h1>
  <p>Sauti ya Kizazi Kipya</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#about">Kuhusu</a>
  <a href="#shows">Vipindi</a>
  <a href="#contact">Mawasiliano</a>
</nav>

<section id="home">
  <h2>Karibu AMA FM Radio</h2>
  <p>Ama FM ni kituo cha redio kinachojikita katika kuelimisha na kuwawezesha vijana kupitia vipindi vya teknolojia, mitandao na ujuzi muhimu kwa maendeleo yao.</p>

  <button id="radioBtn" class="btn-radio">▶ Washa Radio</button>
  <div id="playerBox">
    <audio id="radioPlayer" controls></audio>
  </div>
</section>

<section id="about">
  <h2>Kuhusu AMA FM</h2>
  <p><strong>Dira:</strong> Kuwa redio bora ya kidigitali inayopaza sauti ya vijana na kuwaandaa kwa mustakabali wa teknolojia.</p>
  <p><strong>Dhamira:</strong> Kuwapa vijana elimu, ujuzi na nafasi za kushiriki katika ulimwengu wa kisasa wa digitali.</p>
</section>

<section id="shows">
  <h2>Vipindi Vyetu</h2>
  <table>
    <thead>
      <tr><th>Wakati</th><th>Kipindi</th><th>Maelezo</th><th>Status</th></tr>
    </thead>
    <tbody>
      <tr><td>06:00 - 07:00</td><td>Tech Zone</td><td>Habari za teknolojia, AI, vifaa vipya na fursa za digitali.</td><td class="status"></td></tr>
      <tr><td>07:00 - 08:00</td><td>Habari Kuu</td><td>Kipindi cha habari, kina kuruka kila siku saa moja kamili jioni.</td><td class="status"></td></tr>
      <tr><td>08:00 - 09:00</td><td>Youth Power Talk</td><td>Majadiliano ya changamoto, mafanikio na maendeleo ya vijana.</td><td class="status"></td></tr>
      <tr><td>10:00 - 11:00</td><td>Digital Skills Hour</td><td>Elimu ya mitandao, content creation na online safety.</td><td class="status"></td></tr>
      <tr><td>16:00 - 17:00</td><td>Ama Gospel Morning</td><td>Malezi, maadili na mafundisho ya imani.</td><td class="status"></td></tr>
      <tr><td>19:00 - 21:00</td><td>Weekend Creators</td><td>Muziki, burudani na ubunifu.</td><td class="status"></td></tr>
    </tbody>
  </table>
</section>

<section id="contact">
  <h2>Mawasiliano</h2>
  <p><strong>Simu:</strong> 0745 840 620</p>
  <p><strong>Email:</strong> amosmakali500@gmail.com</p>
  <p><strong>Mahali:</strong> Tanzania</p>
</section>

<footer>
  <p>© 2025 AMA FM RADIO | Sauti ya Kizazi Kipya</p>
</footer>

<script>
  // Radio player
  const radioBtn = document.getElementById('radioBtn');
  const radioPlayer = document.getElementById('radioPlayer');
  radioPlayer.src = "https://zeno.fm/stream/ama-fm.mp3"; // Badilisha na stream URL halisi
  let isPlaying = false;

  radioBtn.onclick = () => {
    if(isPlaying){
      radioPlayer.pause();
      radioBtn.textContent="▶ Washa Radio";
    } else {
      radioPlayer.play();
      radioBtn.textContent="⏹ Zima Radio";
    }
    isPlaying = !isPlaying;
  }

  // Language Switcher
  const swBtn = document.getElementById('swBtn');
  const enBtn = document.getElementById('enBtn');

  function setLanguage(lang){
    if(lang==='sw'){ swBtn.classList.add('active'); enBtn.classList.remove('active'); }
    else{ enBtn.classList.add('active'); swBtn.classList.remove('active'); }
  }
  swBtn.onclick=()=>setLanguage('sw');
  enBtn.onclick=()=>setLanguage('en');

  // Live Now Indicator
  function updateSchedule(){
    const now = new Date();
    const hours = now.getHours();
    const minutes = now.getMinutes();
    const time = hours + minutes/60;
    document.querySelectorAll('#shows tbody tr').forEach(tr=>{
      const [start,end]=tr.cells[0].innerText.split(' - ');
      const startH = parseInt(start.split(':')[0]) + parseInt(start.split(':')[1])/60;
      const endH = parseInt(end.split(':')[0]) + parseInt(end.split(':')[1])/60;
      tr.cells[3].innerText = (time>=startH && time<endH)?'LIVE NOW 🔴':'';
    });
  }
  setInterval(updateSchedule,60000);
  updateSchedule();
</script>
</body>
</html>
