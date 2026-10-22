<!DOCTYPE html>
<html lang="tl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Busog at sulit na tapsilog at silog meals sa Herbosa Street, Tondo, Manila. Bawat menu ay ₱99.">
  <title>Herbosa Tapsi House | Silog Meals ₱99</title>
  <style>
    :root{--red:#a92b1e;--gold:#f4b942;--ink:#25211d;--cream:#fff8ed;--muted:#746b62;--white:#fff}
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{margin:0;font-family:Arial,Helvetica,sans-serif;background:var(--cream);color:var(--ink);line-height:1.6}
    a{color:inherit}
    .topbar{background:#281b16;color:#fff2dc;text-align:center;padding:8px 14px;font-size:.9rem}
    header{position:sticky;top:0;z-index:10;background:rgba(255,248,237,.96);backdrop-filter:blur(8px);border-bottom:1px solid #eadccc}
    .nav{max-width:1150px;margin:auto;padding:14px 22px;display:flex;justify-content:space-between;align-items:center;gap:20px}
    .brand{font-weight:900;font-size:1.15rem;color:var(--red);text-decoration:none;letter-spacing:.2px}
    .brand span{color:var(--ink)}
    .navlinks{display:flex;gap:20px;align-items:center}
    .navlinks a{text-decoration:none;font-weight:700;font-size:.93rem}
    .navlinks a:hover{color:var(--red)}
    .btn{display:inline-block;background:var(--red);color:white;text-decoration:none;padding:12px 18px;border-radius:999px;font-weight:800;border:0;cursor:pointer}
    .btn:hover{background:#812015}
    .btn.gold{background:var(--gold);color:#2a1b12}
    .hero{max-width:1150px;margin:auto;padding:58px 22px 62px;display:grid;grid-template-columns:1fr 1fr;gap:40px;align-items:center}
    .eyebrow{display:inline-block;background:#f9e4b4;color:#6e2c17;font-size:.8rem;letter-spacing:1.4px;font-weight:900;padding:7px 12px;border-radius:999px;text-transform:uppercase}
    h1{font-size:clamp(2.5rem,5vw,4.5rem);line-height:1.03;letter-spacing:-2px;margin:18px 0}
    h1 em{color:var(--red);font-style:normal}
    .hero p{font-size:1.08rem;color:var(--muted);max-width:530px}
    .hero-actions{display:flex;gap:12px;flex-wrap:wrap;margin-top:25px}
    .hero-photo{position:relative}
    .hero-photo img{width:100%;height:430px;object-fit:cover;border-radius:26px;box-shadow:0 18px 45px #5e2b1824}
    .price-sticker{position:absolute;right:-12px;bottom:22px;background:var(--gold);border:5px solid var(--cream);border-radius:50%;width:126px;height:126px;display:grid;place-content:center;text-align:center;transform:rotate(8deg);box-shadow:0 8px 20px #39201224}
    .price-sticker strong{font-size:2rem;line-height:1.1}
    .price-sticker small{font-weight:900;letter-spacing:1px}
    .strip{background:var(--red);color:white;display:flex;justify-content:center;gap:35px;flex-wrap:wrap;padding:15px 18px;font-weight:800}
    section{padding:66px 22px}
    .section-inner{max-width:1150px;margin:auto}
    .section-heading{text-align:center;max-width:650px;margin:0 auto 34px}
    .section-heading h2{font-size:clamp(2rem,4vw,3rem);line-height:1.1;margin:10px 0}
    .section-heading p{color:var(--muted);margin:0}
    .menu-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
    .food-card{background:white;border:1px solid #eee0d0;border-radius:20px;overflow:hidden;box-shadow:0 8px 22px #4023120b;transition:transform .2s,box-shadow .2s}
    .food-card:hover{transform:translateY(-5px);box-shadow:0 14px 30px #40231217}
    .food-card img{width:100%;height:220px;object-fit:cover;display:block;background:#eadccc}
    .food-info{padding:18px}
    .food-title-row{display:flex;justify-content:space-between;gap:10px;align-items:start}
    .food-title-row h3{margin:0;font-size:1.15rem}
    .price{white-space:nowrap;color:var(--red);font-weight:900;font-size:1.08rem}
    .food-info p{margin:8px 0 16px;color:var(--muted);font-size:.94rem;min-height:45px}
    .food-info button{width:100%;padding:10px;border-radius:10px;background:#fff2d7;border:1px solid #f0d69d;color:#653019;font-weight:800;cursor:pointer}
    .food-info button:hover{background:#ffe5ad}
    .note{text-align:center;color:var(--muted);font-size:.9rem;margin-top:22px}
    .about{background:#f5e8d6}
    .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:38px;align-items:center}
    .about-grid img{width:100%;height:350px;object-fit:cover;border-radius:22px}
    .about h2{font-size:clamp(2rem,4vw,3rem);line-height:1.1;margin:14px 0}
    .about p{color:#62564d}
    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:22px}
    .feature{background:#fff9ef;border-radius:14px;padding:15px;font-weight:800}
    .feature span{display:block;font-size:1.4rem;margin-bottom:5px}
    .visit{background:#2a1c16;color:#fff5e7}
    .visit-grid{display:grid;grid-template-columns:1fr 1fr;gap:35px;align-items:center}
    .visit h2{font-size:clamp(2rem,4vw,3rem);line-height:1.1;margin:12px 0}
    .visit p{color:#e4d3c2}
    .address{font-size:1.15rem;font-weight:800;color:white!important}
    .map-frame{width:100%;height:300px;border:0;border-radius:20px;background:#fff}
    footer{background:#1b120e;color:#cbb9a8;text-align:center;padding:23px 18px;font-size:.9rem}
    .cart-toast{position:fixed;bottom:18px;left:50%;transform:translateX(-50%);background:#251a14;color:white;padding:13px 20px;border-radius:999px;box-shadow:0 8px 30px #0003;display:none;z-index:30;max-width:90%;text-align:center}
    @media(max-width:850px){.hero{grid-template-columns:1fr;padding-top:38px}.hero-photo img{height:350px}.menu-grid{grid-template-columns:repeat(2,1fr)}.about-grid,.visit-grid{grid-template-columns:1fr}.navlinks{gap:12px}.navlinks a:not(.btn){display:none}}
    @media(max-width:560px){.nav{padding:12px 15px}.brand{font-size:1rem}.navlinks .btn{padding:9px 12px;font-size:.85rem}.hero{padding-left:17px;padding-right:17px}.hero-photo img{height:285px}.price-sticker{width:100px;height:100px;right:-5px}.price-sticker strong{font-size:1.6rem}section{padding:48px 17px}.menu-grid{grid-template-columns:1fr}.food-card img{height:235px}.features{grid-template-columns:1fr}.strip{gap:10px 22px;font-size:.88rem}}
  </style>
</head>
<body>
  <div class="topbar">🍳 Mainit, masarap, at sulit — lahat ng silog meals ay ₱99!</div>
  <header>
    <nav class="nav">
      <a class="brand" href="#home">HERBOSA <span>TAPSI HOUSE</span></a>
      <div class="navlinks">
        <a href="#menu">Menu</a>
        <a href="#about">Tungkol sa Amin</a>
        <a href="#location">Lokasyon</a>
        <a class="btn" href="#menu">Tingnan ang Menu</a>
      </div>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div>
        <span class="eyebrow">Tapsilogan sa Tondo</span>
        <h1>Busog ka na,<br><em>₱99 lang!</em></h1>
        <p>Craving sa silog? Tara sa Herbosa Tapsi House para sa Pinoy comfort food na bagong luto, masarap, at swak sa budget.</p>
        <div class="hero-actions">
          <a class="btn" href="#menu">🍽️ Pili na ng ulam</a>
          <a class="btn gold" href="#location">📍 Paano pumunta?</a>
        </div>
      </div>
      <div class="hero-photo">
        <img src="https://images.unsplash.com/photo-1544025162-d76694265947?auto=format&fit=crop&w=1000&q=85" alt="Masarap na pagkaing handa para sa kainan">
        <div class="price-sticker"><small>LAHAT NG MENU</small><strong>₱99</strong><small>LANG!</small></div>
      </div>
    </section>

    <div class="strip"><span>🥩 Lutong Pinoy</span><span>🍳 Bagong luto</span><span>💸 Presyong sulit</span><span>📍 Herbosa St., Tondo</span></div>

    <section id="menu">
      <div class="section-inner">
        <div class="section-heading">
          <span class="eyebrow">Paboritong silog</span>
          <h2>Menu namin</h2>
          <p>Pumili ng paborito mong silog meal. Bawat item ay <strong>₱99</strong>.</p>
        </div>
        <div class="menu-grid">
          <article class="food-card">
            <img src="https://images.unsplash.com/photo-1512058564366-18510be2db19?auto=format&fit=crop&w=800&q=85" alt="Tapsilog meal" loading="lazy">
            <div class="food-info"><div class="food-title-row"><h3>Tapsilog</h3><span class="price">₱99</span></div><p>Beef tapa, sinangag, at pritong itlog.</p><button onclick="addItem('Tapsilog')">+ Piliin ang Tapsilog</button></div>
          </article>
          <article class="food-card">
            <img src="https://images.unsplash.com/photo-1604908176997-125f25cc6f3d?auto=format&fit=crop&w=800&q=85" alt="Longsilog meal" loading="lazy">
            <div class="food-info"><div class="food-title-row"><h3>Longsilog</h3><span class="price">₱99</span></div><p>Matamis-alat na longganisa, sinangag, at itlog.</p><button onclick="addItem('Longsilog')">+ Piliin ang Longsilog</button></div>
          </article>
          <article class="food-card">
            <img src="https://images.unsplash.com/photo-1525351484163-7529414344d8?auto=format&fit=crop&w=800&q=85" alt="Tocilog meal" loading="lazy">
            <div class="food-info"><div class="food-title-row"><h3>Tocilog</h3><span class="price">₱99</span></div><p>Tocino, sinangag, at itlog — klasikong almusal.</p><button onclick="addItem('Tocilog')">+ Piliin ang Tocilog</button></div>
          </article>
          <article class="food-card">
            <img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?auto=format&fit=crop&w=800&q=85" alt="Pork chop meal" loading="lazy">
            <div class="food-info"><div class="food-title-row"><h3>Porksilog</h3><span class="price">₱99</span></div><p>Pork chop, sinangag, at itlog para sa solid na kain.</p><button onclick="addItem('Porksilog')">+ Piliin ang Porksilog</button></div>
          </article>
          <article class="food-card">
            <img src="https://images.unsplash.com/photo-1604908554162-45dae9b3a7a2?auto=format&fit=crop&w=800&q=85" alt="Chicken meal" loading="lazy">
            <div class="food-info"><div class="food-title-row"><h3>Chicksilog</h3><span class="price">₱99</span></div><p>Crispy chicken, sinangag, at pritong itlog.</p><button onclick="addItem('Chicksilog')">+ Piliin ang Chicksilog</button></div>
          </article>
          <article class="food-card">
            <img src="https://images.unsplash.com/photo-1547592180-85f173990554?auto=format&fit=crop&w=800&q=85" alt="Hotdog silog meal" loading="lazy">
            <div class="food-info"><div class="food-title-row"><h3>Hotsilog</h3><span class="price">₱99</span></div><p>Hotdog, sinangag, at itlog — simple pero panalo.</p><button onclick="addItem('Hotsilog')">+ Piliin ang Hotsilog</button></div>
          </article>
        </div>
        <p class="note">Sample menu para sa website concept. Palitan ang mga larawan at item kung iba ang aktuwal na menu ng tindahan.</p>
      </div>
    </section>

    <section class="about" id="about">
      <div class="section-inner about-grid">
        <img src="https://images.unsplash.com/photo-1555939594-58d7cb561ad1?auto=format&fit=crop&w=1000&q=85" alt="Pagkaing Pinoy na pinagsasaluhan" loading="lazy">
        <div>
          <span class="eyebrow">Sarap na pang-araw-araw</span>
          <h2>Simple. Sulit. Pinoy na Pinoy.</h2>
          <p>Sa Herbosa Tapsi House, ang goal ay ihain ang mga paboritong silog meal sa presyong kayang balikan. Pang-almusal, pang-tanghalian, pang-hapunan, o pang-midnight cravings.</p>
          <div class="features">
            <div class="feature"><span>🍳</span>Silog favorites</div>
            <div class="feature"><span>₱</span>₱99 bawat meal</div>
            <div class="feature"><span>📍</span>Tondo, Manila</div>
          </div>
        </div>
      </div>
    </section>

    <section class="visit" id="location">
      <div class="section-inner visit-grid">
        <div>
          <span class="eyebrow">Hanapin kami</span>
          <h2>Kita-kits sa Tondo!</h2>
          <p class="address">📍 Herbosa Street, Tondo, Manila, Philippines</p>
          <p>Maghanap ng direksyon gamit ang Google Maps. Ilagay ang eksaktong landmark kung mayroon para mas madali kang makarating.</p>
          <a class="btn gold" target="_blank" rel="noopener" href="https://www.google.com/maps/search/?api=1&query=Herbosa+Street%2C+Tondo%2C+Manila">Buksan ang Google Maps ↗</a>
        </div>
        <iframe class="map-frame" title="Mapa papuntang Herbosa Street, Tondo, Manila" loading="lazy" src="https://maps.google.com/maps?q=Herbosa%20Street%2C%20Tondo%2C%20Manila&t=&z=14&ie=UTF8&iwloc=&output=embed" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>
    </section>
  </main>

  <footer>© <span id="year"></span> Herbosa Tapsi House · Herbosa Street, Tondo, Manila<br>Masarap na silog, presyong sulit — ₱99 bawat menu.</footer>
  <div class="cart-toast" id="toast" role="status" aria-live="polite"></div>
  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    let toastTimer;
    function addItem(item){
      const toast=document.getElementById('toast');
      toast.textContent=item+' ang napili mo — ₱99. Demo lang ang button na ito; wala pang online ordering.';
      toast.style.display='block';
      clearTimeout(toastTimer);
      toastTimer=setTimeout(()=>toast.style.display='none',3500);
    }
  </script>
</body>
</html>
