<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Taher Betwala | Property Consultant — Dubai</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,500;1,600&family=Jost:wght@400;500;600;700&display=swap" rel="stylesheet"/>
<style>
:root {
  --bg:       #F5F0E8;
  --bg2:      #EDE8DE;
  --bg3:      #E4DDD2;
  --card:     #FDFAF5;
  --mocha:    #5C3D2E;
  --mocha2:   #4A3025;
  --bronze:   #9A6B3F;
  --bronze2:  #B5824E;
  --taupe:    #6B5B4E;
  --espresso: #241810;
  --sand:     #8A7465;
  --border:   #CABFB2;
  --border2:  #B8AA9A;
  --text:     #241810;
  --muted:    #6B5B4E;
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Jost', sans-serif;
  font-weight: 400;
  overflow-x: hidden;
  line-height: 1.6;
}

body::before {
  content: '';
  position: fixed; inset: 0; z-index: 0;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='300'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.75' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='300' height='300' filter='url(%23n)' opacity='0.025'/%3E%3C/svg%3E");
  pointer-events: none;
}

/* ══════════════ NAV ══════════════ */
nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 200;
  display: flex; justify-content: space-between; align-items: center;
  padding: 1.1rem 3.5rem;
  background: rgba(245,240,232,0.95);
  backdrop-filter: blur(16px);
  border-bottom: 1.5px solid var(--border);
}
.nav-brand-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.05rem; font-weight: 600;
  color: var(--mocha); letter-spacing: 0.04em;
}
.nav-brand-sub {
  font-size: 0.63rem; letter-spacing: 0.22em; text-transform: uppercase;
  color: var(--sand); margin-top: 2px; font-weight: 500;
}
.nav-links { display: flex; gap: 2.2rem; align-items: center; }
.nav-links a {
  color: var(--taupe); text-decoration: none;
  font-size: 0.76rem; letter-spacing: 0.14em; text-transform: uppercase;
  font-weight: 600; transition: color 0.3s;
}
.nav-links a:hover { color: var(--bronze); }
.nav-cta {
  background: var(--bronze) !important;
  color: #fff !important;
  padding: 0.52rem 1.4rem;
  font-size: 0.74rem !important;
  font-weight: 600 !important;
  transition: background 0.3s !important;
}
.nav-cta:hover { background: var(--mocha) !important; }

/* ══════════════ HERO ══════════════ */
.hero {
  min-height: 100vh;
  display: grid; grid-template-columns: 1fr 1fr;
  padding: 9rem 3.5rem 5rem;
  gap: 5rem; max-width: 1280px; margin: 0 auto;
  align-items: center; position: relative; z-index: 1;
}
.hero::after {
  content: '';
  position: absolute; right: -60px; top: 12%; bottom: 12%;
  width: 340px;
  border: 1px solid rgba(154,107,63,0.13);
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
  pointer-events: none;
}

.hero-left { display: flex; flex-direction: column; }

.eyebrow {
  display: flex; align-items: center; gap: 0.9rem;
  font-size: 0.7rem; letter-spacing: 0.32em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 1.8rem; font-weight: 600;
  animation: fadeUp 0.7s 0.1s ease both;
}
.eyebrow-line { width: 2.5rem; height: 1.5px; background: var(--bronze); }

h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.8rem, 5.5vw, 5rem);
  font-weight: 700; line-height: 1.07; color: var(--espresso);
  margin-bottom: 1.5rem;
  animation: fadeUp 0.7s 0.2s ease both;
}
h1 em { font-style: italic; color: var(--bronze); font-weight: 600; }

.hero-desc {
  font-size: 1rem; color: var(--taupe); font-weight: 400;
  line-height: 1.85; max-width: 420px; margin-bottom: 2.5rem;
  animation: fadeUp 0.7s 0.3s ease both;
}
.hero-desc strong { color: var(--espresso); font-weight: 600; }

.hero-stats {
  display: flex; gap: 2.8rem; margin-bottom: 3rem;
  animation: fadeUp 0.7s 0.4s ease both;
}
.stat { border-left: 2.5px solid var(--border2); padding-left: 1.2rem; }
.stat-val {
  font-family: 'Playfair Display', serif;
  font-size: 2.2rem; color: var(--mocha); font-weight: 700; line-height: 1;
}
.stat-lbl {
  font-size: 0.67rem; letter-spacing: 0.16em; text-transform: uppercase;
  color: var(--sand); margin-top: 0.4rem; font-weight: 600;
}

.hero-btns {
  display: flex; gap: 1rem; flex-wrap: wrap;
  animation: fadeUp 0.7s 0.5s ease both;
}
.btn-wa {
  display: inline-flex; align-items: center; gap: 0.6rem;
  background: #25D366; color: #fff;
  padding: 0.9rem 1.9rem; text-decoration: none;
  font-size: 0.8rem; letter-spacing: 0.13em; text-transform: uppercase;
  font-weight: 600; transition: background 0.3s, transform 0.2s;
}
.btn-wa:hover { background: #1cb85a; transform: translateY(-2px); }
.btn-call {
  display: inline-flex; align-items: center; gap: 0.6rem;
  background: transparent; color: var(--mocha);
  border: 2px solid var(--mocha);
  padding: 0.9rem 1.9rem; text-decoration: none;
  font-size: 0.8rem; letter-spacing: 0.13em; text-transform: uppercase;
  font-weight: 600; transition: all 0.3s;
}
.btn-call:hover { background: var(--mocha); color: #fff; transform: translateY(-2px); }

/* ── PROFILE CARD ── */
.profile-card {
  background: var(--card);
  border: 1.5px solid var(--border);
  padding: 2.8rem;
  box-shadow: 0 10px 56px rgba(92,61,46,0.11), 0 2px 14px rgba(92,61,46,0.06);
  position: relative;
  animation: fadeUp 0.9s 0.35s ease both;
}
.profile-card::before {
  content: '';
  position: absolute; top: 0; left: 0; right: 0; height: 4px;
  background: linear-gradient(90deg, var(--bronze), var(--mocha));
}

.photo-wrap { display: flex; justify-content: center; margin-bottom: 1.8rem; }
.photo-circle {
  width: 115px; height: 115px; border-radius: 50%;
  background: var(--bg2);
  border: 3px solid var(--border2);
  display: flex; flex-direction: column;
  align-items: center; justify-content: center;
  overflow: hidden; position: relative;
}
/* ── TAHER — UPLOAD YOUR PHOTO HERE ──────────────────────────
   1. Upload your photo file (e.g. taher-photo.jpg) to GitHub
      in the same folder as this index.html file
   2. Delete the <svg> and <div class="photo-label"> below
   3. Paste this in their place:
      <img src="taher-photo.jpg" alt="Taher Betwala"
           style="width:100%;height:100%;object-fit:cover;border-radius:50%;"/>
   ──────────────────────────────────────────────────────────── */
.photo-silhouette { width: 44px; height: 44px; fill: var(--border2); }
.photo-label {
  font-size: 0.54rem; letter-spacing: 0.1em; text-transform: uppercase;
  color: var(--sand); margin-top: 4px; font-weight: 600;
}

.card-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.75rem; font-weight: 700;
  text-align: center; color: var(--espresso); margin-bottom: 0.3rem;
}
.card-title {
  font-size: 0.7rem; letter-spacing: 0.22em; text-transform: uppercase;
  color: var(--bronze); text-align: center; font-weight: 700; margin-bottom: 0.3rem;
}
.card-company {
  font-size: 0.82rem; color: var(--taupe); font-weight: 500;
  text-align: center; margin-bottom: 1.6rem;
}
.card-divider { height: 1.5px; background: var(--border); margin: 0 0 1.5rem; }

.card-row { display: flex; align-items: flex-start; gap: 0.9rem; margin-bottom: 1rem; }
.card-icon { font-size: 1.05rem; flex-shrink: 0; margin-top: 1px; }
.card-row-label {
  font-size: 0.63rem; letter-spacing: 0.15em; text-transform: uppercase;
  color: var(--sand); margin-bottom: 2px; font-weight: 600;
}
.card-row-val { font-size: 0.92rem; color: var(--espresso); font-weight: 500; }

.spec-row { display: flex; flex-wrap: wrap; gap: 0.5rem; margin-top: 1.5rem; }
.spec-tag {
  background: var(--bg2); border: 1.5px solid var(--border2);
  color: var(--mocha); padding: 0.3rem 0.85rem;
  font-size: 0.67rem; letter-spacing: 0.13em;
  text-transform: uppercase; font-weight: 600;
}

/* ══════════════ SECTION SHELL ══════════════ */
.section-outer { position: relative; z-index: 1; }
.section-inner { max-width: 1280px; margin: 0 auto; padding: 6rem 3.5rem; }

.sec-eyebrow {
  display: flex; align-items: center; gap: 0.8rem;
  font-size: 0.67rem; letter-spacing: 0.32em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 0.9rem; font-weight: 700;
}
.sec-eyebrow::before { content: ''; width: 2rem; height: 1.5px; background: var(--bronze); }

h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2rem, 4vw, 3.1rem);
  font-weight: 700; color: var(--espresso);
  line-height: 1.18; margin-bottom: 0.8rem;
}
h2 em { font-style: italic; color: var(--bronze); }

.sec-subtitle {
  font-size: 0.95rem; color: var(--taupe); font-weight: 400;
  line-height: 1.85; margin-bottom: 3.5rem; max-width: 540px;
}

/* ══════════════ DEVELOPERS ══════════════ */
.dev-section { background: var(--bg2); }

.dev-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }

.dev-card {
  background: var(--card); border: 1.5px solid var(--border);
  padding: 2.2rem 2rem; position: relative; overflow: hidden;
  transition: box-shadow 0.3s, transform 0.3s, border-color 0.3s;
}
.dev-card:hover {
  box-shadow: 0 14px 44px rgba(92,61,46,0.13);
  transform: translateY(-5px);
  border-color: var(--bronze);
}
.dev-card::after {
  content: attr(data-num);
  position: absolute; bottom: -0.8rem; right: 1.2rem;
  font-family: 'Playfair Display', serif;
  font-size: 5.5rem; color: rgba(154,107,63,0.07);
  line-height: 1; pointer-events: none; user-select: none; font-weight: 700;
}
.dev-icon { font-size: 1.7rem; margin-bottom: 1rem; }
.dev-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.25rem; font-weight: 700;
  color: var(--mocha); margin-bottom: 0.3rem;
}
.dev-type {
  font-size: 0.64rem; letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 1rem; font-weight: 700;
}
.dev-desc {
  font-size: 0.86rem; color: var(--taupe);
  line-height: 1.82; font-weight: 400;
}
.dev-areas { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 1.3rem; }
.area-pill {
  font-size: 0.62rem; letter-spacing: 0.1em; text-transform: uppercase;
  color: var(--taupe); background: var(--bg2); border: 1px solid var(--border2);
  padding: 0.24rem 0.7rem; font-weight: 600;
}

/* ══════════════ LISTINGS ══════════════ */
.listings-section { background: var(--bg); }

.filters { display: flex; gap: 0.7rem; flex-wrap: wrap; margin-bottom: 2.5rem; }
.filter-btn {
  padding: 0.58rem 1.5rem; border: 2px solid var(--border2);
  background: transparent; color: var(--taupe);
  font-family: 'Jost', sans-serif; font-size: 0.74rem;
  letter-spacing: 0.15em; text-transform: uppercase;
  cursor: pointer; font-weight: 600; transition: all 0.25s;
}
.filter-btn:hover { border-color: var(--bronze); color: var(--bronze); }
.filter-btn.active { background: var(--mocha); color: #fff; border-color: var(--mocha); }

.table-wrap { overflow-x: auto; }
table { width: 100%; border-collapse: collapse; }
thead tr { border-bottom: 2.5px solid var(--mocha); }
thead th {
  text-align: left; padding: 0.95rem 1.1rem;
  font-size: 0.64rem; letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--mocha); font-weight: 700; white-space: nowrap;
  font-family: 'Jost', sans-serif;
}
tbody tr { border-bottom: 1px solid var(--border); transition: background 0.2s; }
tbody tr:hover { background: var(--bg2); }
tbody td {
  padding: 1.1rem 1.1rem; color: var(--taupe);
  font-size: 0.87rem; vertical-align: middle; font-weight: 400;
}
.prop-name { font-weight: 600; color: var(--espresso) !important; }
.prop-num { color: var(--sand) !important; font-size: 0.8rem !important; font-weight: 600 !important; }
.prop-dev { font-weight: 600; color: var(--mocha) !important; }
.prop-loc { font-weight: 500; }
.prop-price { color: var(--mocha) !important; font-weight: 700 !important; white-space: nowrap; }

.badge {
  display: inline-block; padding: 0.25rem 0.8rem;
  font-size: 0.62rem; letter-spacing: 0.12em;
  text-transform: uppercase; font-weight: 700;
}
.badge-sell    { background: rgba(92,61,46,0.1);   color: var(--mocha);  }
.badge-rent    { background: rgba(154,107,63,0.13); color: var(--bronze); }
.badge-offplan { background: rgba(80,130,80,0.1);   color: #4a7a4a;       }

.enquire-link {
  display: inline-flex; align-items: center; gap: 0.4rem;
  color: #25D366; text-decoration: none;
  font-size: 0.74rem; letter-spacing: 0.1em; text-transform: uppercase;
  font-weight: 700; border-bottom: 1.5px solid transparent;
  transition: border-color 0.2s, color 0.2s;
}
.enquire-link:hover { border-color: #25D366; }

.empty-row { text-align: center !important; padding: 3rem !important; color: var(--sand) !important; font-weight: 500 !important; }

/* ══════════════ CONTACT STRIP ══════════════ */
.contact-strip {
  background: var(--mocha); padding: 5.5rem 3.5rem;
  position: relative; z-index: 1; overflow: hidden;
}
.contact-strip::before {
  content: '';
  position: absolute; right: -100px; top: -120px;
  width: 420px; height: 420px; border-radius: 50%;
  background: rgba(255,255,255,0.03); pointer-events: none;
}
.contact-strip::after {
  content: '';
  position: absolute; left: -60px; bottom: -80px;
  width: 280px; height: 280px; border-radius: 50%;
  background: rgba(255,255,255,0.025); pointer-events: none;
}
.contact-inner {
  max-width: 1280px; margin: 0 auto;
  display: flex; justify-content: space-between; align-items: center;
  flex-wrap: wrap; gap: 2.5rem; position: relative; z-index: 2;
}
.contact-left h2 { color: var(--bg); margin-bottom: 0.6rem; }
.contact-left p {
  color: rgba(245,240,232,0.7); font-size: 0.95rem; font-weight: 400;
}
.contact-btns { display: flex; gap: 1rem; flex-wrap: wrap; }
.btn-wa-lg {
  display: inline-flex; align-items: center; gap: 0.7rem;
  background: #25D366; color: #fff;
  padding: 1.05rem 2.3rem; text-decoration: none;
  font-size: 0.84rem; letter-spacing: 0.15em; text-transform: uppercase;
  font-weight: 600; transition: all 0.3s;
}
.btn-wa-lg:hover { background: #1cb85a; transform: translateY(-2px); }
.btn-call-lg {
  display: inline-flex; align-items: center; gap: 0.7rem;
  background: transparent; color: var(--bg);
  border: 2px solid rgba(245,240,232,0.45);
  padding: 1.05rem 2.3rem; text-decoration: none;
  font-size: 0.84rem; letter-spacing: 0.15em; text-transform: uppercase;
  font-weight: 600; transition: all 0.3s;
}
.btn-call-lg:hover { border-color: var(--bg); transform: translateY(-2px); }

/* ══════════════ FOOTER ══════════════ */
footer {
  background: var(--espresso); padding: 4rem 3.5rem;
  position: relative; z-index: 1; text-align: center;
}
.footer-name {
  font-family: 'Playfair Display', serif;
  font-size: 2rem; font-weight: 700; color: var(--bg); margin-bottom: 0.35rem;
}
.footer-role {
  font-size: 0.67rem; letter-spacing: 0.25em; text-transform: uppercase;
  color: var(--sand); margin-bottom: 1.8rem; font-weight: 600;
}
.footer-contact-row {
  display: flex; justify-content: center; gap: 2.8rem; flex-wrap: wrap;
  margin-bottom: 1.6rem;
}
.footer-contact-item {
  display: flex; align-items: center; gap: 0.5rem;
  font-size: 0.86rem; color: var(--bg2); text-decoration: none;
  font-weight: 500; transition: color 0.2s;
}
.footer-contact-item:hover { color: var(--bronze2); }

/* Social row — hidden, ready to activate */
.social-row {
  display: none; /* TO ACTIVATE: change to display:flex */
  gap: 1.2rem; justify-content: center; margin-bottom: 1.6rem;
}
/* Instagram → https://www.instagram.com/habibi_chalodubai/         */
/* Facebook  → https://www.facebook.com/profile.php?id=61580013579727 */
.social-link {
  font-size: 0.74rem; letter-spacing: 0.13em; text-transform: uppercase;
  color: var(--sand); text-decoration: none; font-weight: 600;
  transition: color 0.2s;
}
.social-link:hover { color: var(--bronze2); }

.footer-divider { height: 1px; background: rgba(255,255,255,0.07); margin: 1.6rem 0; }
.footer-copy { font-size: 0.67rem; letter-spacing: 0.1em; color: var(--sand); font-weight: 500; }

/* ══════════════ MOBILE STICKY ══════════════ */
.mobile-sticky {
  display: none; position: fixed; bottom: 0; left: 0; right: 0; z-index: 300;
  grid-template-columns: 1fr 1fr;
  border-top: 1.5px solid var(--border);
}
.mob-btn {
  display: flex; align-items: center; justify-content: center; gap: 0.5rem;
  padding: 1rem; text-decoration: none;
  font-size: 0.78rem; letter-spacing: 0.12em; text-transform: uppercase; font-weight: 600;
}
.mob-btn-wa   { background: #25D366; color: #fff; }
.mob-btn-call { background: var(--mocha); color: #fff; }

/* ══════════════ ANIMATIONS ══════════════ */
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(22px); }
  to   { opacity: 1; transform: translateY(0); }
}

/* ══════════════ RESPONSIVE ══════════════ */
@media (max-width: 1024px) {
  .hero { grid-template-columns: 1fr; gap: 3rem; padding: 8rem 2rem 4rem; }
  .hero::after { display: none; }
  .dev-grid { grid-template-columns: 1fr 1fr; }
  .section-inner { padding: 4.5rem 2rem; }
  nav { padding: 1rem 2rem; }
}
@media (max-width: 768px) {
  nav { padding: 1rem 1.5rem; }
  .nav-links a:not(.nav-cta) { display: none; }
  .hero { padding: 7.5rem 1.5rem 3rem; }
  .hero-stats { gap: 1.5rem; }
  .dev-grid { grid-template-columns: 1fr; }
  .contact-inner { flex-direction: column; text-align: center; }
  .contact-btns { justify-content: center; }
  .footer-contact-row { flex-direction: column; gap: 1rem; align-items: center; }
  .mobile-sticky { display: grid; }
  body { padding-bottom: 62px; }
  .section-inner { padding: 3.5rem 1.5rem; }
}
</style>
</head>
<body>

<!-- ══ NAV ══ -->
<nav>
  <div>
    <div class="nav-brand-name">New Heights Real Estate</div>
    <div class="nav-brand-sub">Dubai · UAE</div>
  </div>
  <div class="nav-links">
    <a href="#developers">Developers</a>
    <a href="#listings">Listings</a>
    <a href="#contact">Contact</a>
    <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!%20%F0%9F%94%91" target="_blank" class="nav-cta">WhatsApp</a>
  </div>
</nav>

<!-- ══ HERO ══ -->
<section style="position:relative;z-index:1;">
  <div class="hero">

    <div class="hero-left">
      <div class="eyebrow"><span class="eyebrow-line"></span>Dubai Real Estate</div>
      <h1>Your Property<br><em>Expert</em> in<br>Dubai</h1>
      <p class="hero-desc">
        Whether you're buying, selling, or renting — I guide you through Dubai's market with
        <strong>10+ years of hands-on expertise</strong> across the city's most prestigious communities.
      </p>
      <div class="hero-stats">
        <div class="stat">
          <div class="stat-val">10+</div>
          <div class="stat-lbl">Years in Dubai</div>
        </div>
        <div class="stat">
          <div class="stat-val">7+</div>
          <div class="stat-lbl">Top Developers</div>
        </div>
        <div class="stat">
          <div class="stat-val">Buy · Sell · Rent</div>
          <div class="stat-lbl">All Covered</div>
        </div>
      </div>
      <div class="hero-btns">
        <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!%20%F0%9F%94%91" target="_blank" class="btn-wa">💬 WhatsApp Me</a>
        <a href="tel:+971556472153" class="btn-call">📞 +971 55647 2153</a>
      </div>
    </div>

    <!-- PROFILE CARD -->
    <div class="profile-card">
      <div class="photo-wrap">
        <div class="photo-circle">
          <!-- TAHER — UPLOAD YOUR PHOTO HERE ─────────────────────────
               1. Upload your photo (e.g. taher-photo.jpg) to GitHub
                  in the same folder as this index.html file
               2. Delete the <svg> tag and <div class="photo-label"> below
               3. Paste this line in their place:
                  <img src="taher-photo.jpg" alt="Taher Betwala"
                       style="width:100%;height:100%;object-fit:cover;border-radius:50%;"/>
               ──────────────────────────────────────────────────────── -->
          <svg class="photo-silhouette" viewBox="0 0 80 80" xmlns="http://www.w3.org/2000/svg">
            <circle cx="40" cy="28" r="16" fill="#CABFB2"/>
            <ellipse cx="40" cy="70" rx="26" ry="18" fill="#CABFB2"/>
          </svg>
          <div class="photo-label">Your Photo</div>
        </div>
      </div>

      <div class="card-name">Taher Betwala</div>
      <div class="card-title">Property Consultant — Dubai</div>
      <div class="card-company">New Heights Real Estate</div>
      <div class="card-divider"></div>

      <div class="card-row">
        <div class="card-icon">📱</div>
        <div>
          <div class="card-row-label">Mobile / WhatsApp</div>
          <div class="card-row-val">+971 55647 2153</div>
        </div>
      </div>
      <div class="card-row">
        <div class="card-icon">📍</div>
        <div>
          <div class="card-row-label">Location</div>
          <div class="card-row-val">Dubai, United Arab Emirates</div>
        </div>
      </div>
      <div class="card-row">
        <div class="card-icon">🏢</div>
        <div>
          <div class="card-row-label">Company</div>
          <div class="card-row-val">New Heights Real Estate</div>
        </div>
      </div>
      <div class="card-row">
        <div class="card-icon">⭐</div>
        <div>
          <div class="card-row-label">Experience</div>
          <div class="card-row-val">10+ Years — Dubai Market</div>
        </div>
      </div>

      <div class="spec-row">
        <span class="spec-tag">Buy</span>
        <span class="spec-tag">Sell</span>
        <span class="spec-tag">Rent</span>
        <span class="spec-tag">Off-Plan</span>
        <span class="spec-tag">Investment</span>
      </div>
    </div>

  </div>
</section>

<!-- ══ DEVELOPERS ══ -->
<div class="section-outer dev-section" id="developers">
  <div class="section-inner">
    <div class="sec-eyebrow">Our Network</div>
    <h2>Dubai's Top Developers —<br><em>All Under One Roof</em></h2>
    <p class="sec-subtitle">From iconic master communities to boutique luxury residences — I work across every major developer in Dubai so you always find the right fit.</p>

    <div class="dev-grid">

      <div class="dev-card" data-num="01">
        <div class="dev-icon">🏙️</div>
        <div class="dev-name">Emaar Properties</div>
        <div class="dev-type">Master-Planned Communities</div>
        <div class="dev-desc">Dubai's most iconic developer — creators of Burj Khalifa, Dubai Mall, and Downtown Dubai. Trusted for world-class amenities and strong capital appreciation.</div>
        <div class="dev-areas">
          <span class="area-pill">Downtown Dubai</span>
          <span class="area-pill">Dubai Marina</span>
          <span class="area-pill">Arabian Ranches</span>
          <span class="area-pill">Creek Harbour</span>
        </div>
      </div>

      <div class="dev-card" data-num="02">
        <div class="dev-icon">💎</div>
        <div class="dev-name">DAMAC Properties</div>
        <div class="dev-type">Luxury & Branded Residences</div>
        <div class="dev-desc">High-end developer with bold branded collaborations — Cavalli, Versace, Rotana. Popular with investors for premium finishes and strong rental returns.</div>
        <div class="dev-areas">
          <span class="area-pill">Business Bay</span>
          <span class="area-pill">DAMAC Hills</span>
          <span class="area-pill">Safa Park</span>
          <span class="area-pill">Akoya</span>
        </div>
      </div>

      <div class="dev-card" data-num="03">
        <div class="dev-icon">🌊</div>
        <div class="dev-name">Nakheel</div>
        <div class="dev-type">Waterfront Living</div>
        <div class="dev-desc">Creator of Palm Jumeirah and The World Islands. Nakheel builds waterfront communities and family clusters — ideal for lifestyle buyers and long-term investors.</div>
        <div class="dev-areas">
          <span class="area-pill">Palm Jumeirah</span>
          <span class="area-pill">Jumeirah Village</span>
          <span class="area-pill">Al Furjan</span>
          <span class="area-pill">Deira Islands</span>
        </div>
      </div>

      <div class="dev-card" data-num="04">
        <div class="dev-icon">🏡</div>
        <div class="dev-name">Sobha Realty</div>
        <div class="dev-type">Self-Built Quality</div>
        <div class="dev-desc">Renowned for in-house construction with zero outsourcing — delivering superior build quality and finish. Sobha Hartland in MBR City is their flagship green community.</div>
        <div class="dev-areas">
          <span class="area-pill">MBR City</span>
          <span class="area-pill">Sobha Hartland</span>
          <span class="area-pill">Hartland II</span>
        </div>
      </div>

      <div class="dev-card" data-num="05">
        <div class="dev-icon">🎨</div>
        <div class="dev-name">Meraas</div>
        <div class="dev-type">Lifestyle & Culture</div>
        <div class="dev-desc">Lifestyle-driven developer behind City Walk, Bluewaters Island, and Port De La Mer. Meraas blends culture, retail, and contemporary living in prime walkable areas.</div>
        <div class="dev-areas">
          <span class="area-pill">City Walk</span>
          <span class="area-pill">Bluewaters Island</span>
          <span class="area-pill">Port De La Mer</span>
          <span class="area-pill">La Mer</span>
        </div>
      </div>

      <div class="dev-card" data-num="06">
        <div class="dev-icon">🏛️</div>
        <div class="dev-name">Dubai Properties</div>
        <div class="dev-type">Government-Backed Value</div>
        <div class="dev-desc">A government-backed developer offering communities from affordable to mid-range. Trusted for consistent long-term value, solid infrastructure, and family-friendly layouts.</div>
        <div class="dev-areas">
          <span class="area-pill">JBR</span>
          <span class="area-pill">Mudon</span>
          <span class="area-pill">Villanova</span>
          <span class="area-pill">Culture Village</span>
        </div>
      </div>

      <div class="dev-card" data-num="07">
        <div class="dev-icon">✨</div>
        <div class="dev-name">Danube Properties</div>
        <div class="dev-type">Affordable Luxury</div>
        <div class="dev-desc">One of Dubai's fastest-growing developers — making luxury accessible with flexible payment plans, high-quality finishes, and strong ROI. Ideal for first-time buyers and savvy investors.</div>
        <div class="dev-areas">
          <span class="area-pill">Arjan</span>
          <span class="area-pill">Jumeirah Village Circle</span>
          <span class="area-pill">Al Furjan</span>
          <span class="area-pill">Sports City</span>
        </div>
      </div>

    </div>
  </div>
</div>

<!-- ══ LISTINGS ══ -->
<div class="section-outer listings-section" id="listings">
  <div class="section-inner">
    <div class="sec-eyebrow">Available Properties</div>
    <h2>Current <em>Listings</em></h2>
    <p class="sec-subtitle">Browse available properties across Dubai — updated regularly. Click Enquire on any listing to connect with me directly on WhatsApp with full property details.</p>

    <div class="filters">
      <button class="filter-btn active" onclick="filterListings('all',this)">All Properties</button>
      <button class="filter-btn" onclick="filterListings('sell',this)">For Sale</button>
      <button class="filter-btn" onclick="filterListings('rent',this)">For Rent</button>
      <button class="filter-btn" onclick="filterListings('offplan',this)">Off-Plan</button>
    </div>

    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>#</th>
            <th>Property</th>
            <th>Type</th>
            <th>Developer</th>
            <th>Location</th>
            <th>Beds</th>
            <th>Size (sqft)</th>
            <th>Price (AED)</th>
            <th>Status</th>
            <th>Enquire</th>
          </tr>
        </thead>
        <tbody id="listingsBody"></tbody>
      </table>
    </div>
  </div>
</div>

<!-- ══ CONTACT STRIP ══ -->
<div class="contact-strip" id="contact">
  <div class="contact-inner">
    <div class="contact-left">
      <h2>Let's Find Your<br><em>Perfect Property</em></h2>
      <p>Reach out today — response within the hour.</p>
    </div>
    <div class="contact-btns">
      <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!%20%F0%9F%94%91" target="_blank" class="btn-wa-lg">💬 WhatsApp</a>
      <a href="tel:+971556472153" class="btn-call-lg">📞 Call Now</a>
    </div>
  </div>
</div>

<!-- ══ FOOTER ══ -->
<footer>
  <div class="footer-name">Taher Betwala</div>
  <div class="footer-role">Property Consultant — Dubai · New Heights Real Estate</div>

  <!-- SOCIAL ROW — HIDDEN UNTIL READY
       To activate: find .social-row in CSS above and change display:none → display:flex -->
  <div class="social-row">
    <a href="https://www.instagram.com/habibi_chalodubai/" target="_blank" class="social-link">📸 Instagram</a>
    <a href="https://www.facebook.com/profile.php?id=61580013579727" target="_blank" class="social-link">👍 Facebook</a>
  </div>

  <div class="footer-contact-row">
    <a href="tel:+971556472153" class="footer-contact-item">📞 +971 55647 2153</a>
    <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!%20%F0%9F%94%91" target="_blank" class="footer-contact-item">💬 WhatsApp</a>
    <span class="footer-contact-item">📍 Dubai, UAE</span>
  </div>

  <div class="footer-divider"></div>
  <div class="footer-copy">© 2025 Taher Betwala · New Heights Real Estate · All Rights Reserved</div>
</footer>

<!-- ══ MOBILE STICKY BUTTONS ══ -->
<div class="mobile-sticky">
  <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!%20%F0%9F%94%91" target="_blank" class="mob-btn mob-btn-wa">💬 WhatsApp</a>
  <a href="tel:+971556472153" class="mob-btn mob-btn-call">📞 Call</a>
</div>

<script>
// ═══════════════════════════════════════════════════════════════════
//   TAHER — ADD YOUR LISTINGS HERE
//   Copy one block, fill in details, save & push to GitHub
//   status: "sell" | "rent" | "offplan"
// ═══════════════════════════════════════════════════════════════════
const listings = [
  {
    id: 1,
    name: "Harbour Gate — Tower 1",
    type: "Apartment",
    developer: "Emaar",
    location: "Creek Harbour",
    beds: "1 BR",
    size: "780",
    price: "1,450,000",
    status: "sell"
  },
  {
    id: 2,
    name: "DAMAC Volta",
    type: "Apartment",
    developer: "DAMAC",
    location: "Downtown Dubai",
    beds: "2 BR",
    size: "1,250",
    price: "18,000 / mo",
    status: "rent"
  },
  {
    id: 3,
    name: "Sobha Hartland — Greens",
    type: "Villa",
    developer: "Sobha",
    location: "MBR City",
    beds: "4 BR",
    size: "3,800",
    price: "6,500,000",
    status: "sell"
  },
  {
    id: 4,
    name: "Palm Beach Towers",
    type: "Apartment",
    developer: "Nakheel",
    location: "Palm Jumeirah",
    beds: "3 BR",
    size: "2,100",
    price: "35,000 / mo",
    status: "rent"
  },
  {
    id: 5,
    name: "Elo — Phase 2",
    type: "Townhouse",
    developer: "DAMAC",
    location: "DAMAC Hills 2",
    beds: "3 BR",
    size: "1,900",
    price: "1,750,000",
    status: "offplan"
  },
  {
    id: 6,
    name: "Bluewaters Residences",
    type: "Apartment",
    developer: "Meraas",
    location: "Bluewaters Island",
    beds: "2 BR",
    size: "1,400",
    price: "4,200,000",
    status: "sell"
  },
  {
    id: 7,
    name: "Danube Opalz",
    type: "Apartment",
    developer: "Danube",
    location: "Arjan",
    beds: "Studio",
    size: "450",
    price: "680,000",
    status: "offplan"
  },
];
// ═══════════════════════════════════════════════════════════════════

const statusMap = {
  sell:    { label: "For Sale",  cls: "badge-sell"    },
  rent:    { label: "For Rent",  cls: "badge-rent"    },
  offplan: { label: "Off-Plan",  cls: "badge-offplan" },
};

function buildWaLink(p) {
  const statusLabel = statusMap[p.status]?.label || p.status;
  const msg =
    `Hi Taher! I'm interested in the following property:%0A` +
    `%F0%9F%8F%A0 *${p.name}*%0A` +
    `%F0%9F%93%8D Location: ${p.location}%0A` +
    `%F0%9F%9B%8F Type: ${p.type} | ${p.beds} | ${p.size} sqft%0A` +
    `%F0%9F%92%B0 Price: AED ${p.price} | ${statusLabel}%0A` +
    `Can we discuss further? %F0%9F%94%91`;
  return `https://wa.me/971556472153?text=${msg}`;
}

function renderListings(data) {
  const body = document.getElementById('listingsBody');
  body.innerHTML = '';
  if (!data.length) {
    body.innerHTML = `<tr><td colspan="10" class="empty-row">No listings found for this filter.</td></tr>`;
    return;
  }
  data.forEach(p => {
    const s = statusMap[p.status] || statusMap.sell;
    body.innerHTML += `
      <tr>
        <td class="prop-num">${p.id}</td>
        <td class="prop-name">${p.name}</td>
        <td>${p.type}</td>
        <td class="prop-dev">${p.developer}</td>
        <td class="prop-loc">${p.location}</td>
        <td>${p.beds}</td>
        <td>${p.size}</td>
        <td class="prop-price">${p.price}</td>
        <td><span class="badge ${s.cls}">${s.label}</span></td>
        <td>
          <a href="${buildWaLink(p)}" target="_blank" class="enquire-link">💬 Enquire</a>
        </td>
      </tr>`;
  });
}

function filterListings(type, btn) {
  document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  renderListings(type === 'all' ? listings : listings.filter(l => l.status === type));
}

renderListings(listings);
</script>
</body>
</html>
