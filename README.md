<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>HUSON DIGITAL | IPTV & Digital Services</title>
  <meta name="description" content="HUSON DIGITAL — IPTV, Streaming, Gaming top-ups, and Social services. Pay with PayPal and confirm on WhatsApp."/>
  <style>
    :root{
      --bg:#05070c;
      --card:rgba(12,16,26,.92);
      --card2:rgba(16,21,34,.92);
      --text:#f3f6ff;
      --muted:#aeb8d7;
      --line:rgba(255,255,255,.08);
      --blue:#2b7cff;
      --blue2:#60a5fa;
      --ok:#22c55e;
      --warn:#fbbf24;
      --shadow:0 18px 60px rgba(0,0,0,.55);
      --r:18px;
      --max:1160px;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,"Noto Sans Arabic","Noto Kufi Arabic",sans-serif;
      color:var(--text);
      background:
        radial-gradient(1000px 520px at 10% -10%, rgba(43,124,255,.25), transparent 60%),
        radial-gradient(700px 420px at 95% 10%, rgba(96,165,250,.18), transparent 60%),
        radial-gradient(900px 520px at 50% 120%, rgba(34,197,94,.12), transparent 60%),
        var(--bg);
      line-height:1.65;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max);margin:0 auto;padding:18px}
    header{
      position:sticky;top:0;z-index:50;
      background:rgba(5,7,12,.72);
      backdrop-filter: blur(10px);
      border-bottom:1px solid rgba(255,255,255,.06);
    }
    .nav{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .brand{display:flex;align-items:center;gap:12px;min-width:260px}
    .mark{
      width:46px;height:46px;border-radius:16px;
      background:linear-gradient(135deg, rgba(43,124,255,1), rgba(96,165,250,1));
      display:grid;place-items:center;
      box-shadow:0 16px 40px rgba(43,124,255,.22);
      border:1px solid rgba(255,255,255,.10);
    }
    .mark svg{filter:drop-shadow(0 8px 18px rgba(0,0,0,.35))}
    .name{font-weight:1000;letter-spacing:.4px}
    .tag{font-size:12px;color:var(--muted)}
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
      transition:.15s transform, .15s filter;
      user-select:none;
    }
    .btn:hover{transform:translateY(-1px);filter:brightness(1.03)}
    .btn-primary{
      background:linear-gradient(135deg,var(--ok),#16a34a);
      color:#06110a;border-color:rgba(0,0,0,.08);
      box-shadow:0 18px 40px rgba(34,197,94,.16);
    }
    .btn-blue{
      background:linear-gradient(135deg,var(--blue),var(--blue2));
      color:#061022;border-color:rgba(0,0,0,.08);
      box-shadow:0 18px 40px rgba(43,124,255,.18);
    }
    .btn-ghost{background:rgba(255,255,255,.06)}
    .pill{
      padding:8px 10px;border-radius:999px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.05);
      color:var(--muted); font-size:13px; font-weight:900;
    }
    .lang button{
      cursor:pointer;border-radius:999px;padding:8px 10px;
      background:rgba(255,255,255,.06);color:var(--text);
      border:1px solid rgba(255,255,255,.10);font-weight:900;
    }
    .lang button.active{
      border-color:rgba(43,124,255,.65);
      box-shadow:0 0 0 2px rgba(43,124,255,.18) inset;
    }

    .card{
      background:var(--card);
      border:1px solid rgba(255,255,255,.08);
      border-radius:var(--r);
      box-shadow:var(--shadow);
    }
    .hero{
      padding:18px 0 6px;
      display:grid;
      grid-template-columns: 1.1fr .9fr;
      gap:14px;
      align-items:stretch;
    }
    .heroMain{padding:18px; position:relative; overflow:hidden}
    .heroMain:before{
      content:"";
      position:absolute; inset:-120px -80px auto auto;
      width:320px;height:320px;
      background:radial-gradient(circle at 30% 30%, rgba(43,124,255,.35), transparent 60%);
      transform:rotate(12deg);
    }
    h1{margin:0 0 10px;font-size:clamp(28px,4vw,46px);line-height:1.12; position:relative}
    .sub{margin:0;color:var(--muted);max-width:85ch; position:relative}
    .badges{display:flex;gap:10px;flex-wrap:wrap;margin:14px 0 18px; position:relative}
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
      position:relative;
    }
    .noteBlue{border-color:rgba(43,124,255,.22)}
    .noteWarn{border-color:rgba(251,191,36,.22); color:#ffe7b3}
    .side{padding:16px; display:flex; flex-direction:column; gap:12px; position:relative; overflow:hidden}
    .side:before{
      content:"";
      position:absolute; inset:-120px auto auto -80px;
      width:320px;height:320px;
      background:radial-gradient(circle at 30% 30%, rgba(96,165,250,.22), transparent 60%);
      transform:rotate(-8deg);
    }
    .kpiRow{
      position:relative;
      display:flex; justify-content:space-between; align-items:center; gap:10px;
      padding:10px 12px;
      border-radius:14px;
      background:rgba(255,255,255,.04);
      border:1px solid rgba(255,255,255,.08);
      font-size:14px;
    }
    .kpiRow .k{font-weight:1000}
    .kpiRow .v{font-weight:1000; color:#cfe3ff; background:rgba(43,124,255,.16); border:1px solid rgba(43,124,255,.18); padding:4px 10px; border-radius:999px; white-space:nowrap}

    section{padding:16px 0}
    .sectionTitle{
      display:flex;justify-content:space-between;gap:10px;align-items:end;flex-wrap:wrap;
      margin:0 0 12px;
    }
    .sectionTitle h2{margin:0;font-size:22px}
    .sectionTitle p{margin:0;color:var(--muted);font-size:14px}

    .grid{display:grid;gap:14px;grid-template-columns:repeat(3,1fr)}
    .item{padding:16px;display:flex;flex-direction:column;gap:12px; position:relative; overflow:hidden}
    .item:before{
      content:"";
      position:absolute; inset:auto -120px -120px auto;
      width:260px;height:260px;
      background:radial-gradient(circle at 35% 35%, rgba(43,124,255,.18), transparent 60%);
      transform:rotate(10deg);
      pointer-events:none;
    }
    .top{display:flex;align-items:center;justify-content:space-between;gap:12px; position:relative}
    .svc{display:flex;align-items:center;gap:12px}
    .svcIcon{
      width:48px;height:48px;border-radius:16px;
      border:1px solid rgba(255,255,255,.10);
      background:rgba(255,255,255,.06);
      display:grid;place-items:center;
      overflow:hidden; flex:0 0 auto;
    }
    .svcIcon img{width:100%;height:100%;object-fit:cover}
    .svcName{margin:0;font-size:16px;font-weight:1000}
    .svcDesc{margin:0;color:var(--muted);font-size:13px}
    .row{display:flex;gap:10px;flex-wrap:wrap;align-items:center;justify-content:space-between; position:relative}
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
    .mini{display:flex;gap:8px;flex-wrap:wrap; align-items:center}
    .mini .pill{font-size:12px}

    .two{display:grid;grid-template-columns:1fr 1fr;gap:14px}
    details{
      border:1px solid rgba(255,255,255,.08);
      border-radius:14px;
      padding:12px;
      background:rgba(255,255,255,.04);
      margin:10px 0;
    }
    summary{cursor:pointer;font-weight:1000}
    details p{margin:8px 0 0;color:var(--muted);font-size:14px}

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
      background:rgba(12,16,26,.92);
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
  // ====== YOUR INFO ======
  const BRAND = "HUSON DIGITAL";
  const WHATSAPP_NUMBER = "212702855273";
  const PAYPAL_EMAIL = "onhicham48@gmail.com";

  // USD → MAD rate (edit anytime)
  const FX_USD_TO_MAD = 10.0;

  // ====== PRICES (USD only) ======
  // Put your real prices later. If price is 0 => PayPal is disabled (to avoid wrong payments).
  const PRICES = {
    // IPTV (device selection shown)
    iptv_premium: { m1: 0, m3: 0, m6: 0, m12: 0 },
    iptv_4k:      { m1: 0, m3: 0, m6: 0, m12: 0 },
    iptv_sports:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    iptv_movies:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    iptv_series:  { m1: 0, m3: 0, m6: 0, m12: 0 },

    // Streaming
    netflix:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    disney:   { m1: 0, m3: 0, m6: 0, m12: 0 },
    shahid:   { m1: 0, m3: 0, m6: 0, m12: 0 },
    osn:      { m1: 0, m3: 0, m6: 0, m12: 0 },
    prime:    { m1: 0, m3: 0, m6: 0, m12: 0 },
    appletv:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    crunchy:  { m1: 0, m3: 0, m6: 0, m12: 0 },
    bein:     { m1: 0, m3: 0, m6: 0, m12: 0 },

    // Gaming
    psplus:   { m1: 0, m3: 0, m12: 0 },
    gamepass: { m1: 0, m3: 0 },
    steam:    { m1: 0 },
    pubg:     { m1: 0 },
    freefire: { m1: 0 },

    // Social
    social:   { m1: 0 }
  };

  const DEVICES = [
    { key:"smarttv", label_en:"Smart TV", label_ar:"Smart TV", label_dz:"Smart TV" },
    { key:"android", label_en:"Android",  label_ar:"Android",  label_dz:"Android" },
    { key:"iphone",  label_en:"iPhone",   label_ar:"iPhone",   label_dz:"iPhone" },
    { key:"mag",     label_en:"MAG",      label_ar:"MAG",      label_dz:"MAG" },
    { key:"fire",    label_en:"Fire Stick", label_ar:"Fire Stick", label_dz:"Fire Stick" },
    { key:"pc",      label_en:"PC",       label_ar:"PC",       label_dz:"PC" },
  ];

  const DUR = {
    en:{m1:"1 month",m3:"3 months",m6:"6 months",m12:"12 months"},
    ar:{m1:"شهر",m3:"3 شهور",m6:"6 شهور",m12:"12 شهر"},
    dz:{m1:"شهر",m3:"3 شهور",m6:"6 شهور",m12:"12 شهر"},
  };

  // ====== “PRODUCT IMAGES” (SVG logos) ======
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
              font-family="Arial" font-size="30" font-weight="900" fill="rgba(0,0,0,.76)">
          ${label}
        </text>
      </svg>`;
    return "data:image/svg+xml;charset=UTF-8," + encodeURIComponent(svg.trim());
  }

  const ICONS = {
    iptv_premium: svgData("IPTV", "#2b7cff", "#60a5fa"),
    iptv_4k:      svgData("4K",   "#1d4ed8", "#93c5fd"),
    iptv_sports:  svgData("SP",   "#2563eb", "#60a5fa"),
    iptv_movies:  svgData("MV",   "#0ea5e9", "#7dd3fc"),
    iptv_series:  svgData("SR",   "#3b82f6", "#a5b4fc"),

    netflix:  svgData("N",  "#ff2b2b", "#ff6b6b"),
    disney:   svgData("D+", "#2563eb", "#60a5fa"),
    shahid:   svgData("S",  "#22c55e", "#86efac"),
    osn:      svgData("O",  "#a855f7", "#e879f9"),
    prime:    svgData("P",  "#0ea5e9", "#38bdf8"),
    appletv:  svgData("",  "#94a3b8", "#e2e8f0"),
    crunchy:  svgData("C",  "#f97316", "#fdba74"),
    bein:     svgData("be", "#7c3aed", "#c4b5fd"),

    psplus:   svgData("PS", "#1d4ed8", "#93c5fd"),
    gamepass: svgData("X",  "#16a34a", "#86efac"),
    steam:    svgData("S",  "#0f172a", "#64748b"),
    pubg:     svgData("UC", "#f59e0b", "#fde68a"),
    freefire: svgData("FF", "#ef4444", "#fca5a5"),

    social:   svgData("SM", "#14b8a6", "#99f6e4"),
  };

  // ====== I18N ======
  const I18N = {
    darija:{
      heroTitle:"HUSON DIGITAL",
      heroSub:"IPTV • Streaming • Gaming • Social — خلّص بPayPal وأكد فالواتساب.",
      official:"خدمات ديال الثقة", fast:"تفعيل سريع", secure:"دعم آمن", support:"دعم واتساب",
      cta1:"طلب فواتساب", cta2:"شوف الستور",
      howTitle:"كيفاش كنخدمو",
      howText:"1) تختار البروداكت + المدة (+ الجهاز فـ IPTV)  2) تخلص بPayPal  3) تأكيد فواتساب  4) كنفعّلو بسرعة",
      noteNoHack:"⚠️ ما كنبيعوش hacked accounts ولا ولوج غير قانوني.",
      store:"Store", iptv:"IPTV", streaming:"Streaming", gaming:"Gaming", social:"Social",
      duration:"المدة", device:"الجهاز", price:"الثمن", pay:"خلص بPayPal", confirm:"أكد فWhatsApp", tx:"Transaction ID (اختياري)",
      payments:"طرق الدفع", paymentsText:"PayPal (Visa/Master) + دعم واتساب",
      trust:"الثقة", trustText:"خدمات رسمية/قانونية فقط. إذا وقع شي مشكل كنعاونك فالواتساب.",
      faq:"FAQ",
      faq1q:"شحال كتاخد الخدمة؟", faq1a:"غالباً 5–30 دقيقة حسب الضغط.",
      faq2q:"كيفاش نخلص؟", faq2a:"كتخلص بPayPal ومن بعد كتأكد فالواتساب.",
      faq3q:"IPTV كيخدم فاش؟", faq3a:"كيخدم فـ Smart TV / Android / iPhone / MAG / Fire Stick / PC (اختار الجهاز).",
      supportTitle:"مساعدة؟", supportText:"إلى وقع شي مشكل، ضغط على WhatsApp support وغادي نجاوبوك.",
      pricesNote:"ملاحظة: دابا الأثمنة 0. عمّر أثمنة USD فـ PRICES داخل index.html باش يتفعل PayPal.",
      verified:"PayPal Verified",
      sectionIptv:"قسم IPTV",
      sectionIptvSub:"اختار الباقة + المدة + الجهاز — وكمّل الأداء.",
    },
    ar:{
      heroTitle:"HUSON DIGITAL",
      heroSub:"IPTV • ستريمنغ • ألعاب • سوشيال — ادفع عبر PayPal وأكد عبر واتساب.",
      official:"خدمات موثوقة", fast:"تفعيل سريع", secure:"دعم آمن", support:"دعم واتساب",
      cta1:"اطلب عبر واتساب", cta2:"عرض المتجر",
      howTitle:"كيف نعمل؟",
      howText:"1) اختر المنتج + المدة (+ الجهاز في IPTV)  2) ادفع عبر PayPal  3) أكد الطلب عبر واتساب  4) تفعيل سريع",
      noteNoHack:"⚠️ لا نبيع حسابات مهكرة أو وصول غير قانوني.",
      store:"المتجر", iptv:"IPTV", streaming:"ستريمنغ", gaming:"ألعاب", social:"سوشيال",
      duration:"المدة", device:"الجهاز", price:"السعر", pay:"ادفع عبر PayPal", confirm:"تأكيد واتساب", tx:"رقم العملية (اختياري)",
      payments:"طرق الدفع", paymentsText:"PayPal (Visa/MasterCard) + دعم واتساب",
      trust:"الثقة", trustText:"خدمات رسمية/قانونية فقط. في حال أي مشكلة ندعمك عبر واتساب.",
      faq:"أسئلة شائعة",
      faq1q:"كم يستغرق التفعيل؟", faq1a:"غالباً 5–30 دقيقة حسب الضغط.",
      faq2q:"كيف أدفع؟", faq2a:"تدفع عبر PayPal ثم تؤكد عبر واتساب.",
      faq3q:"هل IPTV يعمل على الأجهزة؟", faq3a:"يعمل على Smart TV / Android / iPhone / MAG / Fire Stick / PC (اختر الجهاز).",
      supportTitle:"تحتاج مساعدة؟", supportText:"إذا واجهت مشكلة، تواصل عبر واتساب وسنساعدك.",
      pricesNote:"ملاحظة: الأسعار الآن 0. ضع أسعار USD في PRICES داخل index.html لتفعيل PayPal.",
      verified:"PayPal موثّق",
      sectionIptv:"قسم IPTV",
      sectionIptvSub:"اختر الباقة + المدة + الجهاز — ثم أكمل الدفع.",
    },
    en:{
      heroTitle:"HUSON DIGITAL",
      heroSub:"IPTV • Streaming • Gaming • Social — Pay with PayPal and confirm on WhatsApp.",
      official:"Trusted services", fast:"Fast activation", secure:"Secure support", support:"WhatsApp support",
      cta1:"Order on WhatsApp", cta2:"View Store",
      howTitle:"How it works",
      howText:"1) Choose product + duration (+ device for IPTV)  2) Pay with PayPal  3) Confirm on WhatsApp  4) Fast activation",
      noteNoHack:"⚠️ No hacked accounts or illegal access.",
      store:"Store", iptv:"IPTV", streaming:"Streaming", gaming:"Gaming", social:"Social",
      duration:"Duration", device:"Device", price:"Price", pay:"Pay with PayPal", confirm:"Confirm on WhatsApp", tx:"Transaction ID (optional)",
      payments:"Payment methods", paymentsText:"PayPal (Visa/MasterCard) + WhatsApp support",
      trust:"Trust", trustText:"Official/legal services only. If any issue happens, WhatsApp support will help you.",
      faq:"FAQ",
      faq1q:"Activation time?", faq1a:"Usually 5–30 minutes depending on demand.",
      faq2q:"How to pay?", faq2a:"Pay with PayPal then confirm on WhatsApp.",
      faq3q:"IPTV devices?", faq3a:"Smart TV / Android / iPhone / MAG / Fire Stick / PC (choose device).",
      supportTitle:"Need help?", supportText:"If you face any issue, contact WhatsApp support and we will help you.",
      pricesNote:"Note: prices are 0 now. Set USD prices in PRICES inside index.html to enable PayPal.",
      verified:"PayPal Verified",
      sectionIptv:"IPTV Section",
      sectionIptvSub:"Choose package + duration + device — then pay.",
    }
  };

  let LANG = "darija"; // default as you requested
  const t = (k)=> (I18N[LANG] && I18N[LANG][k]) || I18N.en[k] || k;

  // ====== HELPERS ======
  function setDir(){
    document.documentElement.lang = (LANG==="en") ? "en" : "ar";
    document.documentElement.dir  = (LANG==="en") ? "ltr" : "rtl";
  }

  function formatPrice(usd){
    if (!usd || usd<=0) return "XX";
    const mad = Math.round(usd * FX_USD_TO_MAD);
    return `$${usd}  •  ${mad} MAD`;
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

  function waConfirm({product, durationLabel, deviceLabel, priceText, txid}){
    const msg =
`Salam/Hi 👋
Order confirmation:
- Brand: ${BRAND}
- Product: ${product}
- Duration: ${durationLabel}
- Device: ${deviceLabel || "N/A"}
- Price: ${priceText || "N/A"}
- Payment: PayPal
- Transaction ID: ${txid || "N/A"}
(Please activate / deliver)`;
    return "https://wa.me/" + WHATSAPP_NUMBER + "?text=" + encodeURIComponent(msg);
  }

  function deviceLabel(devKey){
    const d = DEVICES.find(x=>x.key===devKey);
    if (!d) return "";
    return (LANG==="en") ? d.label_en : (LANG==="ar" ? d.label_ar : d.label_dz);
  }

  // ====== PRODUCTS ======
  const IPTV_PRODUCTS = [
    {key:"iptv_premium", name:"IPTV Premium", desc_dz:"باقة شاملة", desc_ar:"باقة شاملة", desc_en:"All-in-one package"},
    {key:"iptv_4k",      name:"IPTV 4K",      desc_dz:"جودة 4K",    desc_ar:"جودة 4K",    desc_en:"4K quality"},
    {key:"iptv_sports",  name:"IPTV Sports",  desc_dz:"رياضة",      desc_ar:"رياضة",      desc_en:"Sports package"},
    {key:"iptv_movies",  name:"IPTV Movies",  desc_dz:"أفلام",      desc_ar:"أفلام",      desc_en:"Movies package"},
    {key:"iptv_series",  name:"IPTV Series",  desc_dz:"سلاسل",      desc_ar:"مسلسلات",    desc_en:"Series package"},
  ];

  const STORE_PRODUCTS = [
    // Streaming
    {key:"netflix", name:"Netflix", cat:"streaming", desc_dz:"ستريمنغ رسمي", desc_ar:"ستريمنغ رسمي", desc_en:"Official streaming"},
    {key:"disney",  name:"Disney+", cat:"streaming", desc_dz:"ستريمنغ رسمي", desc_ar:"ستريمنغ رسمي", desc_en:"Official streaming"},
    {key:"shahid",  name:"Shahid VIP", cat:"streaming", desc_dz:"ستريمنغ رسمي", desc_ar:"ستريمنغ رسمي", desc_en:"Official streaming"},
    {key:"osn",     name:"OSN+", cat:"streaming", desc_dz:"ستريمنغ رسمي", desc_ar:"ستريمنغ رسمي", desc_en:"Official streaming"},
    {key:"prime",   name:"Prime Video", cat:"streaming", desc_dz:"ستريمنغ رسمي", desc_ar:"ستريمنغ رسمي", desc_en:"Official streaming"},
    {key:"appletv", name:"Apple TV+", cat:"streaming", desc_dz:"ستريمنغ رسمي", desc_ar:"ستريمنغ رسمي", desc_en:"Official streaming"},
    {key:"crunchy", name:"Crunchyroll", cat:"streaming", desc_dz:"أنمي", desc_ar:"أنمي", desc_en:"Anime"},
    {key:"bein",    name:"beIN CONNECT", cat:"streaming", desc_dz:"رياضة", desc_ar:"رياضة", desc_en:"Sports"},

    // Gaming
    {key:"psplus",  name:"PlayStation Plus", cat:"gaming", desc_dz:"اشتراك/شحن", desc_ar:"اشتراك/شحن", desc_en:"Subscription/top-up"},
    {key:"gamepass",name:"Xbox Game Pass",   cat:"gaming", desc_dz:"اشتراك", desc_ar:"اشتراك", desc_en:"Subscription"},
    {key:"steam",   name:"Steam Wallet",     cat:"gaming", desc_dz:"شحن", desc_ar:"شحن", desc_en:"Top-up"},
    {key:"pubg",    name:"PUBG UC",          cat:"gaming", desc_dz:"شحن", desc_ar:"شحن", desc_en:"Top-up"},
    {key:"freefire",name:"Free Fire Diamonds",cat:"gaming",desc_dz:"شحن", desc_ar:"شحن", desc_en:"Top-up"},

    // Social
    {key:"social",  name:"Social Services",   cat:"social", desc_dz:"حسب الطلب", desc_ar:"حسب الطلب", desc_en:"On request"},
  ];

  function renderStatic(){
    setDir();
    document.querySelectorAll("[data-i18n]").forEach(el=>{
      el.textContent = t(el.getAttribute("data-i18n"));
    });
    document.querySelectorAll("[data-lang]").forEach(btn=>{
      btn.classList.toggle("active", btn.getAttribute("data-lang")===LANG);
    });
    document.querySelectorAll("[data-wa-global]").forEach(a=>{
      a.href = waGlobal(); a.target="_blank"; a.rel="noopener";
    });
    document.getElementById("yr").textContent = new Date().getFullYear();
    document.getElementById("fx").textContent = String(FX_USD_TO_MAD);
  }

  function makeCard({key, name, desc_dz, desc_ar, desc_en}, opts){
    const withDevice = !!opts.withDevice;

    const card = document.createElement("div");
    card.className = "card item";

    const top = document.createElement("div");
    top.className = "top";

    const left = document.createElement("div");
    left.className = "svc";

    const icon = document.createElement("div");
    icon.className = "svcIcon";
    const img = document.createElement("img");
    img.alt = name;
    img.src = ICONS[key] || ICONS.social;
    icon.appendChild(img);

    const meta = document.createElement("div");
    const title = document.createElement("div");
    title.className = "svcName";
    title.textContent = name;

    const desc = document.createElement("div");
    desc.className = "svcDesc";
    desc.textContent = (LANG==="en") ? desc_en : (LANG==="ar" ? desc_ar : desc_dz);

    meta.appendChild(title);
    meta.appendChild(desc);

    left.appendChild(icon);
    left.appendChild(meta);

    const right = document.createElement("div");
    right.className = "mini";
    right.innerHTML = withDevice
      ? `<span class="pill">${t("device")}</span><span class="pill">${t("duration")}</span>`
      : `<span class="pill">${t("duration")}</span><span class="pill">${t("payments")}</span>`;

    top.appendChild(left);
    top.appendChild(right);

    // selectors row
    const row = document.createElement("div");
    row.className = "row";

    // duration select
    const durSel = document.createElement("select");
    durSel.id = "dur_"+key;
    const durKeys = Object.keys(PRICES[key] || {});
    durKeys.forEach(kDur=>{
      const opt = document.createElement("option");
      const label = (LANG==="en") ? (DUR.en[kDur]||kDur) : (LANG==="ar" ? (DUR.ar[kDur]||DUR.en[kDur]||kDur) : (DUR.dz[kDur]||DUR.en[kDur]||kDur));
      opt.value = kDur;
      opt.textContent = label;
      durSel.appendChild(opt);
    });

    // device select (optional)
    let devSel = null;
    if (withDevice){
      devSel = document.createElement("select");
      devSel.id = "dev_"+key;
      DEVICES.forEach(d=>{
        const opt = document.createElement("option");
        opt.value = d.key;
        opt.textContent = (LANG==="en") ? d.label_en : (LANG==="ar" ? d.label_ar : d.label_dz);
        devSel.appendChild(opt);
      });
    }

    const price = document.createElement("div");
    price.className = "price";
    price.id = "price_"+key;

    const hint = document.createElement("div");
    hint.className = "hint";
    hint.textContent = withDevice ? `${t("device")} + ${t("duration")}` : t("duration");

    if (withDevice){
      row.appendChild(hint);
      row.appendChild(devSel);
      row.appendChild(durSel);
      row.appendChild(price);
    }else{
      row.appendChild(hint);
      row.appendChild(durSel);
      row.appendChild(price);
    }

    // tx input
    const tx = document.createElement("input");
    tx.placeholder = t("tx");
    tx.id = "tx_"+key;
    tx.style.width = "100%";

    // actions
    const actions = document.createElement("div");
    actions.className = "row";

    const pay = document.createElement("a");
    pay.className = "btn btn-blue";
    pay.textContent = t("pay");
    pay.target="_blank"; pay.rel="noopener";

    const confirm = document.createElement("a");
    confirm.className = "btn btn-primary";
    confirm.textContent = t("confirm");
    confirm.target="_blank"; confirm.rel="noopener";

    function update(){
      const dk = durSel.value;
      const usd = (PRICES[key] && PRICES[key][dk]) ? PRICES[key][dk] : 0;
      const priceText = formatPrice(usd);
      price.textContent = priceText;

      const durLabelEn = DUR.en[dk] || dk;
      const durLabel = (LANG==="en") ? durLabelEn : (LANG==="ar" ? (DUR.ar[dk]||durLabelEn) : (DUR.dz[dk]||durLabelEn));

      const devKey = withDevice ? devSel.value : "";
      const devLabel = withDevice ? deviceLabel(devKey) : "";

      // PayPal: disable if 0
      if (usd > 0){
        pay.href = paypalBuyNow(`${BRAND} - ${name} (${durLabelEn})${withDevice ? " - " + (DEVICES.find(x=>x.key===devKey)?.label_en || devKey) : ""}`, usd);
        pay.style.opacity = "1";
        pay.style.pointerEvents = "auto";
      }else{
        pay.href = "#";
        pay.style.opacity = ".55";
        pay.style.pointerEvents = "none";
      }

      confirm.href = waConfirm({
        product: name,
        durationLabel: durLabel,
        deviceLabel: devLabel,
        priceText,
        txid: tx.value.trim()
      });
    }

    durSel.addEventListener("change", update);
    if (withDevice) devSel.addEventListener("change", update);
    tx.addEventListener("input", update);

    actions.appendChild(pay);
    actions.appendChild(confirm);

    card.appendChild(top);
    card.appendChild(row);
    card.appendChild(tx);
    card.appendChild(actions);

    update();
    return card;
  }

  function renderIPTV(){
    const grid = document.getElementById("iptvCards");
    grid.innerHTML = "";
    IPTV_PRODUCTS.forEach(p=>{
      grid.appendChild(makeCard(p, {withDevice:true}));
    });
  }

  function renderStore(){
    const grid = document.getElementById("storeCards");
    grid.innerHTML = "";
    STORE_PRODUCTS.forEach(p=>{
      grid.appendChild(makeCard(p, {withDevice:false}));
    });
  }

  function setLang(newLang){
    LANG = newLang;
    renderStatic();
    renderIPTV();
    renderStore();
  }

  document.addEventListener("DOMContentLoaded", ()=>{
    // default language = darija
    setLang("darija");

    document.querySelectorAll("[data-lang]").forEach(btn=>{
      btn.addEventListener("click", ()=> setLang(btn.getAttribute("data-lang")));
    });
  });
</script>

<header>
  <div class="wrap nav">
    <div class="brand">
      <div class="mark" aria-hidden="true">
        <svg width="26" height="26" viewBox="0 0 24 24" fill="none">
          <path d="M7 7h10v10H7z" stroke="rgba(6,16,34,.85)" stroke-width="2.4" />
          <path d="M5.5 9.5V6.5h3" stroke="rgba(6,16,34,.85)" stroke-width="2.4" stroke-linecap="round"/>
          <path d="M18.5 14.5v3h-3" stroke="rgba(6,16,34,.85)" stroke-width="2.4" stroke-linecap="round"/>
        </svg>
      </div>
      <div>
        <div class="name">HUSON DIGITAL</div>
        <div class="tag">IPTV Pro • PayPal • WhatsApp Support • Morocco 🇲🇦</div>
      </div>
    </div>

    <nav class="links">
      <a href="#iptv" data-i18n="iptv">IPTV</a>
      <a href="#store" data-i18n="store">Store</a>
      <a href="#how" data-i18n="howTitle">How</a>
      <a href="#faq" data-i18n="faq">FAQ</a>
    </nav>

    <div class="actions">
      <div class="lang">
        <button type="button" data-lang="darija" class="active">Darija</button>
        <button type="button" data-lang="ar">عربية</button>
        <button type="button" data-lang="en">English</button>
      </div>
      <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">طلب فواتساب</a>
    </div>
  </div>
</header>

<main class="wrap">
  <section class="hero">
    <div class="card heroMain">
      <h1 data-i18n="heroTitle">HUSON DIGITAL</h1>
      <p class="sub" data-i18n="heroSub">IPTV • Streaming • Gaming • Social — خلّص بPayPal وأكد فالواتساب.</p>

      <div class="badges">
        <div class="badge">✅ <b data-i18n="official">خدمات ديال الثقة</b></div>
        <div class="badge">⚡ <span data-i18n="fast">تفعيل سريع</span></div>
        <div class="badge">🔒 <span data-i18n="secure">دعم آمن</span></div>
        <div class="badge">💬 <span data-i18n="support">دعم واتساب</span></div>
        <div class="badge">🅿️ <span data-i18n="verified">PayPal Verified</span></div>
      </div>

      <div style="display:flex;gap:10px;flex-wrap:wrap;position:relative">
        <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">طلب فواتساب</a>
        <a class="btn btn-blue" href="#iptv" data-i18n="iptv">IPTV</a>
        <a class="btn btn-ghost" href="#store" data-i18n="cta2">شوف الستور</a>
      </div>

      <div class="note noteBlue" data-i18n="howText" id="howText">
        1) تختار البروداكت + المدة (+ الجهاز فـ IPTV)  2) تخلص بPayPal  3) تأكيد فواتساب  4) كنفعّلو بسرعة
      </div>

      <div class="note noteWarn" data-i18n="noteNoHack">⚠️ ما كنبيعوش hacked accounts ولا ولوج غير قانوني.</div>
    </div>

    <aside class="card side">
      <div class="kpiRow"><span class="k">IPTV Pro</span><span class="v">Smart TV / Android / iPhone</span></div>
      <div class="kpiRow"><span class="k">Payments</span><span class="v">PayPal • Visa • Master</span></div>
      <div class="kpiRow"><span class="k">Support</span><span class="v">WhatsApp 24/7</span></div>
      <div class="kpiRow"><span class="k">FX</span><span class="v">1 USD ≈ <span id="fx"></span> MAD</span></div>

      <div class="note" data-i18n="pricesNote">ملاحظة: دابا الأثمنة 0. عمّر أثمنة USD فـ PRICES داخل index.html باش يتفعل PayPal.</div>

      <div style="display:flex;gap:10px;flex-wrap:wrap;position:relative">
        <a class="btn btn-primary" data-wa-global href="#">WhatsApp</a>
        <a class="btn btn-blue" href="#iptv" data-i18n="sectionIptv">قسم IPTV</a>
      </div>
    </aside>
  </section>

  <!-- IPTV SECTION -->
  <section id="iptv">
    <div class="sectionTitle">
      <h2 data-i18n="sectionIptv">قسم IPTV</h2>
      <p data-i18n="sectionIptvSub">اختار الباقة + المدة + الجهاز — وكمّل الأداء.</p>
    </div>
    <div class="grid" id="iptvCards"></div>
  </section>

  <!-- STORE SECTION -->
  <section id="store">
    <div class="sectionTitle">
      <h2 data-i18n="store">Store</h2>
      <p data-i18n="paymentsText">PayPal (Visa/Master) + دعم واتساب</p>
    </div>
    <div class="grid" id="storeCards"></div>
  </section>

  <section class="two" id="how">
    <div class="card" style="padding:16px">
      <div class="sectionTitle" style="margin:0 0 10px">
        <h2 data-i18n="payments">طرق الدفع</h2>
        <p>Secure</p>
      </div>
      <p class="sub" style="margin:0" data-i18n="paymentsText">PayPal (Visa/Master) + دعم واتساب</p>
      <div class="badges" style="margin-top:12px">
        <div class="badge">🅿️ PayPal</div>
        <div class="badge">💳 Visa</div>
        <div class="badge">💳 MasterCard</div>
        <div class="badge">💬 WhatsApp</div>
        <div class="badge">🔒 SSL</div>
      </div>
      <div class="note noteBlue">
        ✅ PayPal كيخلص بUSD — والثمن كيبان حتى MAD فالموقع.
      </div>
    </div>

    <div class="card" style="padding:16px">
      <div class="sectionTitle" style="margin:0 0 10px">
        <h2 data-i18n="howTitle">كيفاش كنخدمو</h2>
        <p>PayPal → WhatsApp → Activation</p>
      </div>
      <div class="note noteBlue" data-i18n="howText">
        1) تختار البروداكت + المدة (+ الجهاز فـ IPTV)  2) تخلص بPayPal  3) تأكيد فواتساب  4) كنفعّلو بسرعة
      </div>
      <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">طلب فواتساب</a>
        <a class="btn btn-blue" href="#iptv" data-i18n="iptv">IPTV</a>
      </div>
    </div>
  </section>

  <section>
    <div class="sectionTitle">
      <h2 data-i18n="trust">الثقة</h2>
      <p>Trusted</p>
    </div>
    <div class="card" style="padding:16px">
      <div class="sub" data-i18n="trustText">
        خدمات رسمية/قانونية فقط. إذا وقع شي مشكل كنعاونك فالواتساب.
      </div>
      <div class="note noteWarn" data-i18n="noteNoHack">⚠️ ما كنبيعوش hacked accounts ولا ولوج غير قانوني.</div>
    </div>
  </section>

  <section id="faq">
    <div class="sectionTitle">
      <h2 data-i18n="faq">FAQ</h2>
      <p>Quick answers</p>
    </div>
    <div class="card" style="padding:16px">
      <details>
        <summary data-i18n="faq1q">شحال كتاخد الخدمة؟</summary>
        <p data-i18n="faq1a">غالباً 5–30 دقيقة حسب الضغط.</p>
      </details>
      <details>
        <summary data-i18n="faq2q">كيفاش نخلص؟</summary>
        <p data-i18n="faq2a">كتخلص بPayPal ومن بعد كتأكد فالواتساب.</p>
      </details>
      <details>
        <summary data-i18n="faq3q">IPTV كيخدم فاش؟</summary>
        <p data-i18n="faq3a">كيخدم فـ Smart TV / Android / iPhone / MAG / Fire Stick / PC (اختار الجهاز).</p>
      </details>

      <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#" data-i18n="cta1">طلب فواتساب</a>
        <a class="btn btn-blue" href="#store" data-i18n="store">Store</a>
      </div>
    </div>
  </section>

  <section>
    <div class="sectionTitle">
      <h2 data-i18n="supportTitle">مساعدة؟</h2>
      <p>Support</p>
    </div>
    <div class="card" style="padding:16px">
      <div class="sub" data-i18n="supportText">إلى وقع شي مشكل، ضغط على WhatsApp support وغادي نجاوبوك.</div>
      <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-primary" data-wa-global href="#">WhatsApp Support</a>
        <span class="pill">+212 702 855 273</span>
      </div>
    </div>
  </section>

  <div class="footer">
    <div style="display:flex;gap:12px;flex-wrap:wrap;align-items:center;justify-content:space-between">
      <div><b>HUSON DIGITAL</b> • © <span id="yr"></span><br/><span>Digital services • Morocco</span></div>
      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn btn-ghost" data-wa-global href="#">WhatsApp</a>
        <a class="btn btn-ghost" href="#iptv">IPTV</a>
        <a class="btn btn-ghost" href="#store">Store</a>
      </div>
    </div>
  </div>
</main>

<div class="float">
  <div class="bubble">بغيتي تعاون؟</div>
  <a class="btn btn-primary" data-wa-global href="#">WhatsApp 💬</a>
</div>

</body>
</html>
