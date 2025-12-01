<!DOCTYPE html>

<html lang="sw">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AMA FM RADIO</title>
  <style>
    /* CSS */
    body { font-family: Arial, sans-serif; margin:0; padding:0; background:#101820; color:#f2f2f2; }
    header { background:#0d1b2a; padding:20px; text-align:center; }
    nav { background:#1b263b; padding:10px; text-align:center; }
    nav a { color:white; margin:0 15px; text-decoration:none; font-weight:bold; }
    section { padding:40px; max-width:900px; margin:auto; }
    .logo { width:150px; }
    .btn-radio { padding:12px 20px; background:#ff8800; color:white; border:none; cursor:pointer; font-size:16px; margin-top:20px; border-radius:6px; }
    .btn-radio.off { background:#444; }
    #playerBox { margin-top:25px; display:none; }
    footer { background:#0d1b2a; color:white; text-align:center; padding:15px; margin-top:40px; }
    .lang-switch { position: fixed; top: 20px; right: 20px; }
    .lang-switch button { padding: 8px 14px; margin-left:5px; border:none; cursor:pointer; background:#333; color:#fff; border-radius:6px; }
    .lang-switch button.active { background:#ff8800; }
  </style>
</head>
<body>
  <!-- Language Switch -->
  <div class="lang-switch">
    <button id="swBtn" class="active">SW</button>
    <button id="enBtn">EN</button>
  </div>

  <header>
    <img src="images/logo.png" alt="AMA FM Logo" class="logo">
    <h1 lang="sw">AMA FM RADIO</h1>
    <h1 lang="en" style="display:none;">AMA FM RADIO</h1>
    <p lang="sw">Sauti ya Kizazi Kipya</p>
    <p lang="en" style="display:none;">Voice of the New Generation</p>
  </header>

  <nav>
    <a href="#home" lang="sw">Home</a>
    <a href="#about" lang="sw">Kuhusu</a>
    <a href="#shows" lang="sw">Vipindi</a>
    <a href="#contact" lang="sw">Mawasiliano</a>

```
<a href="#home" lang="en" style="display:none;">Home</a>
<a href="#about" lang="en" style="display:none;">About</a>
<a href="#shows" lang="en" style="display:none;">Programs</a>
<a href="#contact" lang="en" style="display:none;">Contact</a>
```

  </nav>

  <section id="home">
    <h2 lang="sw">Karibu AMA FM Radio</h2>
    <h2 lang="en" style="display:none;">Welcome to AMA FM Radio</h2>
    <p lang="sw">
      Ama FM ni kituo cha redio kinachojikita katika kuelimisha na kuwawezesha vijana kupitia vipindi vya teknolojia,
      mitandao na ujuzi muhimu kwa maendeleo yao. Tunatoa maudhui bunifu yanayochochea ubunifu, fikra mpya na matumizi
      sahihi ya teknolojia katika maisha ya kila siku.
    </p>
    <p lang="en" style="display:none;">
      AMA FM is a youth-focused radio station dedicated to education and empowerment through technology programs,
      networks, and essential skills for personal development. We provide innovative content that encourages creativity
      and practical technology use.
    </p>

```
<button id="radioBtn" class="btn-radio">▶ Washa Radio</button>

<div id="playerBox">
  <iframe src="https://zeno.fm/radio/ama-fm/" width="100%" height="300" frameborder="0" allow="autoplay"></iframe>
</div>
```

  </section>

  <section id="about">
    <h2 lang="sw">Kuhusu AMA FM</h2>
    <h2 lang="en" style="display:none;">About AMA FM</h2>
    <p lang="sw">
      AMA FM Radio ni redio ya mtandaoni inayolenga kuwawezesha vijana kwa maarifa ya teknolojia, ubunifu na matumizi bora
      ya mitandao. Kupitia wataalamu na watangazaji makini, tunawafikia vijana kwa elimu, burudani na mjadala wenye tija.
    </p>
    <p lang="en" style="display:none;">
      AMA FM Radio is an online station focused on empowering youth with technology knowledge, creativity, and effective
      digital use. Through experts and dedicated presenters, we provide education, entertainment, and constructive discussions.
    </p>
    <p lang="sw"><strong>Dira:</strong> Kuwa redio bora ya kidigitali inayopaza sauti ya vijana na kuwaandaa kwa mustakabali wa teknolojia.</p>
    <p lang="en" style="display:none;"><strong>Vision:</strong> To be the leading digital radio empowering youth and preparing them for the future of technology.</p>
    <p lang="sw"><strong>Dhamira:</strong> Kuwapa vijana elimu, ujuzi na nafasi za kushiriki katika ulimwengu wa kisasa wa digitali.</p>
    <p lang="en" style="display:none;"><strong>Mission:</strong> To provide youth with education, skills, and opport
