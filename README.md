# landing1
my landing 
  <!DOCTYPE html>
  <html lang="he" dir="rtl">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Refined Bar — מיקסולוגיה פרימיום לאירועים</title>
    <meta name="description" content="Refined Bar — מיקסולוגיה פרימיום לאירועים. בר קוקטיילים מותאם אישית עם צוות מנוסה, תפריט שנבנה סביב אופי האירוע ומשקאות פוטוגניים שנראים ומרגישים חלק מהחוויה.">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Frank+Ruhl+Libre:wght@500;700;800&family=Heebo:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
      :root{
        --bg:#f8f5ef;--bg-2:#eee6d8;--text:#111820;--muted:#667070;
        --navy:#0b1620;--navy-soft:rgba(11,22,32,.08);
        --teal:#147c78;--teal-bright:#22a7a0;--teal-soft:rgba(20,124,120,.12);
        --gold:#c6a15b;--gold-bright:#d8b86f;--gold-soft:rgba(198,161,91,.16);
        --citrus:#d98b3a;--citrus-soft:rgba(217,139,58,.14);
        --card:rgba(255,255,255,.86);--border:rgba(17,24,32,.12);--radius:22px;
        --straw:var(--teal);--straw-soft:var(--teal-soft);
        --plum:var(--navy);--orange:var(--gold);
        --ease:cubic-bezier(.22,1,.36,1);
      }
      *{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent}
      html{scroll-behavior:smooth;scroll-padding-top:86px}
      body{
        font-family:'Heebo',sans-serif;color:var(--text);font-size:16px;
        line-height:1.65;overflow-x:hidden;
        background:
          radial-gradient(circle at 18% 0%,rgba(198,161,91,.14),transparent 28%),
          radial-gradient(circle at 90% 12%,rgba(20,124,120,.12),transparent 30%),
          linear-gradient(180deg,#fffdfb 0%,var(--bg) 40%,var(--bg-2) 100%);
      }
      h1,h2,h3,h4{font-family:'Frank Ruhl Libre',serif;font-weight:700;color:var(--navy)}
      a{text-decoration:none;color:inherit}
      button,input,textarea{font:inherit}
      button{touch-action:manipulation}
      strong{color:var(--teal);font-weight:700}
      :focus-visible{outline:3px solid var(--teal);outline-offset:5px}
      .container{max-width:900px;margin:0 auto;padding:0 22px;position:relative;z-index:2}
      .bg-fruit{
        position:fixed;right:0;top:0;z-index:0;pointer-events:none;width:100%;height:58vh;
        background:url("bg-fruit.png") right center/cover no-repeat;opacity:.46;
        -webkit-mask-image:linear-gradient(180deg,#000 40%,transparent 100%);
        mask-image:linear-gradient(180deg,#000 40%,transparent 100%);
        animation:floatBg 16s ease-in-out infinite alternate;
      }
      @keyframes floatBg{from{transform:translateY(0) scale(1)}to{transform:translateY(-18px) scale(1.03)}}
      nav{
        position:fixed;top:0;left:0;right:0;z-index:100;display:flex;align-items:center;
        gap:12px;padding:12px 20px;background:rgba(248,245,239,.88);
        -webkit-backdrop-filter:blur(14px);backdrop-filter:blur(14px);
        border-bottom:1px solid rgba(17,24,32,.08);
      }
      nav img{width:38px;height:38px;object-fit:contain;mix-blend-mode:multiply}
      .brand{font-family:'Frank Ruhl Libre',serif;font-size:1.45rem;font-weight:800;color:var(--navy);line-height:1}
      .brand span{color:var(--teal)}
      .hero{
        min-height:80svh;display:flex;align-items:center;justify-content:center;text-align:center;
        padding:96px 22px 40px;position:relative;z-index:2;
      }
      .hero-inner{max-width:700px;position:relative}
      .hero-inner::before{
        content:"";position:absolute;z-index:-1;pointer-events:none;left:50%;top:-35px;
        transform:translateX(-50%);width:300px;height:250px;border-radius:50%;
        background:radial-gradient(circle,rgba(216,184,111,.22) 0%,rgba(248,245,239,.78) 45%,transparent 72%);
      }
      .hero-logo-wrap{
        display:inline-flex;align-items:center;justify-content:center;padding:16px;border-radius:40px;
        background:rgba(255,255,255,.52);backdrop-filter:blur(6px);margin-bottom:16px;
      }
      .hero-logo{width:180px;max-width:56vw;display:block;mix-blend-mode:multiply;animation:logoIn 1.2s ease both}
      @keyframes logoIn{from{opacity:0;transform:translateY(20px) scale(.94)}to{opacity:1;transform:none}}
      .kicker{font-size:.78rem;letter-spacing:.08em;color:var(--teal);margin-bottom:12px;font-weight:700}
      .hero h1{font-size:clamp(2.45rem,8.5vw,4.45rem);line-height:1.08;margin-bottom:18px}
      .hero h1 em{font-style:normal;color:var(--teal)}
      .hero p{color:var(--muted);max-width:620px;margin:0 auto 24px;font-size:1.05rem}
      .hero-actions{display:flex;justify-content:center;align-items:center;gap:10px;flex-wrap:wrap}
      .btn{
        display:inline-flex;align-items:center;justify-content:center;padding:14px 30px;border-radius:999px;
        font-size:.94rem;font-weight:700;background:linear-gradient(90deg,var(--navy),var(--teal));
        color:#fff;box-shadow:0 12px 30px rgba(20,124,120,.25);
        transition:transform .25s,box-shadow .25s;background-color:var(--navy);border:0;cursor:pointer;
      }
      .btn:hover{transform:translateY(-2px);box-shadow:0 16px 38px rgba(217,139,58,.20)}
      .btn-ghost{background:rgba(255,255,255,.62);color:var(--navy);border:1px solid var(--border);box-shadow:none}
      .btn-ghost:hover{background:#fff;box-shadow:0 14px 30px rgba(11,22,32,.08)}
      .trust{
        display:flex;justify-content:center;gap:40px;padding:20px;border-block:1px solid var(--border);
        background:rgba(255,255,255,.48);position:relative;z-index:2;
      }
      .trust-num{font-family:'Frank Ruhl Libre',serif;font-size:2.4rem;color:var(--teal);line-height:1;font-weight:800;text-align:center}
      .trust-label{font-size:.78rem;color:var(--muted);text-align:center;margin-top:2px;font-weight:500}
      .sec-title{text-align:center;margin-bottom:24px}
      .sec-title::before{content:"";display:block;width:44px;height:1px;background:var(--gold);margin:0 auto 14px}
      .sec-title h2{font-size:clamp(2.2rem,6.5vw,3.2rem);line-height:1.1}
      .sec-title p{color:var(--muted);font-size:.95rem;margin-top:6px}

      /* Gallery: visible even when JavaScript or animations are unavailable. */
      .gallery{padding:52px 0 20px;position:relative;z-index:2}
      .g-grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px}
      .g-item{position:relative;min-width:0;aspect-ratio:4/5}
      .g-item:first-child{grid-column:1/-1;aspect-ratio:16/10}
      .g-open{
        position:relative;display:block;width:100%;height:100%;overflow:hidden;
        border-radius:18px;border:1px solid var(--border);background:var(--bg-2);
        cursor:zoom-in;text-align:start;color:#fff;
        box-shadow:0 10px 28px rgba(11,22,32,.09);
        transition:transform .65s var(--ease),box-shadow .65s var(--ease);
        isolation:isolate;
      }
      .g-open:focus-visible{outline-offset:5px}
      .g-open img{
        display:block;width:100%;height:100%;object-fit:cover;
        transition:transform 1s var(--ease);
      }
      .g-caption{
        position:absolute;inset:auto 0 0;padding:48px 16px 14px;
        background:linear-gradient(transparent,rgba(11,22,32,.8));
        font-family:'Frank Ruhl Libre',serif;font-size:1.15rem;font-weight:700;
      }
      .g-zoom{
        position:absolute;top:12px;left:12px;width:38px;height:38px;
        display:grid;place-items:center;border-radius:50%;font-size:1.4rem;line-height:1;
        color:#fff;background:rgba(11,22,32,.55);border:1px solid rgba(255,255,255,.35);
        backdrop-filter:blur(6px);opacity:0;transform:translateY(6px);
        transition:opacity .35s,transform .5s var(--ease);
      }
      .g-open:focus-visible .g-zoom{opacity:1;transform:none}
      @media(hover:hover) and (pointer:fine){
        .g-open:hover{transform:translateY(-5px);box-shadow:0 22px 44px rgba(11,22,32,.16)}
        .g-open:hover img{transform:scale(1.055)}
        .g-open:hover .g-zoom{opacity:1;transform:none}
      }
      @media(hover:none){.g-zoom{opacity:1;transform:none}}
      .gallery-hint{text-align:center;color:var(--muted);font-size:.8rem;margin-top:18px}

      /* Native modal: keyboard focus stays inside while the gallery is open. */
      .layer{
        position:fixed;inset:0;width:100%;height:100%;height:100dvh;
        max-width:none;max-height:none;margin:0;padding:0;border:0;
        background:transparent;color:#fff;overflow:hidden;
      }
      .layer::backdrop{background:transparent}
      .layer[open]{display:block}
      .layer-shell{
        position:absolute;inset:0;display:flex;align-items:center;justify-content:center;
        background:radial-gradient(ellipse at 50% 25%,rgba(20,124,120,.17),transparent 60%),rgba(11,22,32,.96);
        -webkit-backdrop-filter:blur(12px);backdrop-filter:blur(12px);
      }
      .layer-stage{
        width:100%;height:100%;padding:82px 76px 32px;
        padding-top:max(82px,calc(env(safe-area-inset-top) + 62px));
        padding-bottom:max(32px,calc(env(safe-area-inset-bottom) + 20px));
        display:flex;align-items:center;justify-content:center;flex-direction:column;
        pointer-events:none;
      }
      .layer-visual{
        min-height:0;max-width:1100px;width:100%;flex:1;
        display:flex;align-items:center;justify-content:center;
      }
      .layer img{
        display:block;max-width:100%;max-height:100%;width:auto;height:auto;object-fit:contain;
        border-radius:16px;box-shadow:0 28px 90px rgba(0,0,0,.4);
        pointer-events:auto;touch-action:pan-y;user-select:none;
      }
      .layer img[hidden]{display:none}
      .layer-cap{text-align:center;margin-top:20px;flex-shrink:0}
      .layer-cap span{display:block;font-family:'Frank Ruhl Libre',serif;font-size:clamp(1.4rem,4vw,1.9rem);line-height:1.2}
      .layer-cap small{display:block;font-size:.82rem;color:rgba(255,255,255,.76);margin-top:6px}
      .layer-x,.layer-prev,.layer-next{
        position:absolute;z-index:3;width:48px;height:48px;display:grid;place-items:center;
        border-radius:50%;border:1px solid rgba(255,255,255,.25);color:#fff;
        background:rgba(255,255,255,.09);font-size:1.6rem;cursor:pointer;
        transition:background .25s,border-color .25s;
      }
      .layer-x:hover,.layer-prev:hover,.layer-next:hover{background:var(--teal);border-color:var(--teal)}
      .layer :focus-visible{outline-color:var(--gold-bright)}
      .layer-x{left:20px;top:max(18px,env(safe-area-inset-top))}
      .layer-prev{right:16px;top:50%;transform:translateY(-50%)}
      .layer-next{left:16px;top:50%;transform:translateY(-50%)}
      .layer-count{
        position:absolute;right:24px;top:max(28px,calc(env(safe-area-inset-top) + 10px));
        font-size:.85rem;letter-spacing:.12em;color:rgba(255,255,255,.8);
      }
      .layer-status{
        position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);
        max-width:75%;text-align:center;font-size:.9rem;pointer-events:none;
      }
      .layer-status:empty{display:none}
      @media(max-width:600px){
        .layer-stage{padding-inline:12px;padding-bottom:max(94px,calc(env(safe-area-inset-bottom) + 82px))}
        .layer-prev,.layer-next{top:auto;bottom:max(18px,env(safe-area-inset-bottom));transform:none}
        .layer-prev{right:calc(50% - 58px)}
        .layer-next{left:calc(50% - 58px)}
        .layer img{border-radius:12px}
        .layer-cap{margin-top:16px}
      }

      .menu{padding:40px 0 90px;position:relative;z-index:2}
      .acc{display:flex;flex-direction:column;gap:12px}
      .acc-item{
        background:var(--card);border:1px solid var(--border);border-radius:var(--radius);
        overflow:hidden;backdrop-filter:blur(8px);
        transition:border-color .3s,box-shadow .3s,transform .3s;
      }
      .acc-item:hover{border-color:rgba(20,124,120,.35)}
      .acc-item.open{border-color:rgba(20,124,120,.4);box-shadow:0 18px 44px rgba(11,22,32,.1);transform:translateY(-2px)}
      .acc-head{display:flex;align-items:center;justify-content:space-between;gap:14px;padding:20px 22px;cursor:pointer;user-select:none}
      .acc-head .num{font-size:.78rem;font-weight:700;color:var(--gold);min-width:30px}
      .acc-head .ttl{flex:1;min-width:0}
      .acc-head h3{font-size:clamp(1.45rem,5vw,1.9rem);line-height:1.15;transition:color .3s}
      .acc-item.open .acc-head h3{color:var(--teal)}
      .acc-head .sub{display:block;font-size:.82rem;color:var(--muted);margin-top:4px}
      .acc-icon{
        width:34px;height:34px;border-radius:50%;border:1px solid var(--border);
        display:flex;align-items:center;justify-content:center;color:var(--teal);font-size:1.3rem;
        transition:.35s;flex-shrink:0;background:#fff;line-height:1;
      }
      .acc-item.open .acc-icon{transform:rotate(45deg);background:var(--teal);color:#fff;border-color:var(--teal)}
      .acc-body{display:grid;grid-template-rows:0fr;transition:grid-template-rows .5s cubic-bezier(.4,0,.2,1)}
      .acc-item.open .acc-body{grid-template-rows:1fr}
      .acc-body>div{overflow:hidden}
      .acc-content{padding:0 22px 26px;opacity:0;transform:translateY(-8px);transition:.45s .1s}
      .acc-item.open .acc-content{opacity:1;transform:none}
      .acc-content p{color:var(--muted);margin-bottom:14px;font-size:.98rem}
      .acc-content .lede{font-family:'Frank Ruhl Libre',serif;font-size:1.55rem;line-height:1.3;color:var(--text);margin-bottom:14px;font-weight:700}
      .acc-content ul{list-style:none;display:grid;gap:8px;margin:6px 0 14px}
      .acc-content li{padding-right:18px;position:relative;color:var(--muted);font-size:.94rem}
      .acc-content li::before{content:"";width:7px;height:7px;border-radius:50%;background:var(--teal);position:absolute;right:0;top:.65em}
      .mini-grid{display:grid;gap:12px}
      .mini{background:#fff;border:1px solid var(--border);border-radius:16px;padding:18px}
      .mini .tag{font-size:.72rem;font-weight:700;color:var(--gold);display:block;margin-bottom:8px}
      .mini h4{font-size:1.45rem;line-height:1.15;margin-bottom:8px}
      .mini p{font-size:.92rem;margin-bottom:10px}
      .pills{display:flex;flex-wrap:wrap;gap:7px}
      .pill{font-size:.75rem;padding:5px 11px;border-radius:999px;background:var(--teal-soft);color:var(--navy);border:1px solid rgba(20,124,120,.22);font-weight:500}
      .steps{display:grid;gap:12px}
      .step{display:flex;gap:14px;align-items:flex-start}
      .step b{font-family:'Frank Ruhl Libre',serif;font-size:1.8rem;color:var(--gold);line-height:1;min-width:38px}
      .step h4{font-size:1.35rem;color:var(--navy);line-height:1.15}
      .step p{font-size:.92rem;margin:3px 0 0}
      .field{margin-bottom:14px}
      label{display:block;font-size:.8rem;color:var(--muted);margin-bottom:6px;font-weight:600}
      input,textarea{width:100%;border:1px solid var(--border);background:#fff;color:var(--text);border-radius:13px;padding:12px 14px;font-size:1rem}
      input:focus,textarea:focus{border-color:var(--teal)}
      .chips{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:16px}
      .chip{border:1px solid var(--border);background:#fff;color:var(--muted);border-radius:999px;padding:8px 15px;cursor:pointer;font-size:.82rem;transition:.25s}
      .chip.active,.chip:hover{color:var(--teal);border-color:var(--teal);background:var(--teal-soft)}
      footer{text-align:center;color:var(--muted);font-size:.82rem;padding:30px 22px 100px;position:relative;z-index:2}
      .tg{position:fixed;left:16px;bottom:16px;z-index:180}
      .tg-btn{
        width:56px;height:56px;border-radius:50%;border:0;cursor:pointer;
        background:linear-gradient(135deg,var(--navy),var(--teal));color:#fff;
        display:flex;align-items:center;justify-content:center;box-shadow:0 12px 34px rgba(20,124,120,.35);
        transition:transform .3s;animation:pulse 3s infinite;
      }
      @keyframes pulse{0%,100%{box-shadow:0 12px 34px rgba(20,124,120,.35)}50%{box-shadow:0 12px 44px rgba(198,161,91,.34)}}
      .tg-btn:hover{transform:scale(1.06)}
      .tg-pop{
        position:absolute;left:0;bottom:68px;min-width:230px;max-width:calc(100vw - 32px);
        background:#fff;border:1px solid var(--border);border-radius:16px;padding:14px 16px;
        box-shadow:0 20px 50px rgba(11,22,32,.14);opacity:0;visibility:hidden;
        transform:translateY(8px) scale(.96);pointer-events:none;transition:.3s;
      }
      .tg.open .tg-pop{opacity:1;visibility:visible;transform:none;pointer-events:auto}
      .tg-pop small{display:block;font-size:.72rem;color:var(--muted);margin-bottom:4px}
      .tg-pop .user{font-family:'Frank Ruhl Libre',serif;font-size:1.5rem;color:var(--navy);font-weight:700;line-height:1}
      .tg-pop a{display:inline-block;margin-top:10px;font-size:.82rem;font-weight:700;color:var(--teal)}

      @media(min-width:760px){
        .bg-fruit{
          width:42vw;height:100vh;opacity:.58;
          -webkit-mask-image:linear-gradient(270deg,#000 55%,transparent 100%);
          mask-image:linear-gradient(270deg,#000 55%,transparent 100%);
        }
        .container{margin-right:auto;margin-left:8vw}
        .hero{justify-content:flex-start;padding-left:8vw;text-align:right}
        .hero-actions{justify-content:flex-start}
        .hero p{margin-right:0}
        .hero-inner::before{right:110px;left:auto}
        .g-grid{grid-template-columns:repeat(3,minmax(0,1fr))}
        .g-item:first-child{grid-column:span 2;grid-row:span 2;aspect-ratio:auto}
        .mini-grid,.steps{grid-template-columns:1fr 1fr}
        .acc-head{padding:22px 26px}
        .acc-content{padding:0 26px 28px}
      }
      @media(min-width:1200px){
        .container{margin-left:auto;margin-right:46vw;max-width:760px}
        .hero{padding-left:22px}
      }
      @media(prefers-reduced-motion:reduce){
        html{scroll-behavior:auto}
        *,*::before,*::after{animation:none!important;transition:none!important}
        .g-open:hover,.g-open:hover img{transform:none}
      }
    </style>
  </head>
  <body>
    <div class="bg-fruit" aria-hidden="true"></div>

    <nav aria-label="ניווט ראשי">
      <img src="logo.png" alt="Refined Bar logo" width="38" height="38">
      <a href="#" class="brand" dir="ltr">Refined <span>Bar</span></a>
    </nav>

    <header class="hero">
      <div class="hero-inner">
        <div class="hero-logo-wrap">
          <img class="hero-logo" src="logo.png" alt="Refined Bar">
        </div>
        <div class="kicker">מיקסולוגיה פרימיום לאירועים עם אופי</div>
        <h1>בר קוקטיילים שנבנה<br><em>סביב האירוע שלכם.</em></h1>
        <p><strong>Refined Bar</strong> משתלב בתוך האירוע כחוויית מיקסולוגיה אישית: צוות מנוסה מאחורי הבר, תפריט שנבנה במיוחד עבורכם, התאמה לאווירה, לקהל, לעונה ולכל הפרטים הקטנים שעושים את ההבדל.</p>
        <div class="hero-actions">
          <a class="btn" href="#menu">לגלות את השירות ↓</a>
          <a class="btn btn-ghost" href="#gallery">לראות גלריה</a>
        </div>
      </div>
    </header>

    <div class="trust">
      <div>
        <div class="trust-num">14</div>
        <div class="trust-label">שנות ניסיון במיקסולוגיה ואירועים</div>
      </div>
      <div>
        <div class="trust-num" dir="ltr">360°</div>
        <div class="trust-label">התאמה מלאה לאופי האירוע</div>
      </div>
    </div>

    <section class="gallery" id="gallery" aria-labelledby="galleryTitle">
      <div class="container">
        <div class="sec-title">
          <h2 id="galleryTitle">משקאות שנראים כמו חלק מהאירוע</h2>
          <p>צבע, חומרי גלם, הגשה ואווירה — הכל נבנה כדי להשתלב בחוויה.</p>
        </div>

        <div class="g-grid" id="gGrid">
          <figure class="g-item" data-cap="Crimson Veil" data-sub="זכוכית סוכר · דובדבנים · נענע">
            <button class="g-open" type="button" aria-label="הגדלת תמונה: Crimson Veil" aria-haspopup="dialog" aria-controls="layer">
              <img src="gallery/crimson-veil.jpg" alt="Crimson Veil — קוקטייל של Refined Bar" loading="lazy" decoding="async">
              <span class="g-caption" dir="ltr">Crimson Veil</span>
              <span class="g-zoom" aria-hidden="true">+</span>
            </button>
          </figure>
          <figure class="g-item" data-cap="White Blossom" data-sub="קצף עדין · פרח מאכל · פטל">
            <button class="g-open" type="button" aria-label="הגדלת תמונה: White Blossom" aria-haspopup="dialog" aria-controls="layer">
              <img src="gallery/white-blossom.jpg" alt="White Blossom — קוקטייל של Refined Bar" loading="lazy" decoding="async">
              <span class="g-caption" dir="ltr">White Blossom</span>
              <span class="g-zoom" aria-hidden="true">+</span>
            </button>
          </figure>
          <figure class="g-item" data-cap="Rose Garden" data-sub="קצף ורוד · עלי ורדים · סחלב">
            <button class="g-open" type="button" aria-label="הגדלת תמונה: Rose Garden" aria-haspopup="dialog" aria-controls="layer">
              <img src="gallery/rose-garden.jpg" alt="Rose Garden — קוקטייל של Refined Bar" loading="lazy" decoding="async">
              <span class="g-caption" dir="ltr">Rose Garden</span>
              <span class="g-zoom" aria-hidden="true">+</span>
            </button>
          </figure>
          <figure class="g-item" data-cap="Golden Hour" data-sub="קרח צלול · קרמל · הדרים">
            <button class="g-open" type="button" aria-label="הגדלת תמונה: Golden Hour" aria-haspopup="dialog" aria-controls="layer">
              <img src="gallery/golden-hour.jpg" alt="Golden Hour — קוקטייל של Refined Bar" loading="lazy" decoding="async">
              <span class="g-caption" dir="ltr">Golden Hour</span>
              <span class="g-zoom" aria-hidden="true">+</span>
            </button>
          </figure>
          <figure class="g-item" data-cap="Evening Bloom" data-sub="מרטיני ענברי · פרח לבן">
            <button class="g-open" type="button" aria-label="הגדלת תמונה: Evening Bloom" aria-haspopup="dialog" aria-controls="layer">
              <img src="gallery/evening-bloom.jpg" alt="Evening Bloom — קוקטייל של Refined Bar" loading="lazy" decoding="async">
              <span class="g-caption" dir="ltr">Evening Bloom</span>
              <span class="g-zoom" aria-hidden="true">+</span>
            </button>
          </figure>
        </div>
        <p class="gallery-hint">לחצו להגדלה · החליקו בין התמונות בתצוגה המלאה</p>
      </div>
    </section>

    <section class="menu" id="menu">
      <div class="container">
        <div class="sec-title">
          <h2>השירות המרכזי שלנו</h2>
          <p>מיקסולוגיה פרימיום שמותאמת לאירוע, לאנשים ולאווירה.</p>
        </div>
        <div class="acc" id="acc">
          <div class="acc-item open">
            <div class="acc-head">
              <span class="num">01</span>
              <div class="ttl">
                <h3>מיקסולוגיה פרימיום לאירוע שלכם</h3>
                <span class="sub">בר שנבנה סביב האופי של האירוע</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <p class="lede">Refined Bar הוא לא רק בר שמגיע לאירוע — זו אינטגרציה של חוויית מיקסולוגיה לתוך האווירה, הקצב והאופי של הערב.</p>
              <p>אנחנו בונים עבורכם תפריט קוקטיילים אישי, כזה שלא מרגיש כמו תפריט מוכן מראש. כל משקה נבחר לפי סוג האירוע, העונה, הקהל, המקום, האוכל, הצבעים והתחושה שאתם רוצים ליצור.</p>
              <p>מאחורי הבר עומד צוות מנוסה שיודע לעבוד בצורה נקייה, רגועה ומדויקת — גם באירוע אינטימי וגם באירוע גדול. השירות נשאר נעים, הקצב נשאר נכון, והבר משתלב בתוך האירוע בלי למשוך אותו לכיוון לא מתאים.</p>
              <p>התוצאה היא חוויה שלא דומה לאף תפריט אחר: משקאות טעימים, אסתטיים, פוטוגניים ומדויקים לאנשים שמולם הם מוגשים.</p>
            </div></div></div>
          </div>

          <div class="acc-item">
            <div class="acc-head">
              <span class="num">02</span>
              <div class="ttl">
                <h3>איך הבר משתלב באירוע</h3>
                <span class="sub">מהרגע הראשון ועד הכוס האחרונה</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <p>לפני האירוע אנחנו מבינים את התמונה המלאה: מי האורחים, מה הסגנון, איפה האירוע מתקיים, מה מוגש באוכל, כמה אנשים צפויים להגיע ומה חשוב לכם שהאורחים ירגישו.</p>
              <p>על בסיס זה אנחנו בונים בר שמתאים לאירוע — לא רק מבחינת טעמים, אלא גם מבחינת נראות, קצב שירות, רמת אלכוהול, אפשרויות ללא אלכוהול והחוויה סביב העמדה.</p>
              <p>באירוע עצמו הבר הופך לנקודת מפגש טבעית: מקום שאנשים ניגשים אליו, טועמים משהו חדש, מצלמים, מדברים וחוזרים אליו במהלך הערב.</p>
              <p>המטרה היא שהבר לא ירגיש כמו תוספת חיצונית, אלא כמו חלק מדויק מהאירוע עצמו.</p>
            </div></div></div>
          </div>

          <div class="acc-item">
            <div class="acc-head">
              <span class="num">03</span>
              <div class="ttl">
                <h3>למי זה מתאים</h3>
                <span class="sub">מאירוח אינטימי ועד אירוע גדול</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <div class="mini-grid">
                <div class="mini">
                  <span class="tag">אירועים אינטימיים</span>
                  <h4>מארוחת ערב משפחתית ועד ערב חברים</h4>
                  <p>בר קוקטיילים אישי שמתאים לאירועים קטנים, ארוחות שף, ימי הולדת, אירוח ביתי, מסיבות גג וערבים שבהם רוצים להוסיף חוויה מיוחדת בלי להפוך את האירוע לרשמי מדי.</p>
                  <ul>
                    <li>תפריט מותאם לאורחים</li>
                    <li>קוקטיילים שמתאימים לאוכל ולאווירה</li>
                    <li>שירות רגוע ולא פולשני</li>
                    <li>אופציות אלכוהוליות וללא אלכוהול</li>
                  </ul>
                </div>
                <div class="mini">
                  <span class="tag">אירועים גדולים ובוטיק</span>
                  <h4>מחתונה ועד אירוע חברה</h4>
                  <p>פתרון מיקסולוגיה פרימיום לאירועים שבהם הבר צריך לעבוד יפה, מהר ומדויק — ועדיין להרגיש אישי, אסתטי ומחובר לאופי של האירוע.</p>
                  <ul>
                    <li>התאמה לכמות האורחים</li>
                    <li>צוות מנוסה מאחורי הבר</li>
                    <li>תפריט קוקטיילים ייחודי לאירוע</li>
                    <li>אפשרות לשפה ויזואלית מותאמת</li>
                  </ul>
                </div>
              </div>
            </div></div></div>
          </div>

          <div class="acc-item">
            <div class="acc-head">
              <span class="num">04</span>
              <div class="ttl">
                <h3>איך זה עובד</h3>
                <span class="sub">תהליך אישי, ברור ומדויק</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <div class="steps">
                <div class="step"><b>01</b><div>
                  <h4>היכרות עם האירוע</h4>
                  <p>מבינים את סוג האירוע, מספר האורחים, המיקום, האוכל, הסגנון והאווירה שאתם רוצים ליצור.</p>
                </div></div>
                <div class="step"><b>02</b><div>
                  <h4>בניית קונספט ותפריט</h4>
                  <p>יוצרים תפריט קוקטיילים אישי שמותאם לאירוע — בטעמים, בצבעים, בחומרי הגלם ובאופן ההגשה.</p>
                </div></div>
                <div class="step"><b>03</b><div>
                  <h4>הכנות ודיוק הפרטים</h4>
                  <p>מכינים מראש סירופים, קישוטים, פירות, קרח, ציוד וכל מה שנדרש כדי שהבר יעבוד חלק.</p>
                </div></div>
                <div class="step"><b>04</b><div>
                  <h4>אינטגרציה באירוע</h4>
                  <p>מקימים את הבר, משתלבים באווירה ומגישים לאורך הערב בצורה מקצועית, אסתטית ורגועה.</p>
                </div></div>
              </div>
            </div></div></div>
          </div>

          <div class="acc-item">
            <div class="acc-head">
              <span class="num">05</span>
              <div class="ttl">
                <h3>דוגמאות לקוקטיילים מותאמים</h3>
                <span class="sub">כל תפריט נבנה מחדש לפי האירוע</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <p class="lede">אלה רק דוגמאות לכיוון. בפועל, כל תפריט נבנה במיוחד עבור האירוע שלכם — לפי הטעם, העונה, האוכל והאווירה.</p>
              <div class="mini-grid">
                <div class="mini">
                  <span class="tag">מתוק · נוסטלגי · רך</span>
                  <h4 dir="ltr">Nostalgic Love</h4>
                  <p>קוקטייל מתוק, רך ונוסטלגי על בסיס רום לבן, תות וקורדיאל נענע, עם קצף רימונים אוורירי. מוגש לצד מרשמלו בננה ביתי — קטן, מפתיע ומאוד מצטלם.</p>
                  <div class="pills">
                    <span class="pill">רום לבן</span><span class="pill">תות</span>
                    <span class="pill">נענע</span><span class="pill">קצף רימונים</span>
                    <span class="pill">מרשמלו בננה</span>
                  </div>
                </div>
                <div class="mini">
                  <span class="tag">בוטני · אלגנטי · מיוחד</span>
                  <h4 dir="ltr">The Secret Garden</h4>
                  <p>קוקטייל בוטני ואלגנטי על בסיס ג׳ין, ליקר גזר, דבש, זרעי כוסברה ואלדרפלאוור. טעם מיוחד, לא כבד, ומתאים למי שאוהב קוקטיילים עם אופי.</p>
                  <div class="pills">
                    <span class="pill">ג׳ין</span><span class="pill">ליקר גזר</span>
                    <span class="pill">דבש</span><span class="pill">זרעי כוסברה</span>
                    <span class="pill">אלדרפלאוור</span>
                  </div>
                </div>
              </div>
            </div></div></div>
          </div>

          <div class="acc-item">
            <div class="acc-head">
              <span class="num">06</span>
              <div class="ttl">
                <h3>הערך שאתם מקבלים</h3>
                <span class="sub">מעבר לבר — חוויה שמרגישים וזוכרים</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <ul>
                <li>תפריט קוקטיילים שלא דומה לאף אירוע אחר</li>
                <li>צוות מנוסה שמחזיק את הבר בצורה רגועה ומקצועית</li>
                <li>התאמה עמוקה לאופי האירוע, לקהל, לאוכל ולעונה</li>
                <li>משקאות פוטוגניים שנראים טוב בתמונות וביד של האורחים</li>
                <li>אפשרויות אלכוהוליות וללא אלכוהול באותה רמת השקעה</li>
                <li>בר שמשתלב באירוע במקום להרגיש כמו תוספת חיצונית</li>
              </ul>
            </div></div></div>
          </div>

          <div class="acc-item">
            <div class="acc-head">
              <span class="num">07</span>
              <div class="ttl">
                <h3>נתחיל לבנות את הבר שלכם</h3>
                <span class="sub">ספרו לנו על האירוע ונחזור עם כיוון מותאם</span>
              </div>
              <span class="acc-icon" aria-hidden="true">+</span>
            </div>
            <div class="acc-body"><div><div class="acc-content">
              <p>אין צורך לדעת הכל מראש. מספיק לספר לנו תאריך, מיקום, כמות אורחים וסגנון כללי — ואנחנו נבנה יחד את הכיוון הנכון.</p>
              <form action="https://formsubmit.co/myasnikilya@gmail.com" method="POST">
                <input type="hidden" name="_subject" value="ליד חדש — Refined Bar">
                <input type="hidden" name="_captcha" value="false">
                <input type="hidden" name="interest" id="interestInput">
                <div class="chips" role="group" aria-label="סוג האירוע">
                  <button type="button" class="chip" aria-pressed="false">ארוחת ערב / אירוח ביתי</button>
                  <button type="button" class="chip" aria-pressed="false">אירוע פרטי</button>
                  <button type="button" class="chip" aria-pressed="false">חתונה</button>
                  <button type="button" class="chip" aria-pressed="false">יום הולדת</button>
                  <button type="button" class="chip" aria-pressed="false">אירוע חברה</button>
                  <button type="button" class="chip" aria-pressed="false">אחר</button>
                </div>
                <div class="field">
                  <label for="fname">שם</label>
                  <input id="fname" type="text" name="name" autocomplete="name" placeholder="איך קוראים לכם?" required>
                </div>
                <div class="field">
                  <label for="fphone">טלפון / וואטסאפ</label>
                  <input id="fphone" type="tel" name="phone" autocomplete="tel" dir="ltr" placeholder="050-0000000" required>
                </div>
                <div class="field">
                  <label for="fmsg">קצת על האירוע</label>
                  <textarea id="fmsg" name="message" rows="3" placeholder="תאריך, מיקום, מספר אורחים ומה הסגנון שאתם מחפשים"></textarea>
                </div>
                <button type="submit" class="btn">בדיקת התאמה וזמינות</button>
              </form>
            </div></div></div>
          </div>
        </div>
      </div>
    </section>

    <footer>© 2026 Refined Bar. כל הזכויות שמורות.</footer>

    <div class="tg" id="tg">
      <div class="tg-pop" id="tgPop">
        <small>לשיחה מהירה עם Refined Bar</small>
        <div class="user"><bdi>@MayIlyaa</bdi></div>
        <a href="https://t.me/MayIlyaa" target="_blank" rel="noopener noreferrer">פתיחת צ׳אט בטלגרם ←</a>
      </div>
      <button class="tg-btn" id="tgBtn" type="button" aria-label="יצירת קשר בטלגרם" aria-expanded="false" aria-controls="tgPop">
        <svg width="26" height="26" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M9.04 15.6l-.37 5.2c.53 0 .76-.23 1.04-.5l2.5-2.4 5.18 3.8c.95.52 1.63.25 1.88-.88l3.4-15.9c.3-1.4-.5-1.95-1.43-1.6L1.3 10.9c-1.36.53-1.34 1.29-.23 1.63l5.1 1.6L18.1 6.7c.56-.37 1.07-.17.65.2L9.04 15.6z"/></svg>
      </button>
    </div>

    <dialog class="layer" id="layer" aria-label="גלריית הקוקטיילים של Refined Bar">
      <div class="layer-shell" id="layerShell">
        <button class="layer-x" id="layerX" type="button" aria-label="סגירת הגלריה" autofocus>×</button>
        <div class="layer-count" id="layerCount" dir="ltr"></div>
        <button class="layer-prev" id="layerPrev" type="button" aria-label="התמונה הקודמת">›</button>
        <div class="layer-stage">
          <div class="layer-visual" id="layerVisual" aria-busy="false">
            <img id="layerImg" alt="" draggable="false" hidden>
          </div>
          <div class="layer-cap" id="layerCaption" aria-live="polite" aria-atomic="true">
            <span id="layerCap" dir="ltr"></span>
            <small id="layerSub"></small>
          </div>
        </div>
        <p class="layer-status" id="layerStatus" role="status"></p>
        <button class="layer-next" id="layerNext" type="button" aria-label="התמונה הבאה">‹</button>
      </div>
    </dialog>

    <script>
      (() => {
        'use strict';

        const reducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)');
        const ease = 'cubic-bezier(.22,1,.36,1)';
        const running = new Set();

        // No animation library needed. Cancel movement if the preference changes.
        function animate(element, keyframes, options = {}) {
          if (reducedMotion.matches || !element.animate) return Promise.resolve();
          const animation = element.animate(keyframes, {
            duration: 480, easing: ease, ...options
          });
          running.add(animation);
          return animation.finished.catch(() => {}).finally(() => {
            running.delete(animation);
          });
        }

        const cancelMotion = () => {
          if (reducedMotion.matches) running.forEach(animation => animation.cancel());
        };
        if (reducedMotion.addEventListener) {
          reducedMotion.addEventListener('change', cancelMotion);
        }

        // Existing accordion, with keyboard support.
        const acc = document.getElementById('acc');
        const panels = [...acc.querySelectorAll('.acc-item')];

        function setPanel(item, open) {
          item.classList.toggle('open', open);
          item.querySelector('.acc-head').setAttribute('aria-expanded', String(open));
          const body = item.querySelector('.acc-body');
          body.inert = !open;
          body.setAttribute('aria-hidden', String(!open));
        }

        panels.forEach((item, i) => {
          const head = item.querySelector('.acc-head');
          const body = item.querySelector('.acc-body');
          head.tabIndex = 0;
          head.setAttribute('role', 'button');
          body.id = `acc-panel-${i}`;
          head.setAttribute('aria-controls', body.id);
          setPanel(item, item.classList.contains('open'));
          head.addEventListener('keydown', event => {
            if (event.key === 'Enter' || event.key === ' ') {
              event.preventDefault();
              head.click();
            }
          });
        });

        acc.addEventListener('click', event => {
          const head = event.target.closest('.acc-head');
          if (!head) return;
          const item = head.parentElement;
          const wasOpen = item.classList.contains('open');
          panels.forEach(panel => setPanel(panel, panel === item && !wasOpen));
        });

        // Telegram.
        const tg = document.getElementById('tg');
        const tgBtn = document.getElementById('tgBtn');
        function setTelegram(open) {
          tg.classList.toggle('open', open);
          tgBtn.setAttribute('aria-expanded', String(open));
        }
        tgBtn.addEventListener('click', () => setTelegram(!tg.classList.contains('open')));
        document.addEventListener('click', event => {
          if (!tg.contains(event.target)) setTelegram(false);
        });
        tg.addEventListener('keydown', event => {
          if (event.key === 'Escape') {
            setTelegram(false);
            tgBtn.focus();
          }
        });

        // Form chips.
        const chips = [...document.querySelectorAll('.chip')];
        chips.forEach(chip => {
          chip.addEventListener('click', () => {
            chips.forEach(other => {
              const selected = other === chip;
              other.classList.toggle('active', selected);
              other.setAttribute('aria-pressed', String(selected));
            });
            document.getElementById('interestInput').value = chip.textContent.trim();
          });
        });

        // Gallery entrance. Each card appears once; no permanent hidden state.
        const items = [...document.querySelectorAll('.g-item')];
        if ('IntersectionObserver' in window) {
          const observer = new IntersectionObserver(entries => {
            let order = 0;
            entries.forEach(entry => {
              if (!entry.isIntersecting) return;
              observer.unobserve(entry.target);
              animate(entry.target, [
                { opacity: 0, transform: 'translateY(28px) scale(.985)' },
                { opacity: 1, transform: 'translateY(0) scale(1)' }
              ], { duration: 850, delay: order++ * 90, fill: 'backwards' });
            });
          }, { threshold: 0.08 });
          items.forEach(item => observer.observe(item));
        }

        const layer = document.getElementById('layer');
        const shell = document.getElementById('layerShell');
        const image = document.getElementById('layerImg');
        const visual = document.getElementById('layerVisual');
        const caption = document.getElementById('layerCaption');
        const cap = document.getElementById('layerCap');
        const sub = document.getElementById('layerSub');
        const counter = document.getElementById('layerCount');
        const status = document.getElementById('layerStatus');
        const closeButton = document.getElementById('layerX');
        const imageCache = new Map();

        let index = 0;
        let requestId = 0;
        let closing = false;
        let opener = null;
        let savedOverflow = '';
        let savedPadding = '';

        function loadImage(src) {
          if (imageCache.has(src)) return imageCache.get(src);
          const promise = new Promise((resolve, reject) => {
            const preload = new Image();
            preload.onload = () => resolve(preload);
            preload.onerror = () => reject(new Error('Image unavailable'));
            preload.src = src;
          });
          imageCache.set(src, promise);
          promise.catch(() => imageCache.delete(src));
          return promise;
        }

        function sourceAt(i) {
          const original = items[(i + items.length) % items.length].querySelector('img');
          return original.currentSrc || original.src;
        }

        async function showImage(nextIndex, direction = 0) {
          const ownRequest = ++requestId;
          index = (nextIndex + items.length) % items.length;
          const currentIndex = index;
          const item = items[currentIndex];
          const original = item.querySelector('img');

          image.getAnimations?.().forEach(animation => animation.cancel());
          caption.getAnimations?.().forEach(animation => animation.cancel());
          image.style.opacity = '0';
          cap.textContent = '';
          sub.textContent = '';
          status.textContent = 'טוען תמונה…';
          visual.setAttribute('aria-busy', 'true');
          counter.textContent = `${currentIndex + 1} / ${items.length}`;

          try {
            // Keep the old photo briefly while it fades, then show only the loaded one.
            await Promise.all([
              loadImage(sourceAt(currentIndex)),
              image.hidden ? Promise.resolve() : animate(image, [
                { opacity: 1, transform: 'translateX(0) scale(1)' },
                { opacity: 0, transform: `translateX(${-direction * 18}px) scale(.99)` }
              ], { duration: 150 })
            ]);

            if (ownRequest !== requestId || !layer.open || closing) return;

            image.src = sourceAt(currentIndex);
            image.alt = original.alt;
            image.hidden = false;
            image.style.opacity = '1';
            cap.textContent = item.dataset.cap || '';
            sub.textContent = item.dataset.sub || '';
            status.textContent = '';
            visual.setAttribute('aria-busy', 'false');

            animate(image, [
              { opacity: 0, transform: `translateX(${direction * 28}px) scale(.975)` },
              { opacity: 1, transform: 'translateX(0) scale(1)' }
            ], { duration: direction ? 450 : 620 });

            animate(caption, [
              { opacity: 0, transform: 'translateY(8px)' },
              { opacity: 1, transform: 'translateY(0)' }
            ], { duration: 420 });

            // Preload adjacent images after opening, not on initial page load.
            loadImage(sourceAt(currentIndex + 1)).catch(() => {});
            loadImage(sourceAt(currentIndex - 1)).catch(() => {});
          } catch {
            if (ownRequest !== requestId || !layer.open || closing) return;
            image.hidden = true;
            visual.setAttribute('aria-busy', 'false');
            status.textContent = 'לא ניתן לטעון את התמונה. אפשר לעבור לתמונה הבאה.';
          }
        }

        function openLayer(i, button) {
          if (layer.open || closing) return;
          // Fallback for browsers without the native dialog API.
          if (typeof layer.showModal !== 'function') {
            window.location.href = sourceAt(i);
            return;
          }
          opener = button;
          savedOverflow = document.body.style.overflow;
          savedPadding = document.body.style.paddingRight;
          const scrollbar = window.innerWidth - document.documentElement.clientWidth;
          if (scrollbar > 0) {
            const existingPadding = parseFloat(getComputedStyle(document.body).paddingRight) || 0;
            document.body.style.paddingRight = `${existingPadding + scrollbar}px`;
          }
          document.body.style.overflow = 'hidden';
          image.hidden = true;
          image.style.opacity = '0';
          setTelegram(false);
          layer.showModal();
          closeButton.focus({ preventScroll: true });
          animate(shell, [{ opacity: 0 }, { opacity: 1 }], { duration: 350 });
          showImage(i);
        }

        async function closeLayer() {
          if (!layer.open || closing) return;
          closing = true;
          requestId++;
          shell.getAnimations?.().forEach(animation => animation.cancel());
          await animate(shell, [{ opacity: 1 }, { opacity: 0 }], { duration: 220 });
          layer.close();
          document.body.style.overflow = savedOverflow;
          document.body.style.paddingRight = savedPadding;
          closing = false;
          opener?.focus({ preventScroll: true });
        }

        function move(direction) {
          if (!layer.open || closing) return;
          showImage(index + direction, direction);
        }

        items.forEach((item, i) => {
          const button = item.querySelector('.g-open');
          button.addEventListener('click', () => openLayer(i, button));
        });

        closeButton.addEventListener('click', closeLayer);
        document.getElementById('layerPrev').addEventListener('click', () => move(-1));
        document.getElementById('layerNext').addEventListener('click', () => move(1));
        shell.addEventListener('click', event => {
          if (event.target === shell) closeLayer();
        });

        layer.addEventListener('cancel', event => {
          event.preventDefault();
          closeLayer();
        });

        layer.addEventListener('keydown', event => {
          if (event.key === 'ArrowLeft') {
            event.preventDefault();
            move(1);
          } else if (event.key === 'ArrowRight') {
            event.preventDefault();
            move(-1);
          }
        });

        // Horizontal swipes only; do not capture vertical gestures or pinch zoom.
        let touchStart = null;
        image.addEventListener('touchstart', event => {
          touchStart = event.touches.length === 1
            ? { x: event.touches[0].clientX, y: event.touches[0].clientY }
            : null;
        }, { passive: true });

        image.addEventListener('touchmove', event => {
          if (event.touches.length !== 1) touchStart = null;
        }, { passive: true });

        image.addEventListener('touchend', event => {
          if (!touchStart || event.touches.length) {
            touchStart = null;
            return;
          }
          const touch = event.changedTouches[0];
          const dx = touch.clientX - touchStart.x;
          const dy = touch.clientY - touchStart.y;
          touchStart = null;
          if (Math.abs(dx) > 55 && Math.abs(dx) > Math.abs(dy) * 1.5) {
            move(dx < 0 ? 1 : -1);
          }
        }, { passive: true });

        image.addEventListener('touchcancel', () => { touchStart = null; }, { passive: true });
      })();
    </script>
  </body>
  </html>
