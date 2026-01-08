<!--
Save as: /cryptosovereignty/index.html  (or your root index.html)
Designed for GitHub Pages. No build step. Brutalist + fast.
Primary CTAs: Amazon + Bitcoin Magazine Store.
Sources for links:
- Amazon: https://www.amazon.com/Cryptosovereignty-Encrypted-Political-Philosophy-Bitcoin/dp/B0CFCW6JJR :contentReference[oaicite:0]{index=0}
- Bitcoin Magazine Store: https://store.bitcoinmagazine.com/products/cryptosovereignty :contentReference[oaicite:1]{index=1}
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />

  <title>CryptoSovereignty — Erik Cason</title>
  <meta name="description" content="CryptoSovereignty: The Encrypted Political Philosophy of Bitcoin — a book about sovereignty, cryptography, money, and the end of managed reality." />
  <meta name="robots" content="index,follow" />
  <link rel="canonical" href="https://cryptosovereignty.org/cryptosovereignty/" />

  <!-- Open Graph -->
  <meta property="og:title" content="CryptoSovereignty — Erik Cason" />
  <meta property="og:description" content="The Encrypted Political Philosophy of Bitcoin. Sovereignty through cryptography." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://cryptosovereignty.org/cryptosovereignty/" />
  <!-- Optional: add your cover image -->
  <!-- <meta property="og:image" content="https://cryptosovereignty.org/assets/cryptosovereignty-cover.jpg" /> -->

  <!-- Twitter -->
  <meta name="twitter:card" content="summary_large_image" />

  <!-- Book schema (JSON-LD) -->
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Book",
    "name": "CryptoSovereignty: The Encrypted Political Philosophy of Bitcoin",
    "author": { "@type": "Person", "name": "Erik Cason" },
    "inLanguage": "en",
    "isbn": "979-8985728972",
    "publisher": { "@type": "Organization", "name": "Bitcoin Magazine Books" },
    "url": "https://cryptosovereignty.org/cryptosovereignty/",
    "workExample": [
      {
        "@type": "Book",
        "bookFormat": "https://schema.org/Paperback",
        "url": "https://www.amazon.com/Cryptosovereignty-Encrypted-Political-Philosophy-Bitcoin/dp/B0CFCW6JJR"
      },
      {
        "@type": "Book",
        "bookFormat": "https://schema.org/EBook",
        "url": "https://store.bitcoinmagazine.com/products/cryptosovereignty"
      }
    ]
  }
  </script>

  <style>
    :root{
      --bg:#0b0b0c;
      --fg:#f6f6f6;
      --muted:#b8b8b8;
      --line:#1f1f22;
      --chip:#101014;
      --accent:#ffffff;
      --danger:#ff3b3b;
      --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
      --sans: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
      --radius: 18px;
      --shadow: 0 10px 30px rgba(0,0,0,.45);
      --max: 1100px;
    }
    *{ box-sizing:border-box; }
    html,body{ height:100%; }
    body{
      margin:0;
      background: radial-gradient(1200px 600px at 80% -10%, rgba(255,255,255,.08), transparent 60%),
                  radial-gradient(900px 500px at 20% 0%, rgba(255,255,255,.06), transparent 55%),
                  var(--bg);
      color:var(--fg);
      font-family: var(--sans);
      letter-spacing: .2px;
    }
    a{ color:inherit; text-decoration:none; }
    .wrap{ max-width:var(--max); margin:0 auto; padding:28px 18px 64px; }
    .top{
      display:flex; align-items:center; justify-content:space-between;
      gap:14px; padding:10px 0 22px;
    }
    .brand{
      display:flex; align-items:center; gap:10px; font-family:var(--mono);
      font-weight:700; letter-spacing: .6px; text-transform: uppercase;
      font-size: 12px; color: var(--muted);
    }
    .dot{ width:9px; height:9px; border-radius:2px; background:var(--fg); box-shadow: 0 0 0 1px rgba(255,255,255,.15); }
    .nav{
      display:flex; gap:14px; flex-wrap:wrap; justify-content:flex-end;
      font-family:var(--mono); font-size:12px; color:var(--muted);
    }
    .nav a{ padding:7px 10px; border:1px solid var(--line); border-radius:999px; background: rgba(255,255,255,.02); }
    .nav a:hover{ border-color: rgba(255,255,255,.22); }

    .hero{
      display:grid;
      grid-template-columns: 1.15fr .85fr;
      gap:22px;
      align-items:stretch;
      margin-top: 8px;
    }
    @media (max-width: 900px){ .hero{ grid-template-columns: 1fr; } }

    .card{
      border:1px solid var(--line);
      background: linear-gradient(180deg, rgba(255,255,255,.03), rgba(255,255,255,.01));
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    .hero-left{ padding:26px 22px; }
    .kicker{
      font-family: var(--mono);
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 1.4px;
      font-size: 12px;
      margin-bottom: 10px;
    }
    h1{
      margin:0 0 10px 0;
      font-family: var(--mono);
      font-size: clamp(28px, 4.1vw, 46px);
      line-height: 1.06;
      letter-spacing: -0.5px;
    }
    .sub{
      margin: 0 0 18px;
      color: var(--muted);
      font-size: 16px;
      line-height: 1.55;
      max-width: 68ch;
    }
    .chips{ display:flex; flex-wrap:wrap; gap:8px; margin: 0 0 18px; }
    .chip{
      font-family: var(--mono);
      font-size: 12px;
      padding: 7px 10px;
      border-radius: 999px;
      border: 1px solid var(--line);
      background: var(--chip);
      color: #d8d8d8;
    }
    .cta-row{ display:flex; gap:10px; flex-wrap:wrap; margin-top: 12px; }
    .btn{
      display:inline-flex; align-items:center; gap:10px;
      padding: 12px 14px;
      border-radius: 14px;
      border: 1px solid rgba(255,255,255,.18);
      background: rgba(255,255,255,.06);
      font-family: var(--mono);
      font-weight: 700;
      letter-spacing: .2px;
      transition: transform .08s ease, background .12s ease, border-color .12s ease;
    }
    .btn:hover{ background: rgba(255,255,255,.10); border-color: rgba(255,255,255,.30); transform: translateY(-1px); }
    .btn.primary{
      background: rgba(255,255,255,.92);
      color: #0b0b0c;
      border-color: rgba(255,255,255,.90);
    }
    .btn.primary:hover{ background: #ffffff; }
    .btn .tag{
      font-size: 11px;
      font-weight: 800;
      padding: 3px 8px;
      border-radius: 999px;
      background: rgba(0,0,0,.12);
      color: rgba(0,0,0,.78);
    }
    .btn.secondary .tag{
      background: rgba(255,255,255,.10);
      color: rgba(255,255,255,.85);
    }

    .hero-right{ padding: 18px; display:flex; flex-direction:column; gap:12px; }
    .cover{
      border-radius: calc(var(--radius) - 6px);
      border: 1px solid rgba(255,255,255,.12);
      background:
        linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02)),
        repeating-linear-gradient(90deg, rgba(255,255,255,.05), rgba(255,255,255,.05) 1px, transparent 1px, transparent 9px);
      min-height: 320px;
      display:flex;
      align-items:flex-end;
      padding: 16px;
      position:relative;
      overflow:hidden;
    }
    .cover:before{
      content:"";
      position:absolute; inset:-60px -80px auto auto;
      width:220px; height:220px;
      background: radial-gradient(circle at 30% 30%, rgba(255,255,255,.28), transparent 60%);
      transform: rotate(12deg);
      opacity:.35;
      pointer-events:none;
    }
    .cover-title{
      position:relative;
      font-family: var(--mono);
      font-weight: 900;
      letter-spacing: .6px;
      text-transform: uppercase;
      font-size: 14px;
      color: rgba(255,255,255,.88);
    }
    .meta{
      border: 1px solid var(--line);
      border-radius: calc(var(--radius) - 6px);
      background: rgba(0,0,0,.25);
      padding: 14px;
      font-family: var(--mono);
      color: #d9d9d9;
      font-size: 12px;
      line-height: 1.55;
    }
    .meta b{ color: var(--fg); }
    .grid{
      margin-top: 18px;
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
    }
    @media (max-width: 900px){ .grid{ grid-template-columns: 1fr; } }
    .mini{
      padding: 16px;
      border-radius: var(--radius);
      border: 1px solid var(--line);
      background: rgba(255,255,255,.02);
    }
    .mini h3{
      margin:0 0 8px;
      font-family: var(--mono);
      font-size: 13px;
      text-transform: uppercase;
      letter-spacing: 1px;
      color: #e9e9e9;
    }
    .mini p{
      margin:0;
      color: var(--muted);
      line-height: 1.55;
      font-size: 14px;
    }
    .quote{
      margin-top: 14px;
      padding: 18px 18px;
      border-radius: var(--radius);
      border: 1px solid rgba(255,255,255,.16);
      background: rgba(255,255,255,.03);
    }
    .quote p{
      margin:0;
      font-size: 15px;
      line-height: 1.6;
      color: #e7e7e7;
    }
    .quote .by{
      margin-top: 10px;
      font-family: var(--mono);
      color: var(--muted);
      font-size: 12px;
    }
    footer{
      margin-top: 26px;
      padding-top: 18px;
      border-top: 1px solid var(--line);
      color: var(--muted);
      font-family: var(--mono);
      font-size: 12px;
      display:flex;
      justify-content:space-between;
      gap:12px;
      flex-wrap:wrap;
    }
    .fine a{ text-decoration: underline; text-underline-offset: 3px; }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="top">
      <div class="brand"><span class="dot"></span> cryptosovereignty.org / book</div>
      <div class="nav">
        <a href="#what">What it is</a>
        <a href="#who">Who it’s for</a>
        <a href="#buy">Buy</a>
      </div>
    </div>

    <section class="hero">
      <div class="card hero-left">
        <div class="kicker">The encrypted political philosophy of Bitcoin</div>
        <h1>CryptoSovereignty</h1>
        <p class="sub">
          A brutal, lucid argument that sovereignty is not granted by institutions —
          it is engineered through cryptography, property, and voluntary coordination.
        </p>

        <div class="chips" aria-label="Topics">
          <span class="chip">Bitcoin as law</span>
          <span class="chip">Exit over voice</span>
          <span class="chip">Truth > authority</span>
          <span class="chip">Cryptography as power</span>
          <span class="chip">Political legitimacy</span>
        </div>

        <div class="cta-row" id="buy">
          <a class="btn primary" href="https://www.amazon.com/Cryptosovereignty-Encrypted-Political-Philosophy-Bitcoin/dp/B0CFCW6JJR" rel="noopener" target="_blank">
            Buy on Amazon <span class="tag">print</span>
          </a>
          <a class="btn secondary" href="https://store.bitcoinmagazine.com/products/cryptosovereignty" rel="noopener" target="_blank">
            Buy on Bitcoin Magazine <span class="tag">BM</span>
          </a>
        </div>

        <div class="quote" style="margin-top:18px">
          <p>
            “Not just a book about money — a book about the re-emergence of personal power.”
          </p>
          <div class="by">— Reader summary / positioning line</div>
        </div>
      </div>

      <aside class="card hero-right">
        <img
  src="/assets/cryptosovereignty-cover.jpg"
  alt="CryptoSovereignty book cover by Erik Cason"
  style="width:100%;height:auto;border-radius:12px;border:1px solid rgba(255,255,255,.12);"
/>


        <div class="meta">
          <div><b>Author:</b> Erik Cason</div>
          <div><b>Publisher:</b> Bitcoin Magazine Books</div>
          <div><b>Format:</b> Print + Digital</div>
          <div><b>Thesis:</b> Sovereignty is a protocol — not permission.</div>
        </div>

        <div class="meta">
          <b>Press:</b> Bitcoin Magazine feature / announcement<br/>
          <a href="https://bitcoinmagazine.com/bitcoin-books/erik-cason-new-bitcoin-book-cryptosovereignty" target="_blank" rel="noopener" style="text-decoration:underline; text-underline-offset:3px;">
            Read the article →
          </a>
        </div>
      </aside>
    </section>

    <section class="grid" id="what">
      <div class="mini">
        <h3>What it is</h3>
        <p>
          A philosophy of Bitcoin as an emergent political order: property, legitimacy, and the
          cryptographic foundations of non-violent coordination.
        </p>
      </div>
      <div class="mini">
        <h3>What it’s not</h3>
        <p>
          Not trading advice. Not blockchain hype. Not institutional apologetics.
          It’s a theory of sovereignty under the conditions of modern surveillance.
        </p>
      </div>
      <div class="mini" id="who">
        <h3>Who it’s for</h3>
        <p>
          Builders, readers, operators, and anyone allergic to managed reality —
          who wants the deepest “why” behind Bitcoin, not just the “what.”
        </p>
      </div>
    </section>

    <footer>
      <div class="fine">
        Two canonical purchase links:
        <a href="https://www.amazon.com/Cryptosovereignty-Encrypted-Political-Philosophy-Bitcoin/dp/B0CFCW6JJR" target="_blank" rel="noopener">Amazon</a>
        ·
        <a href="https://store.bitcoinmagazine.com/products/cryptosovereignty" target="_blank" rel="noopener">Bitcoin Magazine Store</a>
      </div>
      <div class="fine">© <span id="y"></span> CryptoSovereignty</div>
    </footer>
  </div>

  <script>
    document.getElementById("y").textContent = new Date().getFullYear();
  </script>
</body>
</html>
