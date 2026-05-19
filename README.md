# Disposable-
Premium disposable vape 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>VAPE Cloud AI Premium</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Barlow+Condensed:wght@300;400;600;700&family=Barlow:wght@300;400&display=swap" rel="stylesheet"/>
<style>
  :root {
    --gold: #C9A84C;
    --gold-light: #F0D080;
    --smoke: #E8E8E8;
    --deep: #0A0A0A;
    --charcoal: #141414;
    --mid: #1E1E1E;
    --accent: #FF4C29;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background: var(--deep);
    color: var(--smoke);
    font-family: 'Barlow', sans-serif;
    overflow-x: hidden;
  }

  /* Animated grain overlay */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.06'/%3E%3C/svg%3E");
    pointer-events: none;
    z-index: 999;
    opacity: 0.4;
  }

  /* HERO */
  .hero {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 60px 24px;
    position: relative;
    background: radial-gradient(ellipse at 50% 0%, #2a1a00 0%, var(--deep) 65%);
    overflow: hidden;
  }

  .hero::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0; right: 0;
    height: 120px;
    background: linear-gradient(to bottom, transparent, var(--deep));
  }

  /* Floating smoke rings */
  .ring {
    position: absolute;
    border-radius: 50%;
    border: 1px solid rgba(201,168,76,0.12);
    animation: expand 8s ease-out infinite;
    opacity: 0;
  }
  .ring:nth-child(1) { width: 300px; height: 300px; top: 30%; left: 50%; transform: translateX(-50%); animation-delay: 0s; }
  .ring:nth-child(2) { width: 500px; height: 500px; top: 20%; left: 50%; transform: translateX(-50%); animation-delay: 2s; }
  .ring:nth-child(3) { width: 700px; height: 700px; top: 10%; left: 50%; transform: translateX(-50%); animation-delay: 4s; }

  @keyframes expand {
    0%   { opacity: 0; transform: translateX(-50%) scale(0.7); }
    20%  { opacity: 1; }
    100% { opacity: 0; transform: translateX(-50%) scale(1.3); }
  }

  .badge {
    display: inline-block;
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 4px;
    text-transform: uppercase;
    color: var(--gold);
    border: 1px solid var(--gold);
    padding: 6px 18px;
    margin-bottom: 28px;
    animation: fadeUp 0.8s ease both;
  }

  .hero-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(72px, 16vw, 160px);
    line-height: 0.9;
    letter-spacing: 2px;
    color: #fff;
    animation: fadeUp 0.9s ease 0.1s both;
  }

  .hero-title span {
    display: block;
    background: linear-gradient(135deg, var(--gold) 0%, var(--gold-light) 50%, var(--gold) 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .hero-sub {
    margin-top: 20px;
    font-family: 'Barlow Condensed', sans-serif;
    font-size: clamp(16px, 3vw, 22px);
    font-weight: 300;
    letter-spacing: 3px;
    color: rgba(232,232,232,0.6);
    text-transform: uppercase;
    animation: fadeUp 1s ease 0.2s both;
  }

  .hero-cta {
    margin-top: 48px;
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
    justify-content: center;
    animation: fadeUp 1s ease 0.35s both;
  }

  .btn-primary {
    background: linear-gradient(135deg, var(--gold), var(--gold-light), var(--gold));
    background-size: 200%;
    color: #000;
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 700;
    font-size: 13px;
    letter-spacing: 3px;
    text-transform: uppercase;
    padding: 16px 40px;
    border: none;
    cursor: pointer;
    transition: background-position 0.4s, transform 0.2s;
  }
  .btn-primary:hover { background-position: right; transform: scale(1.03); }

  .btn-ghost {
    background: transparent;
    color: var(--gold);
    font-family: 'Barlow Condensed', sans-serif;
    font-weight: 600;
    font-size: 13px;
    letter-spacing: 3px;
    text-transform: uppercase;
    padding: 15px 40px;
    border: 1px solid var(--gold);
    cursor: pointer;
    transition: background 0.3s;
  }
  .btn-ghost:hover { background: rgba(201,168,76,0.08); }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  /* DIVIDER */
  .divider {
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 0 24px;
    margin: 0 auto;
    max-width: 900px;
  }
  .divider-line { flex: 1; height: 1px; background: linear-gradient(to right, transparent, var(--gold), transparent); }
  .divider-icon { color: var(--gold); font-size: 18px; }

  /* SECTION */
  section {
    max-width: 1100px;
    margin: 0 auto;
    padding: 80px 24px;
  }

  .section-label {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 11px;
    letter-spacing: 5px;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 16px;
  }

  .section-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(40px, 7vw, 72px);
    line-height: 1;
    color: #fff;
    margin-bottom: 40px;
  }

  /* BRANDS */
  .brands-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
    gap: 2px;
    margin-top: 40px;
  }

  .brand-card {
    background: var(--charcoal);
    padding: 30px 20px;
    text-align: center;
    border-top: 2px solid transparent;
    transition: border-color 0.3s, background 0.3s;
    cursor: default;
    position: relative;
    overflow: hidden;
  }
  .brand-card::before {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(135deg, rgba(201,168,76,0.04), transparent);
    opacity: 0;
    transition: opacity 0.3s;
  }
  .brand-card:hover { border-color: var(--gold); }
  .brand-card:hover::before { opacity: 1; }

  .brand-name {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 22px;
    letter-spacing: 2px;
    color: #fff;
  }
  .brand-tag {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 10px;
    letter-spacing: 2px;
    color: rgba(201,168,76,0.7);
    text-transform: uppercase;
    margin-top: 4px;
  }

  /* PRODUCTS */
  .products-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 2px;
  }

  .product-card {
    background: var(--charcoal);
    padding: 36px 32px;
    position: relative;
    overflow: hidden;
    transition: transform 0.3s;
  }
  .product-card:hover { transform: translateY(-4px); }
  .product-card::after {
    content: '';
    position: absolute;
    bottom: 0; left: 0;
    width: 0; height: 2px;
    background: var(--gold);
    transition: width 0.4s;
  }
  .product-card:hover::after { width: 100%; }

  .product-tier {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 10px;
    letter-spacing: 3px;
    color: var(--gold);
    text-transform: uppercase;
    margin-bottom: 12px;
  }

  .product-name {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 26px;
    letter-spacing: 1px;
    color: #fff;
    line-height: 1.1;
    margin-bottom: 12px;
  }

  .product-desc {
    font-family: 'Barlow', sans-serif;
    font-size: 13px;
    line-height: 1.6;
    color: rgba(232,232,232,0.5);
    margin-bottom: 24px;
  }

  .product-price {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 36px;
    color: var(--gold-light);
    letter-spacing: 1px;
  }

  /* FEATURES */
  .features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 2px;
    margin-top: 40px;
  }

  .feature-item {
    background: var(--charcoal);
    padding: 32px 24px;
  }

  .feature-icon {
    font-size: 28px;
    margin-bottom: 16px;
    display: block;
  }

  .feature-title {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 16px;
    font-weight: 700;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: #fff;
    margin-bottom: 8px;
  }

  .feature-desc {
    font-size: 13px;
    line-height: 1.6;
    color: rgba(232,232,232,0.45);
  }

  /* PROMO BANNER */
  .promo-banner {
    background: linear-gradient(135deg, #1a0e00, var(--charcoal), #1a0e00);
    border-top: 1px solid rgba(201,168,76,0.2);
    border-bottom: 1px solid rgba(201,168,76,0.2);
    padding: 60px 24px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }

  .promo-banner::before {
    content: '';
    position: absolute;
    top: -100px; left: 50%; transform: translateX(-50%);
    width: 600px; height: 600px;
    background: radial-gradient(circle, rgba(201,168,76,0.06) 0%, transparent 70%);
    pointer-events: none;
  }

  .promo-quote {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(28px, 6vw, 64px);
    line-height: 1.1;
    color: #fff;
    max-width: 900px;
    margin: 0 auto 20px;
  }
  .promo-quote em {
    font-style: normal;
    color: var(--gold);
  }

  .promo-sub {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 14px;
    letter-spacing: 3px;
    color: rgba(232,232,232,0.4);
    text-transform: uppercase;
  }

  /* SOCIAL CAPTIONS */
  .captions-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 2px;
    margin-top: 40px;
  }

  .caption-card {
    background: var(--charcoal);
    padding: 32px;
    border-left: 3px solid var(--gold);
  }

  .caption-platform {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 10px;
    letter-spacing: 4px;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 16px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .caption-text {
    font-family: 'Barlow', sans-serif;
    font-size: 14px;
    line-height: 1.7;
    color: rgba(232,232,232,0.7);
    margin-bottom: 16px;
    font-style: italic;
  }

  .caption-tags {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 12px;
    color: rgba(201,168,76,0.6);
    letter-spacing: 1px;
  }

  /* CTA SECTION */
  .cta-section {
    text-align: center;
    padding: 100px 24px;
    background: radial-gradient(ellipse at 50% 100%, #2a1a00 0%, var(--deep) 60%);
  }

  .cta-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(48px, 10vw, 100px);
    color: #fff;
    line-height: 0.95;
    margin-bottom: 32px;
  }
  .cta-title span { color: var(--gold); }

  .cta-contact {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 18px;
    letter-spacing: 4px;
    color: rgba(232,232,232,0.5);
    text-transform: uppercase;
    margin-bottom: 48px;
  }

  /* FOOTER */
  footer {
    background: #050505;
    padding: 32px 24px;
    text-align: center;
    border-top: 1px solid rgba(255,255,255,0.04);
  }
  .footer-logo {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 24px;
    letter-spacing: 4px;
    color: var(--gold);
    margin-bottom: 8px;
  }
  .footer-text {
    font-family: 'Barlow Condensed', sans-serif;
    font-size: 11px;
    letter-spacing: 2px;
    color: rgba(255,255,255,0.2);
    text-transform: uppercase;
  }

  /* SCROLL REVEAL */
  .reveal {
    opacity: 0;
    transform: translateY(40px);
    transition: opacity 0.7s ease, transform 0.7s ease;
  }
  .reveal.visible {
    opacity: 1;
    transform: translateY(0);
  }
</style>
</head>
<body>

<!-- HERO -->
<div class="hero">
  <div class="ring"></div>
  <div class="ring"></div>
  <div class="ring"></div>

  <div class="badge">🇺🇸 USA Premium Vape Market</div>

  <h1 class="hero-title">
    VAPE<br>
    <span>CLOUD</span><br>
    PREMIUM
  </h1>

  <p class="hero-sub">Luxury Disposables · Wholesale Bundles · Priority US Shipping</p>

  <div class="hero-cta">
    <button class="btn-primary">Shop Premium Bundles</button>
    <button class="btn-ghost">Wholesale Inquiry</button>
  </div>
</div>

<!-- DIVIDER -->
<div class="divider" style="padding: 40px 24px;">
  <div class="divider-line"></div>
  <div class="divider-icon">◆</div>
  <div class="divider-line"></div>
</div>

<!-- BRANDS SECTION -->
<section class="reveal">
  <div class="section-label">◆ Our Brands</div>
  <h2 class="section-title">TOP-TIER<br>BRANDS ONLY</h2>
  <p style="font-size:14px; color:rgba(232,232,232,0.5); max-width:500px; line-height:1.7;">
    We carry only the most sought-after names in the premium vape market — trusted by thousands of US buyers.
  </p>

  <div class="brands-grid">
    <div class="brand-card">
      <div class="brand-name">Elf Bar</div>
      <div class="brand-tag">Most Popular</div>
    </div>
    <div class="brand-card">
      <div class="brand-name">Geek Bar</div>
      <div class="brand-tag">High Capacity</div>
    </div>
    <div class="brand-card">
      <div class="brand-name">Lost Mary</div>
      <div class="brand-tag">Luxury Flavors</div>
    </div>
    <div class="brand-card">
      <div class="brand-name">Flum</div>
      <div class="brand-tag">Smooth Hits</div>
    </div>
    <div class="brand-card">
      <div class="brand-name">RAZ</div>
      <div class="brand-tag">Fan Favorite</div>
    </div>
    <div class="brand-card">
      <div class="brand-name">Tyson</div>
      <div class="brand-tag">Limited Edition</div>
    </div>
  </div>
</section>

<!-- PROMO BANNER -->
<div class="promo-banner">
  <div class="promo-quote">
    "Luxury clouds.<br><em>Premium vibes.</em><br>Every puff worth it."
  </div>
  <div class="promo-sub">VAPE Cloud AI Premium — US Market Leader</div>
</div>

<!-- PRODUCTS SECTION -->
<section class="reveal">
  <div class="section-label">◆ Product Packages</div>
  <h2 class="section-title">PREMIUM<br>COLLECTIONS</h2>

  <div class="products-grid">
    <div class="product-card">
      <div class="product-tier">Starter</div>
      <div class="product-name">Premium Vape Starter Bundle</div>
      <div class="product-desc">2 luxury disposables, your choice of flavor. Perfect intro to the premium experience.</div>
      <div class="product-price">$50</div>
    </div>
    <div class="product-card">
      <div class="product-tier">Best Seller</div>
      <div class="product-name">5-Pack Disposable Vape Set</div>
      <div class="product-desc">Five top-brand disposables. Mix flavors or keep it consistent. Ships fast.</div>
      <div class="product-price">$75</div>
    </div>
    <div class="product-card">
      <div class="product-tier">Fan Favorite</div>
      <div class="product-name">Luxury Flavor Collection</div>
      <div class="product-desc">8 premium flavors, hand-selected from our best-selling lines. Includes priority shipping.</div>
      <div class="product-price">$120</div>
    </div>
    <div class="product-card">
      <div class="product-tier">Wholesale</div>
      <div class="product-name">Wholesale Mini Package</div>
      <div class="product-desc">Ideal for resellers. Bulk pricing, mixed or single brand. Business invoice included.</div>
      <div class="product-price">$250</div>
    </div>
    <div class="product-card">
      <div class="product-tier">VIP</div>
      <div class="product-name">VIP Bulk Order Package</div>
      <div class="product-desc">For serious buyers. Custom order, maximum discounts, free express shipping.</div>
      <div class="product-price">$500+</div>
    </div>
  </div>
</section>

<!-- FEATURES SECTION -->
<section class="reveal">
  <div class="section-label">◆ Why VAPE Cloud AI</div>
  <h2 class="section-title">BUILT FOR<br>PREMIUM BUYERS</h2>
  <div class="features-grid">
    <div class="feature-item">
      <span class="feature-icon">📦</span>
      <div class="feature-title">Fast US Shipping</div>
      <div class="feature-desc">FedEx Priority & Express options. 2–4 business days nationwide.</div>
    </div>
    <div class="feature-item">
      <span class="feature-icon">💼</span>
      <div class="feature-title">Wholesale Deals</div>
      <div class="feature-desc">Volume discounts, custom invoices, and reseller packages available.</div>
    </div>
    <div class="feature-item">
      <span class="feature-icon">🏆</span>
      <div class="feature-title">Top Brands Only</div>
      <div class="feature-desc">Elf Bar, Geek Bar, Lost Mary, Flum, RAZ, Tyson — 100% authentic.</div>
    </div>
    <div class="feature-item">
      <span class="feature-icon">🎁</span>
      <div class="feature-title">Bulk Bonuses</div>
      <div class="feature-desc">Orders $200+ get free shipping plus bonus flavors automatically.</div>
    </div>
    <div class="feature-item">
      <span class="feature-icon">📋</span>
      <div class="feature-title">Auto Invoicing</div>
      <div class="feature-desc">Professional invoice, receipt & tracking details sent with every order.</div>
    </div>
    <div class="feature-item">
      <span class="feature-icon">💬</span>
      <div class="feature-title">VIP Support</div>
      <div class="feature-desc">Direct line to a premium sales rep. Fast response, real solutions.</div>
    </div>
  </div>
</section>

<!-- SOCIAL CAPTIONS -->
<section class="reveal">
  <div class="section-label">◆ Social Content</div>
  <h2 class="section-title">READY-TO-POST<br>CAPTIONS</h2>

  <div class="captions-grid">
    <div class="caption-card">
      <div class="caption-platform">📱 TikTok</div>
      <div class="caption-text">"The vape game just changed. Premium flavors, luxury clouds, shipped straight to your door across the US 🇺🇸 Don't settle for less when you can vape the best."</div>
      <div class="caption-tags">#VapeCloud #LuxuryVape #ElfBar #GeekBar #VapeUSA #DisposableVape #PremiumVape #VapeLife</div>
    </div>
    <div class="caption-card">
      <div class="caption-platform">📸 Instagram</div>
      <div class="caption-text">"Cloud kings don't buy cheap. Shop our premium vape bundles — starting at $50. Bulk orders welcome. 🌫️✨ DM us for wholesale pricing."</div>
      <div class="caption-tags">#VapeCloudAI #LostMary #FlumVape #RazVape #TysonVape #PremiumDisposable #VapeBundle</div>
    </div>
    <div class="caption-card">
      <div class="caption-platform">👻 Snapchat</div>
      <div class="caption-text">"Snap us for the premium plug 🔥 Luxury vapes, real fast US shipping, and deals that hit harder than the flavor. VIP orders only 💨"</div>
      <div class="caption-tags">#VapeDeals #VapeShop #PremiumVapes #BulkVape #VapeWholesale #USShipping</div>
    </div>
  </div>
</section>

<!-- CTA SECTION -->
<div class="cta-section reveal">
  <h2 class="cta-title">ORDER<br><span>TODAY.</span><br>SHIP FAST.</h2>
  <div class="cta-contact">DM to Order · Wholesale Inquiries Welcome · US Nationwide</div>
  <div style="display:flex; gap:16px; justify-content:center; flex-wrap:wrap;">
    <button class="btn-primary">Start Your Order</button>
    <button class="btn-ghost">Request Wholesale Quote</button>
  </div>
</div>

<!-- FOOTER -->
<footer>
  <div class="footer-logo">VAPE CLOUD AI</div>
  <div class="footer-text">Premium Vape Business · United States · Est. 2026</div>
</footer>

<script>
  // Scroll reveal
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) {
        e.target.classList.add('visible');
        observer.unobserve(e.target);
      }
    });
  }, { threshold: 0.1 });
  reveals.forEach(r => observer.observe(r));
</script>
</body>
</html>
