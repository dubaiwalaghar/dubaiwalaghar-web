<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Taher Betwala | Property Consultant, Dubai</title>
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

/* ── NAV ── */
nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 200;
  display: flex; justify-content: center; align-items: center;
  padding: 1.1rem 3.5rem;
  background: rgba(245,240,232,0.96);
  backdrop-filter: blur(16px);
  border-bottom: 1.5px solid var(--border);
}
.nav-brand { display: flex; flex-direction: column; align-items: center; }
.nav-brand-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.45rem; font-weight: 700;
  color: var(--mocha); letter-spacing: 0.07em; line-height: 1;
}
.nav-brand-sub {
  font-size: 0.58rem; letter-spacing: 0.28em; text-transform: uppercase;
  color: var(--bronze); margin-top: 4px; font-weight: 700;
}

/* ── HERO ── */
.hero {
  display: grid; grid-template-columns: 1fr 1fr;
  padding: 5rem 3.5rem 2rem;
  gap: 3.5rem; max-width: 1280px; margin: 0 auto;
  align-items: center; position: relative; z-index: 1;
}
.hero-left { display: flex; flex-direction: column; }
.eyebrow {
  display: flex; align-items: center; gap: 0.9rem;
  font-size: 0.68rem; letter-spacing: 0.3em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 1rem; font-weight: 600;
  animation: fadeUp 0.7s 0.1s ease both;
}
.eyebrow-line { width: 2.2rem; height: 1.5px; background: var(--bronze); }
h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.5rem, 4.5vw, 4.2rem);
  font-weight: 700; line-height: 1.08; color: var(--espresso);
  margin-bottom: 1.2rem;
  animation: fadeUp 0.7s 0.2s ease both;
}
h1 em { font-style: italic; color: var(--bronze); font-weight: 600; }
.hero-desc {
  font-size: 0.95rem; color: var(--taupe); font-weight: 400;
  line-height: 1.85; max-width: 400px; margin-bottom: 1.3rem;
  animation: fadeUp 0.7s 0.3s ease both;
}
.hero-desc strong { color: var(--espresso); font-weight: 600; }
.hero-stats {
  display: flex; gap: 2.2rem;
  animation: fadeUp 0.7s 0.4s ease both;
}
.stat { border-left: 2.5px solid var(--border2); padding-left: 1.1rem; }
.stat-val {
  font-family: 'Playfair Display', serif;
  font-size: 1.9rem; color: var(--mocha); font-weight: 700; line-height: 1;
}
.stat-lbl {
  font-size: 0.62rem; letter-spacing: 0.14em; text-transform: uppercase;
  color: var(--sand); margin-top: 0.3rem; font-weight: 600;
}

/* ── PROFILE CARD ── */
.profile-card {
  background: var(--card);
  border: 1.5px solid var(--border);
  padding: 2.4rem;
  box-shadow: 0 10px 56px rgba(92,61,46,0.11), 0 2px 14px rgba(92,61,46,0.06);
  position: relative;
  animation: fadeUp 0.9s 0.35s ease both;
}
.profile-card::before {
  content: '';
  position: absolute; top: 0; left: 0; right: 0; height: 4px;
  background: linear-gradient(90deg, var(--bronze), var(--mocha));
}
.photo-wrap { display: flex; justify-content: center; margin-bottom: 1.5rem; }
.photo-circle {
  width: 100px; height: 100px; border-radius: 50%;
  background: var(--bg2); border: 3px solid var(--border2);
  overflow: hidden;
}
.photo-circle img { width: 100%; height: 100%; object-fit: cover; }
.card-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.6rem; font-weight: 700;
  text-align: center; color: var(--espresso); margin-bottom: 0.25rem;
}
.card-title {
  font-size: 0.67rem; letter-spacing: 0.22em; text-transform: uppercase;
  color: var(--bronze); text-align: center; font-weight: 700; margin-bottom: 0.25rem;
}
.card-company {
  font-size: 0.8rem; color: var(--taupe); font-weight: 500;
  text-align: center; margin-bottom: 1.4rem;
}
.card-divider { height: 1.5px; background: var(--border); margin: 0 0 1.2rem; }
.card-row { display: flex; align-items: flex-start; gap: 0.8rem; margin-bottom: 0.85rem; }
.card-icon { font-size: 1rem; flex-shrink: 0; margin-top: 1px; }
.card-row-label {
  font-size: 0.6rem; letter-spacing: 0.14em; text-transform: uppercase;
  color: var(--sand); margin-bottom: 1px; font-weight: 600;
}
.card-row-val { font-size: 0.88rem; color: var(--espresso); font-weight: 500; }
.spec-row { display: flex; flex-wrap: wrap; gap: 0.45rem; margin-top: 1.3rem; }
.spec-tag {
  background: var(--bg2); border: 1.5px solid var(--border2);
  color: var(--mocha); padding: 0.27rem 0.8rem;
  font-size: 0.64rem; letter-spacing: 0.12em;
  text-transform: uppercase; font-weight: 600;
}

/* ── SECTION SHARED ── */
.section-outer { position: relative; z-index: 1; }
.section-inner { max-width: 1280px; margin: 0 auto; padding: 3rem 3.5rem; }
.sec-eyebrow {
  display: flex; align-items: center; gap: 0.8rem;
  font-size: 0.65rem; letter-spacing: 0.3em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 0.8rem; font-weight: 700;
}
.sec-eyebrow::before { content: ''; width: 1.8rem; height: 1.5px; background: var(--bronze); }
h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(1.8rem, 3.5vw, 2.8rem);
  font-weight: 700; color: var(--espresso);
  line-height: 1.18; margin-bottom: 0.7rem;
}
h2 em { font-style: italic; color: var(--bronze); }
.sec-subtitle {
  font-size: 0.92rem; color: var(--taupe); font-weight: 400;
  line-height: 1.85; margin-bottom: 1.5rem; max-width: 540px;
}

/* ── FILTER BAR ── */
.filter-bar {
  display: flex; align-items: center; justify-content: space-between;
  flex-wrap: nowrap; gap: 0.9rem; margin-bottom: 1.4rem;
}
.filter-left { display: flex; align-items: center; gap: 0.8rem; flex-shrink: 0; }

/* filter dropdown */
.filter-dropdown-wrap { position: relative; }
.filter-main-btn {
  display: flex; align-items: center; gap: 0.55rem;
  background: var(--card); border: 1.5px solid var(--border2);
  color: var(--mocha); font-family: 'Jost', sans-serif;
  font-size: 0.75rem; letter-spacing: 0.12em; text-transform: uppercase;
  font-weight: 700; padding: 0.58rem 1.1rem; cursor: pointer;
  transition: border-color 0.2s; white-space: nowrap;
}
.filter-main-btn:hover { border-color: var(--bronze); }
.filter-main-btn .arrow {
  display: inline-block; width: 0; height: 0;
  border-left: 4px solid transparent; border-right: 4px solid transparent;
  border-top: 5px solid var(--bronze); margin-left: 0.2rem;
  transition: transform 0.2s;
}
.filter-main-btn.open .arrow { transform: rotate(180deg); }
.filter-panel {
  display: none; position: absolute; top: calc(100% + 4px); left: 0;
  background: var(--card); border: 1.5px solid var(--border2);
  padding: 1rem 1.1rem; z-index: 100; min-width: 340px;
  box-shadow: 0 8px 28px rgba(92,61,46,0.1);
}
.filter-panel.open { display: block; }
.filter-group { margin-bottom: 0.9rem; }
.filter-group:last-child { margin-bottom: 0; }
.filter-group-label {
  font-size: 0.59rem; letter-spacing: 0.16em; text-transform: uppercase;
  color: var(--sand); font-weight: 700; margin-bottom: 0.45rem; display: block;
}
.filter-chips { display: flex; flex-wrap: wrap; gap: 0.35rem; }
.chip {
  padding: 0.38rem 0.85rem; border: 1.5px solid var(--border2);
  background: transparent; color: var(--taupe);
  font-family: 'Jost', sans-serif; font-size: 0.68rem;
  letter-spacing: 0.1em; text-transform: uppercase;
  cursor: pointer; font-weight: 600; transition: all 0.18s;
}
.chip:hover { border-color: var(--bronze); color: var(--bronze); }
.chip.active { background: var(--mocha); color: #fff; border-color: var(--mocha); }

/* ── CURRENCY TOGGLE ── */
.currency-inline {
  display: flex; align-items: center; gap: 0.5rem; flex-shrink: 0;
}
.currency-label {
  font-size: 0.64rem; letter-spacing: 0.16em; text-transform: uppercase;
  color: var(--sand); font-weight: 700; white-space: nowrap;
}
.currency-toggle {
  display: flex; border: 1.5px solid var(--border2); overflow: hidden; flex-shrink: 0;
}
.cur-btn {
  padding: 0.42rem 0.8rem; background: transparent; color: var(--taupe);
  font-family: 'Jost', sans-serif; font-size: 0.68rem;
  letter-spacing: 0.1em; text-transform: uppercase;
  cursor: pointer; font-weight: 700; border: none;
  border-right: 1.5px solid var(--border2);
  transition: all 0.2s; white-space: nowrap;
}
.cur-btn:last-child { border-right: none; }
.cur-btn:hover { background: var(--bg3); color: var(--bronze); }
.cur-btn.active { background: var(--mocha); color: #fff; }

.rate-note {
  font-size: 0.61rem; color: var(--sand); font-weight: 400;
  font-style: italic; display: flex; align-items: center; gap: 0.28rem;
  white-space: nowrap;
}
.rate-dot { width: 6px; height: 6px; border-radius: 50%; background: #4caf50; display: inline-block; flex-shrink: 0; }
.rate-dot.stale { background: var(--bronze); }

/* ── SEARCH BAR ── */
.search-bar-wrap {
  background: var(--card);
  border: 1.5px solid var(--border2);
  padding: 0.7rem 1rem;
  display: flex; gap: 0.7rem;
  align-items: center; margin-bottom: 1rem;
}
.search-input {
  flex: 1 1 0;
  background: var(--bg2); border: 1.5px solid var(--border);
  color: var(--espresso); font-family: 'Jost', sans-serif;
  font-size: 0.82rem; padding: 0.55rem 1rem; font-weight: 500;
  outline: none; transition: border-color 0.2s; min-width: 0;
}
.search-input::placeholder { color: var(--sand); font-weight: 400; }
.search-input:focus { border-color: var(--bronze); }
.search-results-count {
  font-size: 0.72rem; color: var(--sand); font-weight: 600;
  letter-spacing: 0.08em; white-space: nowrap; flex-shrink: 0;
}

/* ── DEVELOPERS ── */
.dev-section { background: var(--bg2); }
.dev-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1.1rem; }
.dev-card {
  background: var(--card); border: 1.5px solid var(--border);
  padding: 1.6rem 1.4rem; position: relative; overflow: hidden;
  transition: box-shadow 0.3s, transform 0.3s, border-color 0.3s;
  text-decoration: none; display: block; color: inherit; cursor: pointer;
}
.dev-card:hover {
  box-shadow: 0 12px 36px rgba(92,61,46,0.13);
  transform: translateY(-4px); border-color: var(--bronze);
}
.dev-card::after {
  content: attr(data-num);
  position: absolute; bottom: -0.5rem; right: 0.8rem;
  font-family: 'Playfair Display', serif;
  font-size: 4.5rem; color: rgba(154,107,63,0.07);
  line-height: 1; pointer-events: none; user-select: none; font-weight: 700;
}
.dev-icon { font-size: 1.4rem; margin-bottom: 0.7rem; }
.dev-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.05rem; font-weight: 700; color: var(--mocha); margin-bottom: 0.2rem;
}
.dev-visit {
  font-size: 0.58rem; letter-spacing: 0.12em; text-transform: uppercase;
  color: var(--bronze); font-weight: 700; margin-bottom: 0.3rem;
  opacity: 0; transition: opacity 0.2s;
  display: flex; align-items: center; gap: 0.3rem;
}
.dev-card:hover .dev-visit { opacity: 1; }
.dev-type {
  font-size: 0.6rem; letter-spacing: 0.16em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 0.7rem; font-weight: 700;
}
.dev-desc { font-size: 0.8rem; color: var(--taupe); line-height: 1.75; font-weight: 400; }
.dev-areas { display: flex; flex-wrap: wrap; gap: 0.35rem; margin-top: 0.9rem; }
.area-pill {
  font-size: 0.58rem; letter-spacing: 0.08em; text-transform: uppercase;
  color: var(--taupe); background: var(--bg2); border: 1px solid var(--border2);
  padding: 0.2rem 0.55rem; font-weight: 600;
}

/* ── BADGES ── */
.badge {
  display: inline-block; padding: 0.2rem 0.65rem;
  font-size: 0.58rem; letter-spacing: 0.1em;
  text-transform: uppercase; font-weight: 700;
}
.badge-sell      { background: rgba(92,61,46,0.1);    color: var(--mocha);  }
.badge-rent      { background: rgba(154,107,63,0.13); color: var(--bronze); }
.badge-offplan   { background: rgba(80,130,80,0.1);   color: #4a7a4a;       }
.badge-vacant    { background: rgba(80,140,200,0.1);  color: #3a6a9a;       }
.badge-rented    { background: rgba(200,140,80,0.12); color: #8a5a20;       }
.badge-distress  { background: rgba(180,60,60,0.1);   color: #9a2a2a;       }

/* ── LISTINGS GRID ── */
.listings-section { background: var(--bg); }
.primary-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; }

.prop-card {
  background: var(--card); border: 1.5px solid var(--border);
  padding: 1.1rem 1.1rem 0.9rem;
  position: relative; overflow: hidden;
  transition: box-shadow 0.25s, transform 0.25s, border-color 0.25s;
  display: flex; flex-direction: column;
}
.prop-card:hover {
  box-shadow: 0 8px 28px rgba(92,61,46,0.12);
  transform: translateY(-3px); border-color: var(--bronze);
}
.prop-card.hot::after {
  content: '🔥 Hot';
  position: absolute; top: 8px; right: 0;
  background: var(--bronze); color: #fff;
  font-size: 0.55rem; letter-spacing: 0.1em; text-transform: uppercase;
  font-weight: 700; padding: 0.18rem 0.6rem;
}
.prop-card.urgent::after {
  content: '⚡ Urgent';
  position: absolute; top: 8px; right: 0;
  background: #9a2a2a; color: #fff;
  font-size: 0.55rem; letter-spacing: 0.1em; text-transform: uppercase;
  font-weight: 700; padding: 0.18rem 0.6rem;
}
.prop-card-head {
  display: flex; justify-content: space-between; align-items: flex-start;
  gap: 0.4rem; margin-bottom: 0.5rem;
}
.prop-card-name {
  font-family: 'Playfair Display', serif;
  font-size: 0.88rem; font-weight: 700; color: var(--espresso);
  line-height: 1.25; flex: 1; padding-right: 0.3rem;
}
.prop-card-area {
  font-size: 0.6rem; letter-spacing: 0.12em; text-transform: uppercase;
  color: var(--bronze); font-weight: 700; margin-bottom: 0.55rem;
}
.prop-inline {
  display: flex; flex-wrap: wrap; gap: 0.3rem 0.7rem;
  margin-bottom: 0.55rem;
}
.prop-inline-item {
  font-size: 0.72rem; color: var(--taupe); font-weight: 500;
  display: flex; align-items: center; gap: 0.22rem;
}
.prop-inline-item span { color: var(--espresso); font-weight: 600; }
.prop-note {
  font-size: 0.7rem; color: var(--taupe); line-height: 1.55;
  margin-bottom: 0.55rem; font-style: italic;
  border-left: 2px solid var(--border2); padding-left: 0.5rem;
}
.prop-price-row {
  display: flex; justify-content: space-between; align-items: flex-end;
  gap: 0.4rem; margin-top: auto; padding-top: 0.55rem;
  border-top: 1px solid var(--border);
}
.prop-price {
  font-family: 'Playfair Display', serif;
  font-size: 1rem; font-weight: 700; color: var(--mocha); line-height: 1.2;
}
.prop-price-conv {
  font-size: 0.65rem; color: var(--sand); font-weight: 500; margin-top: 1px;
}
.prop-enquire {
  display: inline-flex; align-items: center; gap: 0.3rem;
  background: #25D366; color: #fff; padding: 0.42rem 0.85rem;
  text-decoration: none; font-size: 0.65rem; letter-spacing: 0.08em;
  text-transform: uppercase; font-weight: 700;
  transition: background 0.22s, transform 0.18s; white-space: nowrap; flex-shrink: 0;
}
.prop-enquire:hover { background: #1cb85a; transform: translateY(-1px); }
.sec-empty {
  grid-column: 1/-1; text-align: center;
  padding: 2.5rem; color: var(--sand); font-weight: 500; font-size: 0.88rem;
}

.availability-note {
  margin-top: 1.5rem; text-align: center;
  font-size: 0.75rem; font-weight: 500;
  letter-spacing: 0.04em; color: var(--sand);
  padding-top: 1rem; font-style: italic;
  border-top: 1px solid var(--border);
}

.more-properties-banner {
  margin-top: 2rem; background: var(--card);
  border: 1.5px solid var(--border2); border-left: 4px solid var(--bronze);
  padding: 1.3rem 1.8rem;
  display: flex; align-items: center; justify-content: space-between;
  gap: 1.2rem; flex-wrap: wrap;
}
.more-prop-title {
  font-family: 'Playfair Display', serif;
  font-size: 1.05rem; font-weight: 700; color: var(--espresso); margin-bottom: 0.25rem;
}
.more-prop-sub { font-size: 0.8rem; color: var(--taupe); font-weight: 400; line-height: 1.55; }
.more-prop-sub strong { color: var(--mocha); font-weight: 600; }
.btn-more-props {
  display: inline-flex; align-items: center; gap: 0.55rem;
  background: #25D366; color: #fff;
  padding: 0.8rem 1.6rem; text-decoration: none;
  font-size: 0.76rem; letter-spacing: 0.12em; text-transform: uppercase;
  font-weight: 700; white-space: nowrap;
  transition: background 0.3s, transform 0.2s; flex-shrink: 0;
}
.btn-more-props:hover { background: #1cb85a; transform: translateY(-2px); }

/* ── SECONDARY ── */
.secondary-section { background: var(--bg2); }
.sec-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; }

/* ── CONTACT ── */
.contact-strip {
  background: var(--mocha); padding: 3.5rem 3.5rem;
  position: relative; z-index: 1; overflow: hidden;
}
.contact-strip::before {
  content: ''; position: absolute; right: -80px; top: -100px;
  width: 380px; height: 380px; border-radius: 50%;
  background: rgba(255,255,255,0.04); pointer-events: none;
}
.contact-strip::after {
  content: ''; position: absolute; left: -50px; bottom: -70px;
  width: 260px; height: 260px; border-radius: 50%;
  background: rgba(255,255,255,0.025); pointer-events: none;
}
.contact-inner {
  max-width: 900px; margin: 0 auto; text-align: center;
  position: relative; z-index: 2;
}
.contact-inner h2 {
  color: var(--bg); margin-bottom: 0.7rem;
  font-size: clamp(1.8rem, 3.5vw, 2.8rem);
}
.contact-inner h2 em { color: var(--bronze2); font-style: italic; }
.contact-inner p {
  color: rgba(245,240,232,0.72); font-size: 1rem;
  font-weight: 400; margin-bottom: 2rem; line-height: 1.7;
}
.contact-btns {
  display: flex; gap: 1rem; flex-wrap: wrap; justify-content: center;
}
.btn-wa-lg {
  display: inline-flex; align-items: center; gap: 0.65rem;
  background: #25D366; color: #fff;
  padding: 1rem 2.2rem; text-decoration: none;
  font-size: 0.84rem; letter-spacing: 0.14em; text-transform: uppercase;
  font-weight: 600; transition: all 0.3s;
}
.btn-wa-lg:hover { background: #1cb85a; transform: translateY(-2px); }
.btn-call-lg {
  display: inline-flex; align-items: center; gap: 0.65rem;
  background: transparent; color: var(--bg);
  border: 2px solid rgba(245,240,232,0.45);
  padding: 1rem 2.2rem; text-decoration: none;
  font-size: 0.84rem; letter-spacing: 0.14em; text-transform: uppercase;
  font-weight: 600; transition: all 0.3s;
}
.btn-call-lg:hover { border-color: var(--bg); transform: translateY(-2px); }
.contact-details-row {
  display: flex; justify-content: center; gap: 2.5rem; flex-wrap: wrap;
  margin-top: 2rem; padding-top: 2rem;
  border-top: 1px solid rgba(245,240,232,0.15);
}
.contact-detail-item { text-align: center; }
.contact-detail-label {
  font-size: 0.6rem; letter-spacing: 0.2em; text-transform: uppercase;
  color: rgba(245,240,232,0.45); font-weight: 700; margin-bottom: 0.3rem;
}
.contact-detail-val {
  font-size: 0.92rem; color: var(--bg); font-weight: 600;
}

/* ── COMPANY STRIP ── */
.nh-strip-outer {
  background: var(--espresso); position: relative; z-index: 1; overflow: hidden;
}
.nh-strip-outer::before {
  content: ''; position: absolute; right: -80px; top: -80px;
  width: 320px; height: 320px; border-radius: 50%;
  background: rgba(154,107,63,0.07); pointer-events: none;
}
.nh-strip-inner {
  max-width: 1280px; margin: 0 auto;
  padding: 2.8rem 3.5rem;
  display: flex; align-items: center; justify-content: space-between;
  gap: 3rem; flex-wrap: wrap; position: relative; z-index: 2;
}
.nh-strip-eyebrow {
  font-size: 0.63rem; letter-spacing: 0.26em; text-transform: uppercase;
  color: var(--bronze2); font-weight: 700; margin-bottom: 0.45rem;
}
.nh-strip-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.8rem; font-weight: 700; color: var(--bg);
  line-height: 1.1; margin-bottom: 0.22rem;
}
.nh-strip-tagline {
  font-size: 0.68rem; letter-spacing: 0.16em; text-transform: uppercase;
  color: var(--bronze2); font-weight: 600; margin-bottom: 0.9rem;
}
.nh-strip-desc {
  font-size: 0.87rem; color: rgba(245,240,232,0.72);
  line-height: 1.8; max-width: 520px; margin-bottom: 1.3rem;
}
.nh-strip-desc strong { color: var(--bg); font-weight: 600; }
.nh-strip-stats { display: flex; gap: 1.8rem; flex-wrap: wrap; }
.nh-stat {
  display: flex; flex-direction: column; gap: 0.12rem;
  border-left: 2px solid rgba(181,130,78,0.4); padding-left: 0.9rem;
}
.nh-stat-val {
  font-family: 'Playfair Display', serif;
  font-size: 1.35rem; font-weight: 700; color: var(--bronze2); line-height: 1;
}
.nh-stat-lbl {
  font-size: 0.58rem; letter-spacing: 0.12em; text-transform: uppercase;
  color: rgba(245,240,232,0.5); font-weight: 600;
}
.nh-strip-cta {
  display: flex; align-items: center; gap: 1rem;
  background: rgba(154,107,63,0.15);
  border: 1.5px solid rgba(154,107,63,0.4);
  padding: 1.3rem 1.8rem; text-decoration: none;
  transition: background 0.3s, border-color 0.3s, transform 0.2s;
}
.nh-strip-cta:hover {
  background: rgba(154,107,63,0.25);
  border-color: var(--bronze2); transform: translateY(-2px);
}
.nh-cta-icon { font-size: 1.7rem; }
.nh-cta-label {
  font-size: 0.58rem; letter-spacing: 0.16em; text-transform: uppercase;
  color: rgba(245,240,232,0.5); font-weight: 700; margin-bottom: 0.25rem;
}
.nh-cta-link {
  font-family: 'Playfair Display', serif;
  font-size: 1rem; font-weight: 700; color: var(--bronze2);
}

/* ── FOOTER ── */
footer {
  background: var(--espresso); padding: 2.5rem 3.5rem;
  position: relative; z-index: 1; text-align: center;
}
.footer-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.5rem; font-weight: 700; color: var(--bg); margin-bottom: 0.25rem;
}
.footer-role {
  font-size: 0.64rem; letter-spacing: 0.24em; text-transform: uppercase;
  color: var(--sand); margin-bottom: 0.3rem; font-weight: 600;
}
.footer-company {
  font-family: 'Playfair Display', serif;
  font-size: 0.9rem; font-weight: 600;
  color: var(--bronze2); letter-spacing: 0.08em; margin-bottom: 0.4rem;
}
.footer-copy { font-size: 0.64rem; letter-spacing: 0.08em; color: var(--sand); font-weight: 500; margin-top: 1.2rem; }

/* ── MOBILE STICKY ── */
.mobile-sticky {
  display: none;
  position: fixed; bottom: 0; left: 0; right: 0; z-index: 300;
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

@keyframes fadeUp {
  from { opacity: 0; transform: translateY(22px); }
  to   { opacity: 1; transform: translateY(0); }
}

/* ── RESPONSIVE ── */
@media (max-width: 1200px) {
  .primary-grid { grid-template-columns: repeat(3, 1fr); }
  .sec-grid { grid-template-columns: repeat(3, 1fr); }
}
@media (max-width: 1024px) {
  .hero { grid-template-columns: 1fr; gap: 2rem; padding: 5.5rem 2rem 2rem; }
  .dev-grid { grid-template-columns: repeat(2, 1fr); }
  .section-inner { padding: 2.5rem 2rem; }
  .nh-strip-inner { padding: 2.2rem 2rem; }
  nav { padding: 1rem 2rem; }
  .primary-grid { grid-template-columns: repeat(2, 1fr); }
  .sec-grid { grid-template-columns: repeat(2, 1fr); }
  .filter-panel { min-width: 300px; }
}

@media (max-width: 768px) {
  nav { padding: 0.9rem 1.2rem; }
  .nav-brand-name { font-size: 1.1rem; }
  .nav-brand-sub { font-size: 0.52rem; }

  .hero { grid-template-columns: 1fr; padding: 4.8rem 1.2rem 1.5rem; gap: 1.8rem; }
  h1 { font-size: clamp(2rem, 8vw, 3rem); margin-bottom: 1rem; }
  .hero-desc { font-size: 0.88rem; max-width: 100%; margin-bottom: 1rem; }
  .hero-stats { gap: 1rem; flex-wrap: wrap; }
  .stat-val { font-size: 1.5rem; }

  .profile-card { padding: 1.6rem 1.2rem; }
  .card-name { font-size: 1.35rem; }

  .section-inner { padding: 2rem 1.2rem; }
  h2 { font-size: clamp(1.5rem, 6vw, 2.2rem); }
  .sec-subtitle { font-size: 0.85rem; max-width: 100%; }

  .dev-grid { grid-template-columns: 1fr; gap: 0.8rem; }
  .dev-card { padding: 1.2rem 1rem; }

  /* Search bar */
  .search-bar-wrap { padding: 0.6rem 0.8rem; gap: 0.5rem; }
  .search-input { font-size: 0.8rem; padding: 0.5rem 0.8rem; }

  /* Filter bar — stack vertically */
  .filter-bar {
    flex-direction: column;
    align-items: stretch;
    gap: 0.75rem;
  }
  .filter-left {
    display: flex; flex-direction: row;
    align-items: center; gap: 0.6rem; flex-wrap: nowrap;
  }
  /* Currency row on mobile — full width, neat row */
  .currency-inline {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 0.5rem;
    width: 100%;
  }
  .currency-label {
    flex-shrink: 0;
    font-size: 0.62rem;
  }
  .currency-toggle {
    flex: 1;
    display: flex;
  }
  .cur-btn {
    flex: 1;
    text-align: center;
    padding: 0.48rem 0.4rem;
    font-size: 0.66rem;
  }
  .rate-note { display: none; }
  /* filter panel full-width on mobile */
  .filter-panel {
    min-width: 0;
    width: calc(100vw - 2.4rem);
    max-width: 360px;
    left: 0;
  }

  .primary-grid { grid-template-columns: 1fr; gap: 0.9rem; }
  .sec-grid { grid-template-columns: 1fr; gap: 0.9rem; }

  .prop-card { padding: 1rem; }
  .prop-card-name { font-size: 0.85rem; }
  .prop-price { font-size: 0.95rem; }
  .prop-enquire { padding: 0.45rem 0.75rem; font-size: 0.62rem; }

  .more-properties-banner { flex-direction: column; padding: 1rem 1.1rem; }
  .btn-more-props { width: 100%; justify-content: center; }

  .nh-strip-inner { flex-direction: column; padding: 2rem 1.2rem; gap: 1.5rem; }
  .nh-strip-name { font-size: 1.45rem; }
  .nh-strip-stats { gap: 1rem; }
  .nh-strip-cta { padding: 1rem 1.2rem; }

  .contact-strip { padding: 2.5rem 1.2rem; }
  .contact-btns { flex-direction: column; align-items: center; }
  .btn-wa-lg, .btn-call-lg { width: 100%; justify-content: center; padding: 0.9rem 1.5rem; font-size: 0.78rem; }
  .contact-details-row { gap: 1.2rem; }

  footer { padding: 2rem 1.2rem; }
  .mobile-sticky { display: grid; }
  body { padding-bottom: 68px; }
}

@media (max-width: 400px) {
  .hero-stats { flex-direction: column; gap: 0.8rem; }
  .stat { border-left: none; border-top: 1.5px solid var(--border2); padding-left: 0; padding-top: 0.7rem; }
  .filter-left { flex-wrap: wrap; }
}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-brand">
    <div class="nav-brand-name">New Heights Real Estate</div>
    <div class="nav-brand-sub">Dubai · UAE</div>
  </div>
</nav>

<!-- HERO -->
<section style="position:relative;z-index:1;">
  <div class="hero">
    <div class="hero-left">
      <div class="eyebrow"><span class="eyebrow-line"></span>Dubai Real Estate</div>
      <h1>Your Property<br><em>Expert</em> in<br>Dubai</h1>
      <p class="hero-desc">
        Whether you're buying, selling, or renting, I will assist you through Dubai's market with
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
    </div>
    <div class="profile-card">
      <div class="photo-wrap">
        <div class="photo-circle">
          <img src="TB 1.jpg" alt="Taher Betwala"/>
        </div>
      </div>
      <div class="card-name">Taher Betwala</div>
      <div class="card-title">Property Consultant, Dubai</div>
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
          <div class="card-row-val">10+ Years, Dubai Market</div>
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

<!-- COMPANY STRIP -->
<div class="nh-strip-outer">
  <div class="nh-strip-inner">
    <div class="nh-strip-left">
      <div class="nh-strip-eyebrow">📍 Proudly Representing</div>
      <div class="nh-strip-name">New Heights Real Estate</div>
      <div class="nh-strip-tagline">Dubai's Premier Property Advisory Firm</div>
      <p class="nh-strip-desc">
        Backed by one of Dubai's most trusted property advisory firms, I bring you access to exclusive listings, early off-plan launches, and investment-grade secondary market deals. New Heights Real Estate has guided <strong>700+ happy clients</strong> across the emirate with a reputation built on transparency, speed, and results that speak for themselves.
      </p>
      <div class="nh-strip-stats">
        <div class="nh-stat"><span class="nh-stat-val">700+</span><span class="nh-stat-lbl">Happy Clients</span></div>
        <div class="nh-stat"><span class="nh-stat-val">1,500+</span><span class="nh-stat-lbl">Properties Sold</span></div>
        <div class="nh-stat"><span class="nh-stat-val">4.7 / 5</span><span class="nh-stat-lbl">Google Rating</span></div>
        <div class="nh-stat"><span class="nh-stat-val">10+</span><span class="nh-stat-lbl">Years Excellence</span></div>
      </div>
    </div>
    <div>
      <a href="https://newheightsrealestate.ae/" target="_blank" rel="noopener" class="nh-strip-cta">
        <span class="nh-cta-icon">🏢</span>
        <div>
          <div class="nh-cta-label">Official Website</div>
          <div class="nh-cta-link">newheightsrealestate.ae ↗</div>
        </div>
      </a>
    </div>
  </div>
</div>

<!-- DEVELOPERS -->
<div class="section-outer dev-section" id="developers">
  <div class="section-inner">
    <div class="sec-eyebrow" style="justify-content:center;">Our Network</div>
    <h2 style="text-align:center;">Dubai's Top Developers <em>— All Under One Roof</em></h2>
    <p class="sec-subtitle" style="text-align:center;max-width:100%;">From iconic master communities to boutique luxury residences, I work across every major developer in Dubai. Click any card to visit their official website.</p>
    <div class="dev-grid">
      <a class="dev-card" data-num="01" href="https://www.emaar.com" target="_blank" rel="noopener">
        <div class="dev-icon">🏙️</div>
        <div class="dev-name">Emaar Properties</div>
        <div class="dev-visit">↗ Visit emaar.com</div>
        <div class="dev-type">Master-Planned Communities</div>
        <div class="dev-desc">Dubai's most iconic developer — creators of Burj Khalifa and Downtown Dubai. Trusted for world-class amenities and strong capital appreciation.</div>
        <div class="dev-areas">
          <span class="area-pill">Downtown Dubai</span><span class="area-pill">Dubai Marina</span>
          <span class="area-pill">Arabian Ranches</span><span class="area-pill">Creek Harbour</span>
        </div>
      </a>
      <a class="dev-card" data-num="02" href="https://www.damacproperties.com" target="_blank" rel="noopener">
        <div class="dev-icon">💎</div>
        <div class="dev-name">DAMAC Properties</div>
        <div class="dev-visit">↗ Visit damacproperties.com</div>
        <div class="dev-type">Luxury &amp; Branded Residences</div>
        <div class="dev-desc">High-end developer with bold branded collaborations — Cavalli, Versace, Rotana. Popular for premium finishes and strong rental returns.</div>
        <div class="dev-areas">
          <span class="area-pill">Business Bay</span><span class="area-pill">DAMAC Hills</span>
          <span class="area-pill">Safa Park</span><span class="area-pill">Akoya</span>
        </div>
      </a>
      <a class="dev-card" data-num="03" href="https://www.nakheel.com" target="_blank" rel="noopener">
        <div class="dev-icon">🌊</div>
        <div class="dev-name">Nakheel</div>
        <div class="dev-visit">↗ Visit nakheel.com</div>
        <div class="dev-type">Waterfront Living</div>
        <div class="dev-desc">Creator of Palm Jumeirah and The World Islands. Waterfront communities and family clusters ideal for lifestyle buyers and long-term investors.</div>
        <div class="dev-areas">
          <span class="area-pill">Palm Jumeirah</span><span class="area-pill">Jumeirah Village</span>
          <span class="area-pill">Al Furjan</span><span class="area-pill">Deira Islands</span>
        </div>
      </a>
      <a class="dev-card" data-num="04" href="https://www.sobharealty.com" target="_blank" rel="noopener">
        <div class="dev-icon">🏡</div>
        <div class="dev-name">Sobha Realty</div>
        <div class="dev-visit">↗ Visit sobharealty.com</div>
        <div class="dev-type">Self-Built Quality</div>
        <div class="dev-desc">Renowned for in-house construction with zero outsourcing, delivering superior build quality. Sobha Hartland is their flagship green community.</div>
        <div class="dev-areas">
          <span class="area-pill">MBR City</span><span class="area-pill">Sobha Hartland</span>
          <span class="area-pill">Hartland II</span>
        </div>
      </a>
      <a class="dev-card" data-num="05" href="https://www.meraas.com" target="_blank" rel="noopener">
        <div class="dev-icon">🎨</div>
        <div class="dev-name">Meraas</div>
        <div class="dev-visit">↗ Visit meraas.com</div>
        <div class="dev-type">Lifestyle &amp; Culture</div>
        <div class="dev-desc">Lifestyle-driven developer behind City Walk, Bluewaters Island, and Port De La Mer. Blends culture, retail, and contemporary living.</div>
        <div class="dev-areas">
          <span class="area-pill">City Walk</span><span class="area-pill">Bluewaters Island</span>
          <span class="area-pill">Port De La Mer</span><span class="area-pill">La Mer</span>
        </div>
      </a>
      <a class="dev-card" data-num="06" href="https://www.dubaiproperties.ae" target="_blank" rel="noopener">
        <div class="dev-icon">🏛️</div>
        <div class="dev-name">Dubai Properties</div>
        <div class="dev-visit">↗ Visit dubaiproperties.ae</div>
        <div class="dev-type">Government-Backed Value</div>
        <div class="dev-desc">Government-backed developer offering communities from affordable to mid-range. Trusted for consistent long-term value and family-friendly layouts.</div>
        <div class="dev-areas">
          <span class="area-pill">JBR</span><span class="area-pill">Mudon</span>
          <span class="area-pill">Villanova</span><span class="area-pill">Culture Village</span>
        </div>
      </a>
      <a class="dev-card" data-num="07" href="https://www.danubeproperties.com" target="_blank" rel="noopener">
        <div class="dev-icon">✨</div>
        <div class="dev-name">Danube Properties</div>
        <div class="dev-visit">↗ Visit danubeproperties.com</div>
        <div class="dev-type">Affordable Luxury</div>
        <div class="dev-desc">One of Dubai's fastest-growing developers, making luxury accessible with flexible payment plans and strong ROI. Ideal for first-time buyers.</div>
        <div class="dev-areas">
          <span class="area-pill">Arjan</span><span class="area-pill">Jumeirah Village Circle</span>
          <span class="area-pill">Al Furjan</span><span class="area-pill">Sports City</span>
        </div>
      </a>
    </div>
  </div>
</div>

<!-- PRIMARY LISTINGS -->
<div class="section-outer listings-section" id="listings">
  <div class="section-inner">
    <div class="sec-eyebrow" style="justify-content:center;">Primary Market</div>
    <h2 style="text-align:center;">Current <em>Listings</em></h2>
    <p class="sec-subtitle" style="text-align:center;max-width:100%;">Browse available primary market properties across Dubai. Click Enquire to connect directly on WhatsApp with full property details.</p>

    <!-- Search -->
    <div class="search-bar-wrap">
      <input type="text" class="search-input" id="primarySearch" placeholder="🔍  Search by name, location, developer…" oninput="applyPrimaryFilters()"/>
      <span class="search-results-count" id="primaryCount"></span>
    </div>

    <!-- Filter bar: left = filter btn | right = currency -->
    <div class="filter-bar">
      <div class="filter-left">
        <div class="filter-dropdown-wrap">
          <button class="filter-main-btn" id="primaryFilterBtn" onclick="toggleFilterPanel('primaryFilterPanel','primaryFilterBtn')">
            <span id="primaryFilterLabel">Filters</span>
            <span class="arrow"></span>
          </button>
          <div class="filter-panel" id="primaryFilterPanel">
            <!-- Listing Type -->
            <div class="filter-group">
              <span class="filter-group-label">Listing Type</span>
              <div class="filter-chips" id="primaryTypeChips">
                <button class="chip active" onclick="setPrimaryType('all',this)">All</button>
                <button class="chip" onclick="setPrimaryType('sell',this)">For Sale</button>
                <button class="chip" onclick="setPrimaryType('rent',this)">For Rent</button>
                <button class="chip" onclick="setPrimaryType('offplan',this)">Off-Plan</button>
              </div>
            </div>
            <!-- Bedrooms / Size — all in one group -->
            <div class="filter-group">
              <span class="filter-group-label">Bedrooms / Size</span>
              <div class="filter-chips" id="primaryBedsChips">
                <button class="chip active" onclick="setPrimaryBeds('',this)">All</button>
                <button class="chip" onclick="setPrimaryBeds('Studio',this)">Studio</button>
                <button class="chip" onclick="setPrimaryBeds('1 BR',this)">1 BR</button>
                <button class="chip" onclick="setPrimaryBeds('2 BR',this)">2 BR</button>
                <button class="chip" onclick="setPrimaryBeds('3 BR',this)">3 BR</button>
                <button class="chip" onclick="setPrimaryBeds('4 BR',this)">4 BR</button>
                <button class="chip" onclick="setPrimaryBeds('5 BR',this)">5 BR</button>
                <button class="chip" onclick="setPrimaryBeds('6 BR',this)">6+ BR</button>
                <button class="chip" onclick="setPrimaryBeds('Townhouse',this)">Townhouse</button>
                <button class="chip" onclick="setPrimaryBeds('Villa',this)">Villa</button>
                <button class="chip" onclick="setPrimaryBeds('Warehouse',this)">Warehouse</button>
              </div>
            </div>
            <!-- Developer -->
            <div class="filter-group">
              <span class="filter-group-label">Developer</span>
              <div class="filter-chips" id="primaryDevChips">
                <button class="chip active" onclick="setPrimaryDev('',this)">All</button>
                <button class="chip" onclick="setPrimaryDev('Emaar',this)">Emaar</button>
                <button class="chip" onclick="setPrimaryDev('DAMAC',this)">DAMAC</button>
                <button class="chip" onclick="setPrimaryDev('Nakheel',this)">Nakheel</button>
                <button class="chip" onclick="setPrimaryDev('Sobha',this)">Sobha</button>
                <button class="chip" onclick="setPrimaryDev('Meraas',this)">Meraas</button>
                <button class="chip" onclick="setPrimaryDev('Danube',this)">Danube</button>
                <button class="chip" onclick="setPrimaryDev('Binghatti',this)">Binghatti</button>
                <button class="chip" onclick="setPrimaryDev('Azizi',this)">Azizi</button>
              </div>
            </div>
          </div>
        </div>
        <span class="filter-active-label" id="primaryActiveLabel" style="font-size:0.7rem;color:var(--taupe);font-weight:500;"></span>
      </div>
      <!-- Currency -->
      <div class="currency-inline">
        <span class="currency-label">Price in</span>
        <div class="currency-toggle">
          <button class="cur-btn active" onclick="setCurrency('AED',this)">AED</button>
          <button class="cur-btn" onclick="setCurrency('INR',this)">INR</button>
          <button class="cur-btn" onclick="setCurrency('USD',this)">USD</button>
        </div>
        <span class="rate-note" id="rateNote-primary"><span class="rate-dot stale" id="rateDot-primary"></span><span id="rateText-primary">Loading…</span></span>
      </div>
    </div>

    <div class="primary-grid" id="listingsBody"></div>
    <p class="availability-note">All properties are subject to availability at the time of enquiry. INR / USD prices are approximate conversions based on live exchange rates — actual transactions are in AED. Listings updated regularly.</p>
    <div class="more-properties-banner">
      <div>
        <div class="more-prop-title">Looking for something not listed here?</div>
        <div class="more-prop-sub">These are just a selection — I have access to <strong>hundreds more properties</strong> including exclusive off-market deals, new launches, and investor portfolios.</div>
      </div>
      <a href="https://wa.me/971556472153?text=Hi%20Taher!%20I%20checked%20your%20listings%20but%20didn't%20find%20what%20I'm%20looking%20for.%20Can%20you%20help%20me%20find%20more%20options?" target="_blank" class="btn-more-props">💬 Ask for More Options</a>
    </div>
  </div>
</div>

<!-- SECONDARY LISTINGS -->
<div class="section-outer secondary-section" id="secondary">
  <div class="section-inner">
    <div class="sec-eyebrow" style="justify-content:center;">Secondary Market</div>
    <h2 style="text-align:center;">Secondary Market — <em>Direct Listings</em></h2>
    <p class="sec-subtitle" style="text-align:center;max-width:100%;">Exclusive secondary market properties, direct from owners and investors. Prices are negotiable. Click Enquire on any property to connect directly on WhatsApp.</p>

    <!-- Search -->
    <div class="search-bar-wrap">
      <input type="text" class="search-input" id="secSearch" placeholder="🔍  Search by name, area, notes…" oninput="applySecFilters()"/>
      <span class="search-results-count" id="secCount"></span>
    </div>

    <!-- Filter bar -->
    <div class="filter-bar">
      <div class="filter-left">
        <div class="filter-dropdown-wrap">
          <button class="filter-main-btn" id="secFilterBtn" onclick="toggleFilterPanel('secFilterPanel','secFilterBtn')">
            <span id="secFilterLabel">Filters</span>
            <span class="arrow"></span>
          </button>
          <div class="filter-panel" id="secFilterPanel">
            <!-- Listing Type -->
            <div class="filter-group">
              <span class="filter-group-label">Listing Type</span>
              <div class="filter-chips" id="secTypeChips">
                <button class="chip active" onclick="setSecType('all',this)">All</button>
                <button class="chip" onclick="setSecType('rent',this)">For Rent</button>
                <button class="chip" onclick="setSecType('sell',this)">For Sale</button>
                <button class="chip" onclick="setSecType('offplan',this)">Off-Plan Resale</button>
              </div>
            </div>
            <!-- Bedrooms / Size — all in one group -->
            <div class="filter-group">
              <span class="filter-group-label">Bedrooms / Size</span>
              <div class="filter-chips" id="secBedsChips">
                <button class="chip active" onclick="setSecBeds('',this)">All</button>
                <button class="chip" onclick="setSecBeds('Studio',this)">Studio</button>
                <button class="chip" onclick="setSecBeds('1 BR',this)">1 BR</button>
                <button class="chip" onclick="setSecBeds('2 BR',this)">2 BR</button>
                <button class="chip" onclick="setSecBeds('3 BR',this)">3 BR</button>
                <button class="chip" onclick="setSecBeds('4 BR',this)">4 BR</button>
                <button class="chip" onclick="setSecBeds('5 BR',this)">5 BR</button>
                <button class="chip" onclick="setSecBeds('6 BR',this)">6+ BR</button>
                <button class="chip" onclick="setSecBeds('Plot',this)">Plot</button>
                <button class="chip" onclick="setSecBeds('Villa',this)">Villa</button>
                <button class="chip" onclick="setSecBeds('Penthouse',this)">Penthouse</button>
                <button class="chip" onclick="setSecBeds('Full Floor',this)">Full Floor</button>
              </div>
            </div>
            <!-- Occupancy Status -->
            <div class="filter-group">
              <span class="filter-group-label">Occupancy Status</span>
              <div class="filter-chips" id="secOccChips">
                <button class="chip active" onclick="setSecOcc('',this)">Any</button>
                <button class="chip" onclick="setSecOcc('Vacant',this)">Vacant</button>
                <button class="chip" onclick="setSecOcc('Rented',this)">Rented</button>
                <button class="chip" onclick="setSecOcc('Off-Plan',this)">Off-Plan</button>
              </div>
            </div>
          </div>
        </div>
        <span class="filter-active-label" id="secActiveLabel" style="font-size:0.7rem;color:var(--taupe);font-weight:500;"></span>
      </div>
      <!-- Currency -->
      <div class="currency-inline">
        <span class="currency-label">Price in</span>
        <div class="currency-toggle">
          <button class="cur-btn active" onclick="setCurrency('AED',this)">AED</button>
          <button class="cur-btn" onclick="setCurrency('INR',this)">INR</button>
          <button class="cur-btn" onclick="setCurrency('USD',this)">USD</button>
        </div>
        <span class="rate-note" id="rateNote-secondary"><span class="rate-dot stale" id="rateDot-secondary"></span><span id="rateText-secondary">Loading…</span></span>
      </div>
    </div>

    <div class="sec-grid" id="secGrid"></div>
    <p class="availability-note">All properties are subject to availability at the time of enquiry. INR / USD prices are approximate conversions — actual transactions are in AED. Listings updated regularly.</p>
  </div>
</div>

<!-- CONTACT -->
<div class="contact-strip" id="contact">
  <div class="contact-inner">
    <h2>Let's Find Your<br><em>Perfect Property</em></h2>
    <p>Reach out today — response within the hour. Whether you're buying, selling, renting or investing, I'm here to guide you every step of the way.</p>
 <!-- FOOTER -->
<footer>
  <div class="footer-name">Taher Betwala</div>
  <div class="footer-role">Property Consultant, Dubai</div>
  <div class="footer-company">New Heights Real Estate</div>
  <div class="footer-copy">© 2025 Taher Betwala · New Heights Real Estate · All Rights Reserved · Dubai, UAE</div>
</footer>

<!-- MOBILE STICKY BUTTONS -->
<div class="mobile-sticky">
  <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!" target="_blank" class="mob-btn mob-btn-wa">💬 WhatsApp</a>
  <a href="tel:+971556472153" class="mob-btn mob-btn-call">📞 Call</a>
</div>

<script>
/* ── RATES ── */
const FALLBACK_RATES = { AED: 1, INR: 22.45, USD: 0.2722 };
let rates = { ...FALLBACK_RATES };
let activeCurrency = 'AED';
let ratesLive = false;

async function fetchRates() {
  try {
    const res = await fetch('https://api.exchangerate-api.com/v4/latest/AED');
    if (!res.ok) throw new Error();
    const data = await res.json();
    rates.INR = data.rates.INR || FALLBACK_RATES.INR;
    rates.USD = data.rates.USD || FALLBACK_RATES.USD;
    ratesLive = true;
    updateRateNote();
    applyPrimaryFilters();
    applySecFilters();
  } catch(e) {
    ratesLive = false;
    updateRateNote();
  }
}

function updateRateNote() {
  ['primary','secondary'].forEach(id => {
    const dot = document.getElementById('rateDot-' + id);
    const txt = document.getElementById('rateText-' + id);
    if (!dot || !txt) return;
    if (activeCurrency === 'AED') {
      dot.className = 'rate-dot';
      txt.textContent = 'Prices in AED';
      return;
    }
    if (ratesLive) {
      dot.className = 'rate-dot';
      const sym = activeCurrency === 'INR' ? '₹' : '$';
      const r = activeCurrency === 'INR' ? rates.INR.toFixed(2) : rates.USD.toFixed(4);
      txt.textContent = 'Live: 1 AED = ' + sym + r + ' · Approx';
    } else {
      dot.className = 'rate-dot stale';
      txt.textContent = 'Approx (offline) · Verify before transacting';
    }
  });
}

function setCurrency(cur, btn) {
  activeCurrency = cur;
  // update all cur-btn toggles on the page
  document.querySelectorAll('.cur-btn').forEach(b => {
    b.classList.toggle('active', b.textContent.trim() === cur);
  });
  updateRateNote();
  applyPrimaryFilters();
  applySecFilters();
}

/* ── PRICE HELPERS ── */
function parsePriceAED(priceStr) {
  const s = priceStr.toString().trim();
  if (/on request/i.test(s)) return { value: null, isSpecial: true };
  if (/contact/i.test(s))    return { value: null, isSpecial: true };
  if (/same as capital/i.test(s)) return { value: null, isSpecial: true };
  let suffix = '';
  if (/\/\s*mo/i.test(s)) suffix = '/mo';
  else if (/\/\s*yr/i.test(s)) suffix = '/yr';
  const cleaned = s.replace(/AED\s*/i,'').replace(/[,\s]/g,'').replace(/\/.*$/,'').trim();
  const num = parseFloat(cleaned);
  return { value: isNaN(num) ? null : num, suffix, isSpecial: false };
}

function formatConverted(priceStr) {
  if (activeCurrency === 'AED') return '';
  const { value, suffix, isSpecial } = parsePriceAED(priceStr);
  if (isSpecial || value === null) return '';
  const rate = rates[activeCurrency];
  const converted = value * rate;
  const sym = activeCurrency === 'INR' ? '₹' : '$';
  let formatted;
  if (activeCurrency === 'INR') {
    if (converted >= 1e7)      formatted = sym + (converted / 1e7).toFixed(2) + ' Cr';
    else if (converted >= 1e5) formatted = sym + (converted / 1e5).toFixed(2) + ' L';
    else                       formatted = sym + Math.round(converted).toLocaleString('en-IN');
  } else {
    if (converted >= 1e6)      formatted = sym + (converted / 1e6).toFixed(2) + 'M';
    else if (converted >= 1e3) formatted = sym + Math.round(converted / 1000) + 'K';
    else                       formatted = sym + Math.round(converted).toLocaleString();
  }
  return '≈ ' + formatted + (suffix||'') + ' <span style="font-size:0.58rem;opacity:0.7">(approx)</span>';
}

/* ── DATA ── */
const listings = [
  { id:1,  name:"Harbour Gate — Tower 1",          type:"Apartment",  developer:"Emaar",            location:"Creek Harbour",           beds:"1 BR",       size:"780",    price:"1,450,000",   status:"sell" },
  { id:2,  name:"Sobha Hartland — Greens",          type:"Villa",      developer:"Sobha",            location:"MBR City",                beds:"4 BR",       size:"3,800",  price:"6,500,000",   status:"sell" },
  { id:3,  name:"Bluewaters Residences",            type:"Apartment",  developer:"Meraas",           location:"Bluewaters Island",       beds:"2 BR",       size:"1,400",  price:"4,200,000",   status:"sell" },
  { id:4,  name:"Address Harbour Point",            type:"Apartment",  developer:"Emaar",            location:"Creek Harbour",           beds:"2 BR",       size:"1,180",  price:"2,800,000",   status:"sell" },
  { id:5,  name:"Golf Place — Phase II",            type:"Villa",      developer:"Emaar",            location:"Dubai Hills Estate",      beds:"5 BR",       size:"5,200",  price:"9,800,000",   status:"sell" },
  { id:6,  name:"Cavalli Estates",                  type:"Villa",      developer:"DAMAC",            location:"DAMAC Hills",             beds:"6 BR",       size:"8,500",  price:"18,500,000",  status:"sell" },
  { id:7,  name:"Jumeirah Living — Marina",         type:"Apartment",  developer:"Dubai Properties", location:"Dubai Marina",            beds:"3 BR",       size:"2,050",  price:"5,100,000",   status:"sell" },
  { id:8,  name:"Villanova — La Rosa 5",            type:"Townhouse",  developer:"Dubai Properties", location:"Dubailand",               beds:"3 BR",       size:"2,220",  price:"2,150,000",   status:"sell" },
  { id:9,  name:"DAMAC Volta",                      type:"Apartment",  developer:"DAMAC",            location:"Downtown Dubai",          beds:"2 BR",       size:"1,250",  price:"18,000 / mo", status:"rent" },
  { id:10, name:"Palm Beach Towers",                type:"Apartment",  developer:"Nakheel",          location:"Palm Jumeirah",           beds:"3 BR",       size:"2,100",  price:"35,000 / mo", status:"rent" },
  { id:11, name:"Mudon Al Ranim",                   type:"Townhouse",  developer:"Dubai Properties", location:"Mudon",                   beds:"4 BR",       size:"2,700",  price:"22,000 / mo", status:"rent" },
  { id:12, name:"Creek Vistas Reserve",             type:"Apartment",  developer:"Sobha",            location:"MBR City",                beds:"1 BR",       size:"710",    price:"9,500 / mo",  status:"rent" },
  { id:13, name:"City Walk Residences",             type:"Apartment",  developer:"Meraas",           location:"City Walk",               beds:"2 BR",       size:"1,350",  price:"19,000 / mo", status:"rent" },
  { id:14, name:"Emaar Beachfront — Beach Vista",   type:"Apartment",  developer:"Emaar",            location:"Emaar Beachfront",        beds:"1 BR",       size:"820",    price:"13,000 / mo", status:"rent" },
  { id:15, name:"Elo — Phase 2",                   type:"Townhouse",  developer:"DAMAC",            location:"DAMAC Hills 2",           beds:"3 BR",       size:"1,900",  price:"1,750,000",   status:"offplan" },
  { id:16, name:"Danube Opalz",                    type:"Apartment",  developer:"Danube",           location:"Arjan",                   beds:"Studio",     size:"450",    price:"680,000",     status:"offplan" },
  { id:17, name:"Sobha Solis",                     type:"Apartment",  developer:"Sobha",            location:"Motor City",              beds:"1 BR",       size:"660",    price:"1,100,000",   status:"offplan" },
  { id:18, name:"Creek Waters 2",                  type:"Apartment",  developer:"Emaar",            location:"Creek Harbour",           beds:"2 BR",       size:"1,050",  price:"2,350,000",   status:"offplan" },
  { id:19, name:"Danube Petalz — Phase 3",         type:"Apartment",  developer:"Danube",           location:"Jumeirah Village Circle", beds:"1 BR",       size:"580",    price:"790,000",     status:"offplan" },
  { id:20, name:"Safa One — De GRISOGONO",         type:"Apartment",  developer:"DAMAC",            location:"Safa Park",               beds:"2 BR",       size:"1,320",  price:"3,600,000",   status:"offplan" },
  { id:21, name:"Nakheel Bay Residences",          type:"Apartment",  developer:"Nakheel",          location:"Deira Islands",           beds:"2 BR",       size:"1,100",  price:"1,950,000",   status:"offplan" },
  { id:22, name:"J One — Business Bay",            type:"Apartment",  developer:"—",                location:"Business Bay",            beds:"2 BR",       size:"1,600",  price:"3,300,000",   status:"sell",   note:"Was 3.8M · Furnished · 3 Bath · Motivated Seller" },
  { id:23, name:"Collective 2.0 Tower",            type:"Apartment",  developer:"Emaar",            location:"Dubai Hills",             beds:"1 BR",       size:"479",    price:"1,350,000",   status:"sell",   note:"Rented · Furnished · Community View · Investor Deal" },
  { id:24, name:"Binghatti Elite — Bulk 🔥",       type:"Apartment",  developer:"Binghatti",        location:"Dubai Silicon Oasis",     beds:"Studio",     size:"—",      price:"580,000",     status:"offplan",note:"Market Price 800K — Save AED 220K! Bulk (17 units) 580K · Separately 585K · Handover July 30, 2026" },
  { id:25, name:"Florine Beach — Sobha Siniya",    type:"Apartment",  developer:"Sobha",            location:"Siniya Island",           beds:"1 BR",       size:"513",    price:"1,165,000",   status:"offplan",note:"High Floor · Lagoon & Beach View · OP 1.217M · Market 1.465M · 40% Paid · Handover Sept 2028" },
  { id:26, name:"Rukan Townhouse",                 type:"Townhouse",  developer:"—",                location:"Rukan",                   beds:"1 BR",       size:"—",      price:"1,050,000",   status:"sell",   note:"Fully Furnished · Rented 75K/6 cheques · ROI 7.15% · Direct garden access" },
  { id:27, name:"AG Residence",                    type:"Apartment",  developer:"AG",               location:"Jumeirah Village Circle", beds:"2 BR",       size:"1,141",  price:"1,250,000",   status:"sell",   note:"Fully Furnished · Vacant on Transfer · Good Price Alert 🚨" },
  { id:28, name:"La Fontana Di Trevi",             type:"Apartment",  developer:"—",                location:"Arjan",                   beds:"1 BR",       size:"920",    price:"850,000",     status:"sell",   note:"Fully Furnished · 2 Bath · Covered Parking · Upgraded · Spacious Layout" },
  { id:29, name:"Azizi Venice — Bulk 🔥",          type:"Apartment",  developer:"Azizi",            location:"Dubai South",             beds:"Studio",     size:"—",      price:"450,000",     status:"offplan",note:"10 Units Bulk · 70% Paid · OP 604K · Handover Dec 2026 · Super Distressed ⚡" },
  { id:30, name:"Warehouse — Nad Al Hammar",       type:"Warehouse",  developer:"—",                location:"Nad Al Hammar",           beds:"Industrial", size:"20,551", price:"26,000,000",  status:"sell",   note:"Brand New · Vacant · 180 KW Power · Rare Commercial Opportunity" },
];

const secondaryListings = [
  { id:"S14", name:"Hawthorn Cluster — Corner",    area:"DAMAC Hills 2",      type:"sell",    beds:"Villa Plot",    size:"2,643 sqft",  price:"1,390,000",      occupancy:"—",            tag:"",         note:"Corner Plot" },
  { id:"S15", name:"Hawthorn Cluster — Plot",      area:"DAMAC Hills 2",      type:"sell",    beds:"Villa Plot",    size:"1,881 sqft",  price:"900,000",        occupancy:"—",            tag:"",         note:"" },
  { id:"S16", name:"Rabia Tower",                  area:"Majan",              type:"sell",    beds:"2 BR",          size:"1,127 sqft",  price:"1,000,000",      occupancy:"Vacant",       tag:"",         note:"" },
  { id:"S17", name:"Downtown Views 1",             area:"Downtown Dubai",     type:"sell",    beds:"1 BR",          size:"870 sqft",    price:"2,250,000",      occupancy:"Rented",       tag:"hot",      note:"Rented 125K · Furnished · Near Dubai Mall" },
  { id:"S18", name:"Jebel Ali Hills — Plot P8",    area:"Jebel Ali Hills",    type:"sell",    beds:"Plot",          size:"9,688 sqft",  price:"3,250,000",      occupancy:"—",            tag:"",         note:"Park Facing" },
  { id:"S19", name:"Al Furjan — 6 Bed Villa",      area:"Al Furjan",          type:"sell",    beds:"6 BR",          size:"9,400 sqft",  price:"10,000,000",     occupancy:"Vacant",       tag:"hot",      note:"Private Pool · Vacating Dec" },
  { id:"S20", name:"Haven by Aldar 2 — TH",        area:"Haven Falls",        type:"sell",    beds:"4 BR",          size:"3,105 sqft",  price:"4,350,000",      occupancy:"Off-Plan",     tag:"",         note:"40% Paid · OP + DLD Included" },
  { id:"S21", name:"Marina Dec Tower",             area:"Dubai Marina",       type:"sell",    beds:"1 BR",          size:"823 sqft",    price:"1,100,000",      occupancy:"Vacant",       tag:"",         note:"1st Floor" },
  { id:"S22", name:"Jebel Ali Hills — Plot P14",   area:"Jebel Ali Hills",    type:"sell",    beds:"Corner Plot",   size:"13,000 sqft", price:"325 / sqft",     occupancy:"—",            tag:"",         note:"Corner Plot" },
  { id:"S23", name:"Alvorada — Arabian Ranches",   area:"Arabian Ranches",    type:"sell",    beds:"5 BR",          size:"9,300 sqft",  price:"13,800,000",     occupancy:"Vacant",       tag:"hot",      note:"Private Pool · Type C2" },
  { id:"S24", name:"Palm Jumeirah Penthouse",      area:"Palm Jumeirah",      type:"sell",    beds:"Penthouse",     size:"10,000 sqft", price:"29,000,000",     occupancy:"Vacant",       tag:"hot",      note:"Fully Upgraded" },
  { id:"S25", name:"Vida Downtown",                area:"Downtown Dubai",     type:"sell",    beds:"2 BR",          size:"—",           price:"4,700,000",      occupancy:"Vacant",       tag:"",         note:"" },
  { id:"S26", name:"Camelia Prestige TH",          area:"DAMAC Hills 2",      type:"sell",    beds:"3 BR",          size:"1,924 sqft",  price:"1,900,000",      occupancy:"Off-Plan",     tag:"",         note:"Handover Jan 2026" },
  { id:"S27", name:"DAMAC Lagoons — Malta",        area:"DAMAC Lagoons",      type:"sell",    beds:"4 BR",          size:"—",           price:"2,750,000",      occupancy:"Vacant",       tag:"hot",      note:"Lagoon Proximity" },
  { id:"S28", name:"Silicon Heights 3",            area:"Dubai Silicon Oasis",type:"sell",    beds:"1 BR",          size:"700 sqft",    price:"725,000",        occupancy:"Rented",       tag:"",         note:"Rented 52K" },
  { id:"S29", name:"Suburbia",                     area:"Jebel Ali",          type:"sell",    beds:"1 BR",          size:"751 sqft",    price:"630,000",        occupancy:"Vacant",       tag:"",         note:"" },
  { id:"S30", name:"Remraam — Studio",             area:"Dubailand",          type:"sell",    beds:"Studio",        size:"387 sqft",    price:"480,000",        occupancy:"Rented",       tag:"",         note:"Furnished · Rented 42K" },
  { id:"S31", name:"Remraam",                      area:"Dubailand",          type:"sell",    beds:"1 BR",          size:"665 sqft",    price:"670,000",        occupancy:"Vacant",       tag:"",         note:"" },
  { id:"S32", name:"DAMAC Lagoons — Venice Villa", area:"DAMAC Lagoons",      type:"sell",    beds:"6 BR Villa",    size:"5,073 sqft",  price:"6,600,000",      occupancy:"Vacant",       tag:"hot",      note:"Walking distance to lagoon" },
  { id:"S33", name:"Emaar Oasis — Palace Ostra",   area:"Emaar Oasis",        type:"sell",    beds:"5 BR",          size:"11,363 sqft", price:"15,800,000",     occupancy:"Off-Plan",     tag:"hot",      note:"OP Price 14.98M · Selling 15.8M" },
  { id:"S34", name:"Royal Residence 2",            area:"Sports City",        type:"sell",    beds:"2 BR",          size:"1,154 sqft",  price:"1,050,000",      occupancy:"Rented",       tag:"",         note:"1st Floor · Upgraded" },
  { id:"S35", name:"Jebel Ali Hills — P8 Corner",  area:"Jebel Ali Hills",    type:"sell",    beds:"Corner Plot",   size:"9,748 sqft",  price:"340 / sqft",     occupancy:"—",            tag:"",         note:"Small corner — rare" },
  { id:"S36", name:"Lago Vista",                   area:"IMPZ",               type:"sell",    beds:"Studio",        size:"496 sqft",    price:"460,000",        occupancy:"Vacant",       tag:"",         note:"With Parking" },
  { id:"S37", name:"Fox Hill 6",                   area:"Motor City",         type:"sell",    beds:"2 BR",          size:"2,000 sqft",  price:"1,900,000",      occupancy:"Vacant",       tag:"",         note:"2.5 Bath · 2 Parking · Storage" },
  { id:"S38", name:"Camelia 1 — Arabian Ranches 2",area:"Arabian Ranches 2",  type:"sell",    beds:"4 BR",          size:"4,386 sqft",  price:"5,200,000",      occupancy:"Vacant",       tag:"hot",      note:"Corner · Private Pool · Furnished · Below Market" },
  { id:"S39", name:"DAMAC Lagoons Morocco — Corner",area:"DAMAC Lagoons",     type:"sell",    beds:"5 BR + Maid",   size:"—",           price:"4,800,000",      occupancy:"Off-Plan",     tag:"distress", note:"Vastu Unit · Near Lagoon · Handover Q4 2026 · OP + DLD Included" },
  { id:"S40", name:"Saheel — Arabian Ranches",     area:"Arabian Ranches",    type:"sell",    beds:"5 BR + Maid",   size:"—",           price:"14,200,000",     occupancy:"Vacant",       tag:"hot",      note:"Fully Upgraded · Corner Plot · Negotiable" },
  { id:"S41", name:"Palace — Dubai Hills",         area:"Dubai Hills",        type:"sell",    beds:"Full Floor",    size:"—",           price:"On Request",     occupancy:"Vacant",       tag:"",         note:"Can sell individually or as full floor" },
  { id:"O1",  name:"Azizi Venice",                 area:"Dubai South",        type:"offplan", beds:"1 BR",          size:"—",           price:"Same as Capital",occupancy:"Near Handover",tag:"hot",      note:"40% Paid · 60% Remaining · Same price as original" },
  { id:"O2",  name:"Azizi Grand",                  area:"Dubai Sports City",  type:"offplan", beds:"1 BR",          size:"—",           price:"770,000",        occupancy:"Off-Plan",     tag:"distress", note:"Below OP (was 800K) · Handover June 2026 · Big Layout" },
];

/* ── FILTER STATE ── */
let primaryTypeFilter = 'all';
let primaryBedsFilter = '';
let primaryDevFilter  = '';
let secTypeFilter = 'all';
let secBedsFilter = '';
let secOccFilter  = '';

/* ── DROPDOWN ── */
function toggleFilterPanel(panelId, btnId) {
  const panel = document.getElementById(panelId);
  const btn   = document.getElementById(btnId);
  const isOpen = panel.classList.contains('open');
  document.querySelectorAll('.filter-panel').forEach(p => p.classList.remove('open'));
  document.querySelectorAll('.filter-main-btn').forEach(b => b.classList.remove('open'));
  if (!isOpen) { panel.classList.add('open'); btn.classList.add('open'); }
}
document.addEventListener('click', function(e) {
  if (!e.target.closest('.filter-dropdown-wrap')) {
    document.querySelectorAll('.filter-panel').forEach(p => p.classList.remove('open'));
    document.querySelectorAll('.filter-main-btn').forEach(b => b.classList.remove('open'));
  }
});

/* ── ACTIVE LABEL ── */
function updatePrimaryActiveLabel() {
  const parts = [];
  if (primaryTypeFilter !== 'all') parts.push(primaryTypeFilter === 'sell' ? 'For Sale' : primaryTypeFilter === 'rent' ? 'For Rent' : 'Off-Plan');
  if (primaryBedsFilter) parts.push(primaryBedsFilter);
  if (primaryDevFilter)  parts.push(primaryDevFilter);
  const lbl    = document.getElementById('primaryActiveLabel');
  const btnLbl = document.getElementById('primaryFilterLabel');
  if (parts.length) {
    lbl.innerHTML = '<strong>' + parts.join(' · ') + '</strong>';
    btnLbl.textContent = 'Filters (' + parts.length + ')';
  } else {
    lbl.innerHTML = '';
    btnLbl.textContent = 'Filters';
  }
}
function updateSecActiveLabel() {
  const parts = [];
  if (secTypeFilter !== 'all') parts.push(secTypeFilter === 'sell' ? 'For Sale' : secTypeFilter === 'rent' ? 'For Rent' : 'Off-Plan Resale');
  if (secBedsFilter) parts.push(secBedsFilter);
  if (secOccFilter)  parts.push(secOccFilter);
  const lbl    = document.getElementById('secActiveLabel');
  const btnLbl = document.getElementById('secFilterLabel');
  if (parts.length) {
    lbl.innerHTML = '<strong>' + parts.join(' · ') + '</strong>';
    btnLbl.textContent = 'Filters (' + parts.length + ')';
  } else {
    lbl.innerHTML = '';
    btnLbl.textContent = 'Filters';
  }
}

/* ── WA LINKS ── */
function buildWaLink(p) {
  const sl = { sell:'For Sale', rent:'For Rent', offplan:'Off-Plan' }[p.status] || p.status;
  const n  = p.note ? '%0A%F0%9F%93%8C ' + encodeURIComponent(p.note) : '';
  return 'https://wa.me/971556472153?text=Hi%20Taher!%20I%27m%20interested%20in:%0A%F0%9F%8F%A0%20*'+encodeURIComponent(p.name)+'*%0A%F0%9F%93%8D%20'+encodeURIComponent(p.location)+'%0A%F0%9F%9B%8F%20'+p.type+'%20|%20'+p.beds+(p.size&&p.size!=='—'?'%20|%20'+p.size+' sqft':'')+'%0A%F0%9F%92%B0%20AED%20'+p.price+'%20|%20'+sl+n+'%0ACan%20we%20discuss?%20%F0%9F%94%91';
}
function buildSecWaLink(p) {
  const tl = { sell:'For Sale', rent:'For Rent', offplan:'Off-Plan Resale' }[p.type] || p.type;
  return 'https://wa.me/971556472153?text=Hi%20Taher!%20I%27m%20interested%20in:%0A%F0%9F%8F%A0%20*'+encodeURIComponent(p.name)+'*%0A%F0%9F%93%8D%20'+encodeURIComponent(p.area)+'%0A%F0%9F%9B%8F%20'+p.beds+(p.size&&p.size!=='—'?'%20|%20'+p.size:'')+'%0A%F0%9F%92%B0%20AED%20'+p.price+'%20|%20'+tl+'%0A'+(p.note?'%F0%9F%93%8C%20'+encodeURIComponent(p.note)+'%0A':'')+'Can%20we%20discuss?%20%F0%9F%94%91';
}

/* ── RENDER PRIMARY ── */
const statusMap = { sell:{ label:"For Sale", cls:"badge-sell" }, rent:{ label:"For Rent", cls:"badge-rent" }, offplan:{ label:"Off-Plan", cls:"badge-offplan" } };
function renderListings(data) {
  const grid = document.getElementById('listingsBody');
  grid.innerHTML = '';
  if (!data.length) {
    grid.innerHTML = '<div class="sec-empty">No properties match your search. Try different filters or <a href="https://wa.me/971556472153" target="_blank" style="color:var(--bronze);font-weight:700;">ask Taher directly →</a></div>';
    document.getElementById('primaryCount').textContent = '0 found';
    return;
  }
  document.getElementById('primaryCount').textContent = data.length + ' found';
  data.forEach(p => {
    const s = statusMap[p.status] || statusMap.sell;
    const isHot    = p.note && (p.note.includes('Save') || p.note.includes('Bulk') || p.note.includes('Motivated') || p.note.includes('🔥'));
    const isUrgent = p.note && (p.note.includes('Distress') || p.note.includes('⚡'));
    const conv = activeCurrency !== 'AED' ? formatConverted(p.price) : '';
    grid.innerHTML += '<div class="prop-card '+(isUrgent?'urgent':isHot?'hot':'')+'">'
      +'<div class="prop-card-head"><div class="prop-card-name">'+p.name+'</div><span class="badge '+s.cls+'">'+s.label+'</span></div>'
      +'<div class="prop-card-area">📍 '+p.location+'</div>'
      +'<div class="prop-inline">'
        +'<div class="prop-inline-item">🏠 <span>'+p.type+'</span></div>'
        +'<div class="prop-inline-item">🛏 <span>'+p.beds+'</span></div>'
        +(p.size&&p.size!=='—'?'<div class="prop-inline-item">📐 <span>'+p.size+' sqft</span></div>':'')
        +'<div class="prop-inline-item">🏗 <span>'+p.developer+'</span></div>'
      +'</div>'
      +(p.note?'<div class="prop-note">'+p.note+'</div>':'')
      +'<div class="prop-price-row"><div><div class="prop-price">AED '+p.price+'</div>'+(conv?'<div class="prop-price-conv">'+conv+'</div>':'')+'</div>'
      +'<a href="'+buildWaLink(p)+'" target="_blank" class="prop-enquire">💬 Enquire</a></div></div>';
  });
}

function applyPrimaryFilters() {
  const q = (document.getElementById('primarySearch')?.value || '').toLowerCase();
  let data = listings;
  if (primaryTypeFilter !== 'all') data = data.filter(p => p.status === primaryTypeFilter);
  if (primaryBedsFilter) {
    if (primaryBedsFilter === '6 BR')      data = data.filter(p => /6 BR|7 BR|8 BR/.test(p.beds));
    else if (primaryBedsFilter === 'Townhouse') data = data.filter(p => p.type === 'Townhouse');
    else if (primaryBedsFilter === 'Villa')     data = data.filter(p => p.type === 'Villa');
    else if (primaryBedsFilter === 'Warehouse') data = data.filter(p => p.type === 'Warehouse');
    else data = data.filter(p => p.beds.includes(primaryBedsFilter));
  }
  if (primaryDevFilter) data = data.filter(p => p.developer === primaryDevFilter);
  if (q) data = data.filter(p => (p.name+p.location+p.developer+p.type+(p.note||'')).toLowerCase().includes(q));
  renderListings(data);
  updatePrimaryActiveLabel();
}

function setPrimaryType(type, btn) {
  primaryTypeFilter = type;
  btn.closest('.filter-chips').querySelectorAll('.chip').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applyPrimaryFilters();
}
function setPrimaryBeds(beds, btn) {
  primaryBedsFilter = beds;
  btn.closest('.filter-chips').querySelectorAll('.chip').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applyPrimaryFilters();
}
function setPrimaryDev(dev, btn) {
  primaryDevFilter = dev;
  btn.closest('.filter-chips').querySelectorAll('.chip').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applyPrimaryFilters();
}

/* ── RENDER SECONDARY ── */
const secTypeMap = { sell:{ label:"For Sale", cls:"badge-sell" }, rent:{ label:"For Rent", cls:"badge-rent" }, offplan:{ label:"Off-Plan Resale", cls:"badge-offplan" } };
const occupancyMap = { "Vacant":"badge-vacant","Rented":"badge-rented","Off-Plan":"badge-offplan","Near Handover":"badge-offplan","—":"" };

function renderSecondary(data) {
  const grid = document.getElementById('secGrid');
  grid.innerHTML = '';
  if (!data.length) {
    grid.innerHTML = '<div class="sec-empty">No properties match your search. <a href="https://wa.me/971556472153" target="_blank" style="color:var(--bronze);font-weight:700;">Ask Taher directly →</a></div>';
    document.getElementById('secCount').textContent = '0 found';
    return;
  }
  document.getElementById('secCount').textContent = data.length + ' found';
  data.forEach(p => {
    const t = secTypeMap[p.type] || secTypeMap.sell;
    const occCls = occupancyMap[p.occupancy] || '';
    const conv = activeCurrency !== 'AED' ? formatConverted(p.price) : '';
    grid.innerHTML += '<div class="prop-card '+(p.tag==='distress'?'urgent':p.tag==='hot'?'hot':'')+'">'
      +'<div class="prop-card-head"><div class="prop-card-name">'+p.name+'</div><span class="badge '+t.cls+'">'+t.label+'</span></div>'
      +'<div class="prop-card-area">📍 '+p.area+'</div>'
      +'<div class="prop-inline">'
        +'<div class="prop-inline-item">🛏 <span>'+p.beds+'</span></div>'
        +(p.size&&p.size!=='—'?'<div class="prop-inline-item">📐 <span>'+p.size+'</span></div>':'')
        +'<div class="prop-inline-item">🔑 <span>'+p.occupancy+'</span></div>'
      +'</div>'
      +(p.note?'<div class="prop-note">'+p.note+'</div>':'')
      +'<div class="prop-price-row"><div><div class="prop-price">AED '+p.price+'</div>'
      +(conv?'<div class="prop-price-conv">'+conv+'</div>':'')
      +(occCls?'<span class="badge '+occCls+'" style="margin-top:3px;display:inline-block;">'+p.occupancy+'</span>':'')
      +'</div><a href="'+buildSecWaLink(p)+'" target="_blank" class="prop-enquire">💬 Enquire</a></div></div>';
  });
}

function applySecFilters() {
  const q = (document.getElementById('secSearch')?.value || '').toLowerCase();
  let data = secondaryListings;
  if (secTypeFilter !== 'all') data = data.filter(p => p.type === secTypeFilter);
  if (secBedsFilter) {
    if (secBedsFilter === '6 BR')       data = data.filter(p => /6 BR|7 BR|8 BR|6 Bed/.test(p.beds));
    else if (secBedsFilter === 'Villa') data = data.filter(p => /Villa/.test(p.beds));
    else if (secBedsFilter === 'Plot')  data = data.filter(p => /Plot/.test(p.beds));
    else if (secBedsFilter === 'Penthouse')  data = data.filter(p => /Penthouse/.test(p.beds));
    else if (secBedsFilter === 'Full Floor') data = data.filter(p => /Full Floor/.test(p.beds));
    else data = data.filter(p => p.beds.includes(secBedsFilter));
  }
  if (secOccFilter) data = data.filter(p => p.occupancy === secOccFilter);
  if (q) data = data.filter(p => (p.name+p.area+(p.note||'')+p.beds+p.occupancy).toLowerCase().includes(q));
  renderSecondary(data);
  updateSecActiveLabel();
}

function setSecType(type, btn) {
  secTypeFilter = type;
  btn.closest('.filter-chips').querySelectorAll('.chip').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applySecFilters();
}
function setSecBeds(beds, btn) {
  secBedsFilter = beds;
  btn.closest('.filter-chips').querySelectorAll('.chip').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applySecFilters();
}
function setSecOcc(occ, btn) {
  secOccFilter = occ;
  btn.closest('.filter-chips').querySelectorAll('.chip').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applySecFilters();
}

/* ── INIT ── */
applyPrimaryFilters();
applySecFilters();
fetchRates();
</script>
</body>
</html>
