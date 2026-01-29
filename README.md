<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>HUSON DIGITA | Official Digital Services</title>
  <meta name="description" content="HUSON DIGITA — Streaming, gaming top-ups, gift cards, and social services. Pay with PayPal and confirm on WhatsApp."/>
  <style>
    :root{
      --bg:#07070b; --card:#0f0f18; --card2:#121220; --text:#f4f4f8; --muted:#b9b9c9;
      --line:#242436; --accent:#ff2b2b; --ok:#22c55e; --warn:#fbbf24;
      --shadow: 0 18px 60px rgba(0,0,0,.45);
      --r:18px; --max:1140px;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0; color:var(--text);
      font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,"Noto Sans Arabic","Noto Kufi Arabic",sans-serif;
      background:
        radial-gradient(900px 450px at 15% -10%, rgba(255,43,43,.22), transparent 60%),
        radial-gradient(700px 380px at 90% 10%, rgba(34,197,94,.14), transparent 60%),
        var(--bg);
      line-height:1.65;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max);margin:0 auto;padding:18px}
    header{
      position:sticky; top:0; z-index:50;
      background:rgba(7,7,11,.72);
      backdrop-filter: blur(10px);
      border-bottom:1px solid rgba(255,255,255,.06);
    }
    .nav{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:12px;min-width:240px}
    .logo{
      width:44px;height:44px;border-radius:14px;
      background:linear-gradient(135deg,var(--accent),#ff6b6b);
      display:grid;place-items:center;
      font-weight:1000; color:#170404;
      box-shadow:0 10px 32px rgba(255,43,43,.18);
      letter-spacing:.5px;
    }
    .brand .name{font-weight:1000}
    .brand .tag{font-size:12px;color:var(--muted)}
    nav.links{display:flex;gap:10px;flex-wrap:wrap;color:var(--muted);font-size:14px}
    nav.links a{padding:8px 10px;border-radius:12px}
    nav.links a:hover{background:rgba(255,255,255,.06);color:var(--text)}
    .actions{display:flex;gap:8px;flex-wrap:wrap;align-items:center;justify-content:flex-end}
    .btn{
      display:inline-flex;align-items:center;justify-content:center;gap:10px;
      padding:12px 14px;border-radius:14px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.06);
      font-weight:950;
      transition:.15s transform;
      user-select:none;
    }
    .btn:hover{transform:translateY(-1px)}
    .btn-primary{
      background:linear-gradient(135deg,var(--ok),#22c55e);
      color:#06110a;border-color:rgba(0,0,0,.08);
      box-shadow:0 18px 40px rgba(34,197,94,.16);
    }
    .btn-accent{
      background:linear-gradient(135deg,var(--accent),#ff6b6b);
      color:#1a0505;border-color:rgba(0,0,0,.08);
    }
    .pill{
      padding:8px 10px;border-radius:999px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.05);
      color:var(--muted); font-size:13px; font-weight:800;
    }
    .lang button{
      cursor:pointer;
      border-radius:999px;
      padding:8px 10px;
      background:rgba(255,255,255,.06);
      color:var(--text);
      border:1px solid rgba(255,255,255,.10);
      font-weight:900;
    }
    .lang button.active{
      border-color:rgba(34,197,94,.55);
      box-shadow:0 0 0 2px rgba(34,197,94,.16) inset;
    }

    .card{
      background:rgba(16,16,24,.92);
      border:1px solid rgba(255,255,255,.08);
      border-radius:var(--r);
      box-shadow:var(--shadow);
    }

    .hero{
      padding:20px 0 6px;
      display:grid;
      grid-template-columns: 1.1fr .9fr;
      gap:14px;
      align-items:stretch;
    }
    h1{margin:0 0 10px;font-size:clamp(28px,4vw,46px);line-height:1.12}
    .sub{margin:0;color:var(--muted);max-width:80ch}
    .badges{display:flex;gap:10px;flex-wrap:wrap;margin:14px 0 18px}
    .badge{
      font-size:13px;padding:8px 10px;border-radius:999px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.05);
    }
    .badge b{color:var(--ok)}
    .note{
      margin-top:12px;
      padding:12px 14px;
      border-radius:14px;
      background:rgba(255,255,255,.04);
      border:1px solid rgba(255,255,255,.08);
      color:var(--muted);
      font-size:13px;
    }
    .quick{
      padding:16px;
      display:flex;
      flex-direction:column;
      gap:12px;
      position:relative;
      overflow:hidden;
    }
    .quick:before{
      content:"";
      position:absolute; inset:-100px -80px auto auto;
      width:260px;height:260px;
      background: radial-gradient(circle at 35% 35%, rgba(255,43,43,.28), transparent 60%);
      transform: rotate(12deg);
    }
    .qrow{
      position:relative;
      display:flex;
      justify-content:space-between;
      gap:10px;
      padding:10px 12px;
      border-radius:14px;
      background:rgba(255,255,255,.04);
      border:1px solid rgba(255,255,255,.08);
      font-size:14px;
    }
    .qrow .tag{
      font-weight:1000;
      padding:4px 10px;
      border-radius:999px;
      background:rgba(34,197,94,.14);
      border:1px solid rgba(34,197,94,.18);
      color:#b8ffcf;
      white-space:nowrap;
    }

    section{padding:16px 0}
    .sectionTitle{
      display:flex;justify-content:space-between;gap:10px;align-items:end;flex-wrap:wrap;
      margin:0 0 12px;
    }
    .sectionTitle h2{margin:0;font-size:22px}
    .sectionTitle p{margin:0;color:var(--muted);font-size:14px}

    .filters{display:flex;gap:8px;flex-wrap:wrap;margin:10px 0 14px}
    .filters button{
      cursor:pointer;
      padding:10px 12px;border-radius:999px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.05);
      color:var(--text);
      font-weight:950;
    }
    .filters button.active{border-color:rgba(255,43,43,.55); box-shadow:0 0 0 2px rgba(255,43,43,.14) inset}

    .grid{display:grid;gap:14px;grid-template-columns:repeat(3,1fr)}
    .item{padding:16px;display:flex;flex-direction:column;gap:12px}
    .top{
      display:flex;align-items:center;justify-content:space-between;gap:12px
    }
    .svc{
      display:flex;align-items:center;gap:12px
    }
    .svcIcon{
      width:46px;height:46px;border-radius:16px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.06);
      display:grid;place-items:center;
      overflow:hidden;
      flex:0 0 auto;
    }
    .svcIcon img{width:100%;height:100%;object-fit:cover}
    .svcName{margin:0;font-size:16px;font-weight:1000}
    .svcDesc{margin:0;color:var(--muted);font-size:13px}
    .row{display:flex;gap:10px;flex-wrap:wrap;align-items:center;justify-content:space-between}
    select,input{
      background:rgba(255,255,255,.06);
      color:var(--text);
      border:1px solid rgba(255,255,255,.10);
      border-radius:12px;
      padding:10px 12px;
      outline:none;
    }
    .price{font-weight:1000}
    .hint{color:var(--muted);font-size:13px}

    details{
      border:1px solid rgba(255,255,255,.08);
      border-radius:14px;
      padding:12px;
      background:rgba(255,255,255,.04);
      margin:10px 0;
    }
    summary{cursor:pointer;font-weight:1000}
    details p{margin:8px 0 0;color:var(--muted);font-size:14px}

    .two{display:grid;grid-template-columns:1fr 1fr;gap:14px}
    .footer{
      border-top:1px solid rgba(255,255,255,.08);
      margin-top:16px;
      padding:18px 0 34px;
      color:var(--muted);
      font-size:13px;
    }
    .float{
      position:fixed; left:18px; bottom:18px; z-index:999;
      display:flex; gap:10px; align-items:center;
    }
    .bubble{
      padding:10px 12px;border-radius:999px;
      background:rgba(16,16,24,.92);
      border:1px solid rgba(255,255,255,.08);
      color:var(--muted);
      box-shadow:var(--shadow);
      font-size:13px;
    }

    @media (max-width: 980px){
      .hero{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr}
      nav.links{display:none}
      .two{grid-template-columns:1fr}
      .brand{min-width:auto}
    }
  </style>
</head>
<body>

<script>
  // ✅ Your info
  const BRAND = "HUSON DIGITA";
  const WHATSAPP_NUMBER = "212702855273";
  const PAYPAL_EMAIL = "onhicham48@gmail.com";

  // ✅ USD→MAD rate (edit anytime)
  const FX_USD_TO_MAD = 10.0;

  // ✅ Prices: put USD only (site shows USD + MAD automatically)
  // If price is 0 => PayPal button will be disabled.
  const PRICES = {
    // Streaming
    netflix: { m1: 0, m3: 0, m6: 0, m12: 0 },
    disney:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    shahid:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    osn:     { m1: 0, m3: 0, m6: 0, m12: 0 },
    prime:   { m1: 0, m3: 0, m6: 0, m12: 0 },
    appletv: { m1: 0, m3: 0, m6: 0, m12: 0 },
    crunchy: { m1: 0, m3: 0, m6: 0, m12: 0 },
    bein:    { m1: 0, m3: 0, m6: 0, m12: 0 },

    // Gaming
    psplus:  { m1: 0, m3: 0, m12: 0 },
    gamepass:{ m1: 0, m3: 0 },
    steam:   { m1: 0 },
    pubg:    { m1: 0 },
    freefire:{ m1: 0 },

    // Social (services on request)
    social:  { m1: 0 }
  };

  const DUR = {
    en:{m1:"1 month",m3:"3 months",m6:"6 months",m12:"12 months"},
    ar:{m1:"شهر",m3:"3 شهور",m6:"6 شهور",m12:"12 شهر"},
    dz:{m1:"شهر",m3:"3 شهور",m6:"6 شهور",m12:"12 شهر"},
  };

  // ✅ Small “images” (SVG icons) — no download needed
  function svgData(label, bg1, bg2){
    const svg = `
      <svg xmlns="http://www.w3.org/2000/svg" width="96" height="96">
        <defs>
          <linearGradient id="g" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0" stop-color="${bg1}"/>
            <stop offset="1" stop-color="${bg2}"/>
          </linearGradient>
        </defs>
        <rect rx="22" ry="22" x="0" y="0" width="96" height="96" fill="url(#g)"/>
        <text x="50%" y="56%" dominant-baseline="middle" text-anchor="middle"
              font-family="Arial" font-size="34" font-weight="900" fill="rgba(0,0,0,.75)">
          ${label}
        </text>
      </svg>`;
    return "data:image/svg+xml;charset=UTF-8," + encodeURIComponent(svg.trim());
  }

  const ICONS = {
    netflix:  svgData("N", "#ff2b2b", "#ff6b6b"),
    disney:   svgData("D+", "#2563eb", "#60a5fa"),
    shahid:   svgData("S", "#22c55e", "#86efac"),
    osn:      svgData("O", "#a855f7", "#e879f9"),
    prime:    svgData("P", "#0ea5e9", "#38bdf8"),
    appletv:  svgData("", "#94a3b8", "#e2e8f0"),
    crunchy:  svgData("C", "#f97316", "#fdba74"),
    bein:     svgData("be", "#7c3aed", "#c4b5fd"),
    psplus:   svgData("PS", "#2563eb", "#93c5fd"),
    gamepass: svgData("X", "#16a34a", "#86efac"),
    steam:    svgData("S", "#0f172a", "#64748b"),
    pubg:     svgData("UC", "#f59e0b", "#fde68a"),
    freefire: svgData("FF", "#ef4444", "#fca5a5"),
    social:   svgData("SM", "#14b8a6", "#99f6e4"),
  };

  const I18N = {
    en:{
      heroTitle:"Official Digital Services",
      heroSub:"Streaming • Gaming top-ups • Gift Cards • Social services — Pay with PayPal, confirm on WhatsApp.",
      official:"100% official services", fast:"Fast activation", secure:"Secure support", support:"WhatsApp support",
      cta1:"Order on WhatsApp", cta2:"View services",
      quick:"Quick offers (edit prices later)",
      services:"Services", pick:"Choose service + duration → Pay with PayPal → Confirm on WhatsApp.",
      duration:"Duration", price:"Price", pay:"Pay with PayPal", confirm:"Confirm on WhatsApp", tx:"Transaction ID (optional)",
      payments:"Payment methods", paymentsText:"PayPal (Visa/MasterCard) + WhatsApp support",
      how:"How it works", howText:"1) Choose service & duration  2) Pay with PayPal  3) Confirm on WhatsApp  4) We activate fast",
      trust:"Trust & policy", trustText:"We provide official services only. No hacked accounts. Support is available if any issue happens.",
      faq:"FAQ",
      faq1q:"Is it official?", faq1a:"Yes — official services only.",
      faq2q:"Activation time?", faq2a:"Usually 5–30 minutes depending on demand.",
      faq3q:"Refund / guarantee?", faq3a:"We clarify terms before payment and support you if there is an issue.",
      filterAll:"All", filterStreaming:"Streaming", filterGaming:"Gaming", filterSocial:"Social",
      supportTitle:"Need help?", supportText:"If you face any issue, contact WhatsApp support and we will help you.",
      noteNoHack:"⚠️ We do NOT sell hacked accounts or illegal access.",
      pricesNote:"Prices are placeholders now (0). Set USD prices in PRICES inside index.html.",
    },
    ar:{
      heroTitle:"خدمات رقمية رسمية",
      heroSub:"ستريمنغ • شحن الألعاب • كروت رقمية • خدمات السوشيال — أداء عبر بايبال وتأكيد عبر واتساب.",
      official:"خدمات رسمية 100%", fast:"تفعيل سريع", secure:"دعم آمن", support:"دعم واتساب",
      cta1:"اطلب عبر واتساب", cta2:"شوف الخدمات",
      quick:"عروض سريعة (غيّر الأثمنة من بعد)",
      services:"الخدمات", pick:"اختار الخدمة والمدة → خلّص ببايبال → أكد الطلب فالواتساب.",
      duration:"المدة", price:"الثمن", pay:"الأداء عبر PayPal", confirm:"تأكيد عبر WhatsApp", tx:"رقم العملية (اختياري)",
      payments:"طرق الدفع", paymentsText:"PayPal (Visa/MasterCard) + دعم واتساب",
      how:"كيفاش كنخدمو؟", howText:"1) كتختار الخدمة والمدة  2) كتخلص ببايبال  3) كتأكد فالواتساب  4) كنفعّلو بسرعة",
      trust:"الثقة والسياسة", trustText:"كنقدمو خدمات رسمية فقط. ماكيناش حسابات مهكرة. وإذا كان شي مشكل كنعاونوك فالدعم.",
      faq:"أسئلة شائعة",
      faq1q:"واش رسمي؟", faq1a:"نعم — خدمات رسمية فقط.",
      faq2q:"شحال كتاخد؟", faq2a:"غالباً بين 5 و30 دقيقة حسب الضغط.",
      faq3q:"ضمان/استرجاع؟", faq3a:"كنوضحوا الشروط قبل الأداء وأي مشكل كنحلوه عبر الدعم.",
      filterAll:"الكل", filterStreaming:"ستريمنغ", filterGaming:"ألعاب", filterSocial:"سوشيال",
      supportTitle:"باغي مساعدة؟", supportText:"إذا وقع شي مشكل فطلبك تواصل معنا فالواتساب وغادي نعاونك.",
      noteNoHack:"⚠️ ما كنبيعوش حسابات مهكرة ولا ولوج غير قانوني.",
      pricesNote:"الأثمنة دابا غير بلايص (0). عمّر أثمنة USD فـ PRICES داخل index.html.",
    },
    darija:{
      heroTitle:"خدمات رقمية ديال الثقة",
      heroSub:"Streaming • شحن الألعاب • Gift Cards • خدمات السوشيال — PayPal + تأكيد واتساب.",
      official:"رسمية 100%", fast:"تفعيل سريع", secure:"خدمة آمنة", support:"دعم واتساب",
      cta1:"طلب فواتساب", cta2:"شوف الخدمات",
      quick:"عروض سريعة (بدّل الثمن من بعد)",
      services:"Services", pick:"اختار الخدمة والمدة → خلّص بPayPal → أكد فالواتساب.",
      duration:"المدة", price:"الثمن", pay:"خلص بPayPal", confirm:"أكد فWhatsApp", tx:"Transaction ID (اختياري)",
      payments:"طرق الدفع", paymentsText:"PayPal (Visa/Master) + دعم واتساب",
      how:"كيفاش كنخدمو", howText:"1) تختار الخدمة والمدة  2) تخلص بPayPal  3) تأكيد فواتساب  4) كنفعّلو بسرعة",
      trust:"الثقة", trustText:"خدمات رسمية فقط ✅ ماشي مهكر. إلا وقع شي مشكل كنعاونوك فواتساب.",
      faq:"FAQ",
      faq1q:"واش رسمي؟", faq1a:"اييه ✅ خدمات رسمية فقط.",
      faq2q:"شحال كتاخد؟", faq2a:"غالباً 5–30 دقيقة.",
      faq3q:"ضمان؟", faq3a:"كنوضحوا الشروط قبل الأداء وأي مشكل كنحلوه فالدعم.",
      filterAll:"All", filterStreaming:"Streaming", filterGaming:"Gaming", filterSocial:"Social",
      supportTitle:"باغي تعاون؟", supportText:"إلى وقع شي مشكل فطلبك تواصل معنا فالواتساب وغادي نعاونك.",
      noteNoHack:"⚠️ ما كنبيعوش hacked accounts.",
      pricesNote:"الأثمنة دابا بلايص (0). عمّر ثمن USD فـ PRICES داخل index.html.",
    }
  };

  let LANG = "darija";
  let FILTER = "all";

  const SERVICES = [
    // Streaming
    {key:"netflix",  name:"Netflix",      cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"disney",   name:"Disney+",      cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"shahid",   name:"Shahid VIP",   cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"osn",      name:"OSN+",         cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"prime",    name:"Prime Video",  cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"appletv",  name:"Apple TV+",    cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"crunchy",  name:"Crunchyroll",  cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},
    {key:"bein",     name:"beIN CONNECT", cat:"streaming", desc_en:"Official subscription", desc_ar:"اشتراك رسمي", desc_dz:"اشتراك رسمي"},

    // Gaming
    {key:"psplus",   name:"PlayStation Plus", cat:"gaming", desc_en:"Subscription / top-up", desc_ar:"اشتراك/شحن", desc_dz:"اشتراك/شحن"},
    {key:"gamepass", name:"Xbox Game Pass",   cat:"gaming", desc_en:"Subscription",         desc_ar:"اشتراك",     desc_dz:"اشتراك"},
    {key:"steam",    name:"Steam Wallet",     cat:"gaming", desc_en:"Top-up",               desc_ar:"شحن",        desc_dz:"شحن"},
    {key:"pubg",     name:"PUBG UC",          cat:"gaming", desc_en:"Top-up",               desc_ar:"شحن",        desc_dz:"شحن"},
    {key:"freefire", name:"Free Fire Diamonds",cat:"gaming",desc_en:"Top-up",               desc_ar:"شحن",        desc_dz:"شحن"},

    // Social (on request)
    {key:"social",   name:"Social Services",  cat:"social", desc_en:"On request (ask details)", desc_ar:"حسب الطلب (سولنا)", desc_dz:"حسب الطلب (سولنا)"},
  ];

  const t = (k)=> (I18N[LANG] && I18N[LANG][k]) || I18N.en[k] || k;

  function setDir(){
    document.documentElement.lang = (LANG==="en") ? "en" : "ar";
    document.documentElement.dir  = (LANG==="en") ? "ltr" : "rtl";
  }

  function paypalBuyNow(itemName, amountUSD){
    const params = new URLSearchParams({
      cmd:"_xclick",
      business: PAYPAL_EMAIL,
      item_name: itemName,
      amount: String(amountUSD || 0),
      currency_code:"USD",
      no_note:"1"
    });
    return "https://www.paypal.com/cgi-bin/webscr?" + params.toString();
  }

  function waGlobal(){
    const msg = `Salam/Hi 👋\nI want to order from ${BRAND}.\nPlease send me today's prices.`;
    return "https://wa.me/" + WHATSAPP_NUMBER + "?text=" + encodeURIComponent(msg);
  }

  function waConfirm(serviceName, durationLabel, txid){
    const msg =
`Salam/Hi 👋
Order confirmation:
- Brand: ${BRAND}
- Service: ${serviceName}
- Duration: ${durationLabel}
- Payment: PayPal
- Transaction ID: ${txid || "N/A"}
(Please activate / deliver)`;
    return "https://wa.me/" + WHATSAPP_NUMBER + "?text=" + encodeURIComponent(msg);
  }

  function formatPrice(usd){
    if (!usd || usd<=0) return "XX";
    const mad = Math.round(usd * FX_USD_TO_MAD);
    return `$${usd}  •  ${mad} MAD`;
  }

  function renderStatic(){
    setDir();
    document.querySelectorAll("[data-i18n]").forEach(el=>{
      el.textContent = t(el.getAttribute("data-i18n"));
    });

    document.querySelectorAll("[data-lang]").forEach(btn=>{
      btn.classList.toggle("active", btn.getAttribute("data-lang")===LANG);
    });

    document.querySelectorAll("[data-filter]").forEach(btn=>{
      btn.classList.toggle("active", btn.getAttribute("data-filter")===FILTER);
    });

    document.querySelectorAll("[data-wa-global]").forEach(a=>{
      a.href = waGlobal(); a.target="_blank"; a.rel="noopener";
    });

    document.getElementById("yr").textContent = new Date().getFullYear();
  }

  function renderServices(){
    const grid = document.getElementById("cards");
    grid.innerHTML = "";

    const list = SERVICES.filter(s => FILTER==="all" ? true : s.cat===FILTER);

    list.forEach(svc=>{
      const durKeys = Object.keys(PRICES[svc.key] || {});
      const card = document.createElement("div");
      card.className = "card item";
      card.setAttribute("data-cat", svc.cat);

      const top = document.createElement("div");
      top.className = "top";

      const left = document.createElement("div");
      left.className = "svc";

      const icon = document.createElement("div");
      icon.className = "svcIcon";
      const img = document.createElement("img");
      img.alt = svc.name;
      img.src = ICONS[svc.key] || svgData("HD","#ff2b2b","#ff6b6b");
      icon.appendChild(img);

      const meta = document.createElement("div");
      const name = document.createElement("div");
      name.className = "svcName";
      name.textContent = svc.name;

      const desc = document.createElement("div");
      desc.className = "svcDesc";
      desc.textContent =
        (LANG==="en") ? svc.desc_en :
        (LANG==="ar") ? svc.desc_ar : svc.desc_dz;

      meta.appendChild(name);
      meta.appendChild(desc);

      left.appendChild(icon);
      left.appendChild(meta);

      const catPill = document.createElement("div");
      catPill.className = "pill";
      catPill.textContent =
        svc.cat==="streaming" ? t("filterStreaming") :
        svc.cat==="gaming" ? t("filterGaming") : t("filterSocial");

      top.appendChild(left);
      top.appendChild(catPill);

      const row = document.createElement("div");
      row.className = "row";

      const hint = document.createElement("div");
      hint.className = "hint";
      hint.textContent = t("duration")+":";

      const sel = document.createElement("select");
      sel.id = "dur_"+svc.key;

      // if service has no durations configured, show message
      if (!durKeys.length){
        const opt = document.createElement("option");
        opt.value = "m1";
        opt.textContent = (LANG==="en") ? "Contact us" : (LANG==="ar" ? "تواصل معنا" : "تواصل معنا");
        sel.appendChild(opt);
      }else{
        durKeys.forEach(k=>{
          const opt = document.createElement("option");
          const label = (LANG==="en") ? (DUR.en[k]||k) : (LANG==="ar" ? (DUR.ar[k]||DUR.en[k]||k) : (DUR.dz[k]||DUR.en[k]||k));
          opt.value = k;
          opt.textContent = label;
          sel.appendChild(opt);
        });
      }

      const price = document.createElement("div");
      price.className = "price";
      price.id = "price_"+svc.key;

      row.appendChild(hint);
      row.appendChild(sel);
      row.appendChild(price);

      const tx = document.createElement("input");
      tx.placeholder = t("tx");
      tx.id = "tx_"+svc.key;
      tx.style.width = "100%";

      const actions = document.createElement("div");
      actions.className = "row";

      const pay = document.createElement("a");
      pay.className = "btn btn-accent";
      pay.textContent = t("pay");
      pay.target="_blank"; pay.rel="noopener";

      const confirm = document.createElement("a");
      confirm.className = "btn btn-primary";
      confirm.textContent = t("confirm");
      confirm.target="_blank"; confirm.rel="noopener";

      function update(){
        const dk = sel.value;
        const usd = (PRICES[svc.key] && PRICES[svc.key][dk]) ? PRICES[svc.key][dk] : 0;
        price.textContent = formatPrice(usd);

        const durLabelEn = DUR.en[dk] || dk;
        const durLabel = (LANG==="en") ? durLabelEn : (LANG==="ar" ? (DUR.ar[dk]||durLabelEn) : (DUR.dz[dk]||durLabelEn));

        // PayPal link
        if (usd>0){
          pay.href = paypalBuyNow(`${BRAND} - ${svc.name} (${durLabelEn})`, usd);
          pay.style.opacity = "1";
          pay.style.pointerEvents = "auto";
        }else{
          pay.href = "#";
          pay.style.opacity = ".55";
          pay.style.pointerEvents = "none";
        }

        // WhatsApp confirm always works
        confirm.href = waConfirm(svc.name, durLabel, tx.value.trim());
      }

      sel.addEventListener("change", update);
      tx.addEventListener("input", update);

      actions.appendChild(pay);
      actions.appendChild(confirm);

      card.appendChild(top);
      card.appendChild(row);
      card.appendChild(tx);
      card.appendChild(actions);

      grid.appendChild(card);
      update();
    });
  }

  function setLang(newLang){
    LANG = newLang;
    renderStatic();
    renderServices();
  }

  function setFilter(newFilter){
    FILTER = newFilter;
    renderStatic();
    renderServices();
  }

  document.addEventListener("DOMContentLoaded", ()=>{
    // default
    setLang("darija");

    document.querySelectorAll("[data-lang]").forEach(btn=>{
      btn.addEventListener("click", ()=> setLang(btn.getAttribute("data-lang")));
    });

    document.querySelectorAll("[data-filter]").forEach(btn=>{
      btn.addEventListener("click", ()=> setFilter(btn.getAttribute("data-filter")));
    });
  });
</script>

<header>
  <div class="wrap nav">
    <div class="brand">
      <div class="logo">HD</div>
      <div>
        <div class="name">HUSON DIGITA</div>
        <div class="tag">PayPal payment • WhatsApp support • Morocco 🇲🇦</div>
      </div>
    </div>

    <nav class="links">
      <a href="#services" data-i18n="services">Services</a>
      <a href="#how" data-i18n="how">How</a>
      <a href="#faq" data-i18n="faq">FAQ</a>
    </nav>

    <div class="actions">
      <div class="lang">
        <button type="button" data-lang="darija" class="active">Darija</button>
        <button type="button" data-lang="ar">عربية</button>
        <button type="button" data-lang="en">English</button>
      </div>
      <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">Order on WhatsApp</a>
    </div>
  </div>
</header>

<main class="wrap">
  <section class="hero">
    <div class="card" style="padding:18px">
      <h1 data-i18n="heroTitle">Official Digital Services</h1>
      <p class="sub" data-i18n="heroSub">Streaming • Gaming top-ups • Gift cards • Social services — PayPal + WhatsApp.</p>

      <div class="badges">
        <div class="badge">✅ <b data-i18n="official">100% official services</b></div>
        <div class="badge">⚡ <span data-i18n="fast">Fast activation</span></div>
        <div class="badge">🔒 <span data-i18n="secure">Secure support</span></div>
        <div class="badge">💬 <span data-i18n="support">WhatsApp support</span></div>
      </div>

      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">Order on WhatsApp</a>
        <a class="btn" href="#services" data-i18n="cta2">View services</a>
      </div>

      <div class="note" data-i18n="pick">
        Choose service + duration → Pay with PayPal → Confirm on WhatsApp.
      </div>

      <div class="note" style="border-color:rgba(251,191,36,.22); color:#ffe7b3">
        <span data-i18n="noteNoHack">⚠️ We do NOT sell hacked accounts or illegal access.</span>
      </div>
    </div>

    <aside class="card quick">
      <div style="position:relative">
        <div style="color:var(--muted);font-size:14px;font-weight:1000" data-i18n="quick">Quick offers (edit prices later)</div>
      </div>
      <div class="qrow"><div><b>Netflix</b> Premium</div><div class="tag">USD + MAD</div></div>
      <div class="qrow"><div><b>Shahid</b> VIP</div><div class="tag">PayPal</div></div>
      <div class="qrow"><div><b>PS Plus</b></div><div class="tag">Fast</div></div>
      <div class="qrow"><div><b>Gaming</b> Top-ups</div><div class="tag">Support</div></div>

      <div style="display:flex;gap:10px;flex-wrap:wrap;position:relative">
        <a class="btn btn-primary" data-wa-global href="#">WhatsApp</a>
        <a class="btn" href="#how" data-i18n="how">How</a>
      </div>

      <div class="note" data-i18n="pricesNote">Prices are placeholders now (0). Set USD prices in PRICES inside index.html.</div>
    </aside>
  </section>

  <section id="services">
    <div class="sectionTitle">
      <h2 data-i18n="services">Services</h2>
      <p data-i18n="pick">Choose service + duration → Pay with PayPal → Confirm on WhatsApp.</p>
    </div>

    <div class="filters">
      <button type="button" data-filter="all" class="active" data-i18n="filterAll">All</button>
      <button type="button" data-filter="streaming" data-i18n="filterStreaming">Streaming</button>
      <button type="button" data-filter="gaming" data-i18n="filterGaming">Gaming</button>
      <button type="button" data-filter="social" data-i18n="filterSocial">Social</button>
    </div>

    <div class="grid" id="cards"></div>
  </section>

  <section class="two">
    <div class="card" style="padding:16px">
      <div class="sectionTitle" style="margin:0 0 10px">
        <h2 data-i18n="payments">Payment methods</h2>
        <p style="color:var(--muted)">Secure</p>
      </div>
      <p class="sub" style="margin:0" data-i18n="paymentsText">PayPal (Visa/MasterCard) + WhatsApp support</p>
      <div class="badges" style="margin-top:12px">
        <div class="badge">💳 Visa</div>
        <div class="badge">💳 MasterCard</div>
        <div class="badge">🅿️ PayPal</div>
        <div class="badge">📲 WhatsApp</div>
      </div>
      <div class="note">💱 FX: 1 USD ≈ <b id="fx"></b> MAD</div>
      <script>document.addEventListener("DOMContentLoaded",()=>{document.getElementById("fx").textContent = String(FX_USD_TO_MAD);});</script>
    </div>

    <div class="card" style="padding:16px" id="how">
      <div class="sectionTitle" style="margin:0 0 10px">
        <h2 data-i18n="how">How it works</h2>
        <p>PayPal → WhatsApp → Activation</p>
      </div>
      <div class="note" id="howText" data-i18n="howText">
        1) Choose service & duration  2) Pay with PayPal  3) Confirm on WhatsApp  4) We activate fast
      </div>
      <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">Order on WhatsApp</a>
        <a class="btn" href="#services" data-i18n="services">Services</a>
      </div>
    </div>
  </section>

  <section>
    <div class="sectionTitle">
      <h2 data-i18n="trust">Trust & policy</h2>
      <p>Clear terms</p>
    </div>
    <div class="card" style="padding:16px">
      <div class="sub" data-i18n="trustText">
        We provide official services only. No hacked accounts. Support is available if any issue happens.
      </div>
      <div class="note" style="margin-top:12px">
        ✅ Official services • 🔒 Privacy respected • 💬 Support via WhatsApp
      </div>
    </div>
  </section>

  <section id="faq">
    <div class="sectionTitle">
      <h2 data-i18n="faq">FAQ</h2>
      <p>Quick answers</p>
    </div>
    <div class="card" style="padding:16px">
      <details>
        <summary data-i18n="faq1q">Is it official?</summary>
        <p data-i18n="faq1a">Yes — official services only.</p>
      </details>
      <details>
        <summary data-i18n="faq2q">Activation time?</summary>
        <p data-i18n="faq2a">Usually 5–30 minutes depending on demand.</p>
      </details>
      <details>
        <summary data-i18n="faq3q">Refund / guarantee?</summary>
        <p data-i18n="faq3a">We clarify terms before payment and support you if there is an issue.</p>
      </details>

      <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">Order on WhatsApp</a>
        <a class="btn" href="#services" data-i18n="services">Services</a>
      </div>
    </div>
  </section>

  <section>
    <div class="sectionTitle">
      <h2 data-i18n="supportTitle">Need help?</h2>
      <p>Support</p>
    </div>
    <div class="card" style="padding:16px">
      <div class="sub" data-i18n="supportText">If you face any issue, contact WhatsApp support and we will help you.</div>
      <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#">WhatsApp Support</a>
        <span class="pill">+212 702 855 273</span>
      </div>
    </div>
  </section>

  <div class="footer">
    <div style="display:flex;gap:12px;flex-wrap:wrap;align-items:center;justify-content:space-between">
      <div><b>HUSON DIGITA</b> • © <span id="yr"></span><br/><span>Digital services • Morocco</span></div>
      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn" data-wa-global href="#">WhatsApp</a>
        <a class="btn" href="#services">Services</a>
        <a class="btn" href="#faq">FAQ</a>
      </div>
    </div>
  </div>
</main>

<div class="float">
  <div class="bubble">Need help? بغيتي تعاون؟</div>
  <a class="btn btn-primary" data-wa-global href="#">WhatsApp 💬</a>
</div>

</body>
</html>
