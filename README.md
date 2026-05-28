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

/* ══════════════ REFRESH BANNER ══════════════ */
#refresh-banner {
  display: none;
  position: fixed; top: 0; left: 0; right: 0; z-index: 999;
  background: var(--bronze);
  color: #fff;
  text-align: center;
  padding: 0.7rem 1rem;
  font-size: 0.82rem;
  font-weight: 600;
  letter-spacing: 0.05em;
  animation: slideDown 0.4s ease;
  cursor: pointer;
}
#refresh-banner span { text-decoration: underline; margin-left: 0.5rem; cursor: pointer; font-weight: 700; }
#refresh-countdown { font-weight: 800; margin: 0 0.3rem; }
@keyframes slideDown {
  from { transform: translateY(-100%); }
  to   { transform: translateY(0); }
}

/* ══════════════ NAV ══════════════ */
nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 200;
  display: flex; justify-content: center; align-items: center;
  padding: 1.2rem 3.5rem;
  background: rgba(245,240,232,0.95);
  backdrop-filter: blur(16px);
  border-bottom: 1.5px solid var(--border);
}
.nav-brand { display: flex; flex-direction: column; align-items: center; }
.nav-brand-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.55rem; font-weight: 700;
  color: var(--mocha); letter-spacing: 0.07em; line-height: 1;
}
.nav-brand-sub {
  font-size: 0.6rem; letter-spacing: 0.3em; text-transform: uppercase;
  color: var(--bronze); margin-top: 5px; font-weight: 700;
}

/* ══════════════ HERO ══════════════ */
.hero {
  min-height: auto;
  display: grid; grid-template-columns: 1fr 1fr;
  padding: 4.5rem 3.5rem 2rem;
  gap: 4rem; max-width: 1280px; margin: 0 auto;
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
  color: var(--bronze); margin-bottom: 1rem; font-weight: 600;
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
  line-height: 1.85; max-width: 420px; margin-bottom: 1.5rem;
  animation: fadeUp 0.7s 0.3s ease both;
}
.hero-desc strong { color: var(--espresso); font-weight: 600; }

.hero-stats {
  display: flex; gap: 2.8rem; margin-bottom: 2rem;
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
  background: var(--bg2); border: 3px solid var(--border2);
  display: flex; flex-direction: column;
  align-items: center; justify-content: center;
  overflow: hidden;
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
.section-inner { max-width: 1280px; margin: 0 auto; padding: 3.5rem 3.5rem; }

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
  line-height: 1.85; margin-bottom: 2rem; max-width: 540px;
}

/* ══════════════ DEVELOPERS ══════════════ */
.dev-section { background: var(--bg2); }
.dev-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }

/* Featured company card */
.dev-card-featured {
  grid-column: 1 / -1;
  background: linear-gradient(135deg, var(--mocha) 0%, var(--mocha2) 100%);
  border: 1.5px solid var(--mocha);
  padding: 2.2rem 2.5rem;
  position: relative; overflow: hidden;
  text-decoration: none; display: flex; align-items: center; justify-content: space-between;
  gap: 2rem; flex-wrap: wrap;
  transition: box-shadow 0.3s, transform 0.3s;
}
.dev-card-featured:hover {
  box-shadow: 0 14px 44px rgba(92,61,46,0.28);
  transform: translateY(-3px);
}
.dev-card-featured::before {
  content: '';
  position: absolute; right: -60px; top: -60px;
  width: 220px; height: 220px; border-radius: 50%;
  background: rgba(255,255,255,0.04); pointer-events: none;
}
.dev-featured-left { display: flex; align-items: center; gap: 1.5rem; }
.dev-featured-icon { font-size: 2.2rem; }
.dev-featured-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.55rem; font-weight: 700; color: var(--bg);
  margin-bottom: 0.2rem;
}
.dev-featured-label {
  font-size: 0.63rem; letter-spacing: 0.25em; text-transform: uppercase;
  color: var(--bronze2); font-weight: 700; margin-bottom: 0.4rem;
}
.dev-featured-desc {
  font-size: 0.87rem; color: rgba(245,240,232,0.75); line-height: 1.7; max-width: 520px;
}
.dev-featured-cta {
  display: inline-flex; align-items: center; gap: 0.5rem;
  background: var(--bronze); color: #fff;
  padding: 0.75rem 1.6rem; font-size: 0.74rem;
  letter-spacing: 0.15em; text-transform: uppercase; font-weight: 700;
  transition: background 0.25s, transform 0.2s; white-space: nowrap; flex-shrink: 0;
}
.dev-featured-cta:hover { background: var(--bronze2); transform: translateY(-2px); }

.dev-card {
  background: var(--card); border: 1.5px solid var(--border);
  padding: 2.2rem 2rem; position: relative; overflow: hidden;
  transition: box-shadow 0.3s, transform 0.3s, border-color 0.3s;
  text-decoration: none; display: block; color: inherit; cursor: pointer;
}
.dev-card:hover {
  box-shadow: 0 14px 44px rgba(92,61,46,0.13);
  transform: translateY(-5px); border-color: var(--bronze);
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
  font-size: 1.25rem; font-weight: 700; color: var(--mocha); margin-bottom: 0.3rem;
}
.dev-visit {
  font-size: 0.6rem; letter-spacing: 0.14em; text-transform: uppercase;
  color: var(--bronze); font-weight: 700; margin-bottom: 0.35rem;
  opacity: 0; transition: opacity 0.2s;
  display: flex; align-items: center; gap: 0.3rem;
}
.dev-card:hover .dev-visit { opacity: 1; }
.dev-type {
  font-size: 0.64rem; letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--bronze); margin-bottom: 1rem; font-weight: 700;
}
.dev-desc { font-size: 0.86rem; color: var(--taupe); line-height: 1.82; font-weight: 400; }
.dev-areas { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-top: 1.3rem; }
.area-pill {
  font-size: 0.62rem; letter-spacing: 0.1em; text-transform: uppercase;
  color: var(--taupe); background: var(--bg2); border: 1px solid var(--border2);
  padding: 0.24rem 0.7rem; font-weight: 600;
}

/* ══════════════ SHARED TABLE STYLES ══════════════ */
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

.badge {
  display: inline-block; padding: 0.25rem 0.8rem;
  font-size: 0.62rem; letter-spacing: 0.12em;
  text-transform: uppercase; font-weight: 700;
}
.badge-sell      { background: rgba(92,61,46,0.1);    color: var(--mocha);  }
.badge-rent      { background: rgba(154,107,63,0.13); color: var(--bronze); }
.badge-offplan   { background: rgba(80,130,80,0.1);   color: #4a7a4a;       }
.badge-vacant    { background: rgba(80,140,200,0.1);  color: #3a6a9a;       }
.badge-rented    { background: rgba(200,140,80,0.12); color: #8a5a20;       }
.badge-distress  { background: rgba(180,60,60,0.1);   color: #9a2a2a;       }
.badge-negotiable{ background: rgba(100,160,100,0.1); color: #3a7a3a;       }

/* ══════════════ PRIMARY LISTINGS ══════════════ */
.listings-section { background: var(--bg); }

/* ══════════════ AVAILABILITY NOTE ══════════════ */
.availability-note {
  margin-top: 2rem;
  text-align: center;
  font-size: 0.78rem;
  font-family: 'Jost', sans-serif;
  font-weight: 500;
  letter-spacing: 0.06em;
  color: var(--sand);
  border-top: 1px solid var(--border);
  padding-top: 1.2rem;
  font-style: italic;
}

/* ══════════════ PRIMARY CARD GRID ══════════════ */
.primary-grid {
  display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.4rem;
}
@media (max-width: 1024px) { .primary-grid { grid-template-columns: 1fr 1fr; } }
@media (max-width: 768px)  { .primary-grid { grid-template-columns: 1fr; } }

.more-properties-banner {
  margin-top: 2.5rem; background: var(--card);
  border: 1.5px solid var(--border2); border-left: 4px solid var(--bronze);
  padding: 1.6rem 2rem;
  display: flex; align-items: center; justify-content: space-between;
  gap: 1.5rem; flex-wrap: wrap;
}
.more-prop-title {
  font-family: 'Playfair Display', serif;
  font-size: 1.15rem; font-weight: 700; color: var(--espresso); margin-bottom: 0.3rem;
}
.more-prop-sub { font-size: 0.82rem; color: var(--taupe); font-weight: 400; line-height: 1.6; }
.more-prop-sub strong { color: var(--mocha); font-weight: 600; }
.btn-more-props {
  display: inline-flex; align-items: center; gap: 0.6rem;
  background: #25D366; color: #fff;
  padding: 0.85rem 1.8rem; text-decoration: none;
  font-size: 0.78rem; letter-spacing: 0.13em; text-transform: uppercase;
  font-weight: 700; white-space: nowrap;
  transition: background 0.3s, transform 0.2s; flex-shrink: 0;
}
.btn-more-props:hover { background: #1cb85a; transform: translateY(-2px); }

/* ══════════════ SECONDARY MARKET ══════════════ */
.secondary-section { background: var(--bg2); }

.sec-tabs {
  display: flex; gap: 0; margin-bottom: 2.5rem;
  border: 2px solid var(--border2); width: fit-content; overflow: hidden;
}
.sec-tab {
  padding: 0.65rem 1.8rem; background: transparent; color: var(--taupe);
  font-family: 'Jost', sans-serif; font-size: 0.74rem;
  letter-spacing: 0.15em; text-transform: uppercase;
  cursor: pointer; font-weight: 600; transition: all 0.25s;
  border: none; border-right: 1.5px solid var(--border2);
}
.sec-tab:last-child { border-right: none; }
.sec-tab:hover { background: var(--bg3); color: var(--bronze); }
.sec-tab.active { background: var(--mocha); color: #fff; }

.sec-grid {
  display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.4rem;
}

.sec-card {
  background: var(--card); border: 1.5px solid var(--border);
  padding: 1.6rem; position: relative; overflow: hidden;
  transition: box-shadow 0.3s, transform 0.3s, border-color 0.3s;
  display: flex; flex-direction: column; gap: 0;
}
.sec-card:hover {
  box-shadow: 0 12px 40px rgba(92,61,46,0.12);
  transform: translateY(-4px); border-color: var(--bronze);
}

.sec-card.hot::before {
  content: '🔥 Hot Deal';
  position: absolute; top: 12px; right: -1px;
  background: var(--bronze); color: #fff;
  font-size: 0.6rem; letter-spacing: 0.12em; text-transform: uppercase;
  font-weight: 700; padding: 0.22rem 0.8rem;
}
.sec-card.distress::before {
  content: '⚡ Urgent';
  position: absolute; top: 12px; right: -1px;
  background: #9a2a2a; color: #fff;
  font-size: 0.6rem; letter-spacing: 0.12em; text-transform: uppercase;
  font-weight: 700; padding: 0.22rem 0.8rem;
}

.sec-card-top {
  display: flex; justify-content: space-between; align-items: flex-start;
  margin-bottom: 0.9rem; gap: 0.5rem;
}
.sec-card-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.05rem; font-weight: 700; color: var(--espresso);
  line-height: 1.25; flex: 1;
}
.sec-card-badge { flex-shrink: 0; margin-top: 2px; }

.sec-card-area {
  font-size: 0.68rem; letter-spacing: 0.14em; text-transform: uppercase;
  color: var(--bronze); font-weight: 700; margin-bottom: 0.9rem;
}

.sec-card-details {
  display: grid; grid-template-columns: 1fr 1fr; gap: 0.5rem 1rem;
  margin-bottom: 1.1rem;
}
.sec-det-label {
  font-size: 0.58rem; letter-spacing: 0.13em; text-transform: uppercase;
  color: var(--sand); font-weight: 700; margin-bottom: 1px;
}
.sec-det-val {
  font-size: 0.84rem; color: var(--espresso); font-weight: 600;
}

.sec-card-price {
  font-family: 'Playfair Display', serif;
  font-size: 1.25rem; font-weight: 700; color: var(--mocha);
  margin-bottom: 0.4rem;
}
.sec-card-divider { height: 1px; background: var(--border); margin: 0 0 1rem; }

.sec-card-footer {
  display: flex; align-items: center; justify-content: space-between;
  gap: 0.5rem; flex-wrap: wrap; margin-top: auto;
}
.sec-status-row { display: flex; gap: 0.4rem; flex-wrap: wrap; }

.sec-enquire-btn {
  display: inline-flex; align-items: center; gap: 0.4rem;
  background: #25D366; color: #fff; padding: 0.52rem 1.1rem;
  text-decoration: none; font-size: 0.7rem; letter-spacing: 0.1em;
  text-transform: uppercase; font-weight: 700;
  transition: background 0.25s, transform 0.2s; white-space: nowrap;
}
.sec-enquire-btn:hover { background: #1cb85a; transform: translateY(-1px); }

.sec-empty {
  grid-column: 1/-1; text-align: center;
  padding: 3rem; color: var(--sand); font-weight: 500; font-size: 0.9rem;
}

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
.contact-left p { color: rgba(245,240,232,0.7); font-size: 0.95rem; font-weight: 400; }
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
  background: var(--espresso); padding: 3rem 3.5rem;
  position: relative; z-index: 1; text-align: center;
}
.footer-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.7rem; font-weight: 700; color: var(--bg); margin-bottom: 0.3rem;
}
.footer-role {
  font-size: 0.67rem; letter-spacing: 0.25em; text-transform: uppercase;
  color: var(--sand); margin-bottom: 0.35rem; font-weight: 600;
}
.footer-company {
  font-family: 'Playfair Display', serif;
  font-size: 0.95rem; font-weight: 600;
  color: var(--bronze2); letter-spacing: 0.08em; margin-bottom: 1.4rem;
}
.social-row {
  display: none;
  gap: 1.2rem; justify-content: center; margin-bottom: 1.2rem;
}
.social-link {
  font-size: 0.74rem; letter-spacing: 0.13em; text-transform: uppercase;
  color: var(--sand); text-decoration: none; font-weight: 600; transition: color 0.2s;
}
.social-link:hover { color: var(--bronze2); }
.footer-divider { height: 1px; background: rgba(255,255,255,0.07); margin: 1.2rem 0; }
.footer-copy { font-size: 0.67rem; letter-spacing: 0.1em; color: var(--sand); font-weight: 500; }

/* ══════════════ MOBILE STICKY ══════════════ */
.mobile-sticky {
  display: none; position: fixed; bottom: 0; left: 0; right: 0; z-index: 300;
  grid-template-columns: 1fr 1fr; border-top: 1.5px solid var(--border);
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

/* ══════════════ NEW HEIGHTS STRIP ══════════════ */
.nh-strip-outer {
  background: var(--espresso);
  position: relative; z-index: 1; overflow: hidden;
}
.nh-strip-outer::before {
  content: '';
  position: absolute; right: -80px; top: -80px;
  width: 320px; height: 320px; border-radius: 50%;
  background: rgba(154,107,63,0.07); pointer-events: none;
}
.nh-strip-inner {
  max-width: 1280px; margin: 0 auto;
  padding: 3rem 3.5rem;
  display: flex; align-items: center; justify-content: space-between;
  gap: 3rem; flex-wrap: wrap; position: relative; z-index: 2;
}
.nh-strip-eyebrow {
  font-size: 0.65rem; letter-spacing: 0.28em; text-transform: uppercase;
  color: var(--bronze2); font-weight: 700; margin-bottom: 0.5rem;
}
.nh-strip-name {
  font-family: 'Playfair Display', serif;
  font-size: 2rem; font-weight: 700; color: var(--bg);
  line-height: 1.1; margin-bottom: 0.25rem;
}
.nh-strip-tagline {
  font-size: 0.72rem; letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--bronze2); font-weight: 600; margin-bottom: 1rem;
}
.nh-strip-desc {
  font-size: 0.9rem; color: rgba(245,240,232,0.72);
  line-height: 1.8; max-width: 540px; margin-bottom: 1.5rem;
}
.nh-strip-desc strong { color: var(--bg); font-weight: 600; }
.nh-strip-stats {
  display: flex; gap: 2rem; flex-wrap: wrap;
}
.nh-stat {
  display: flex; flex-direction: column; gap: 0.15rem;
  border-left: 2px solid rgba(181,130,78,0.4); padding-left: 1rem;
}
.nh-stat-val {
  font-family: 'Playfair Display', serif;
  font-size: 1.5rem; font-weight: 700; color: var(--bronze2); line-height: 1;
}
.nh-stat-lbl {
  font-size: 0.6rem; letter-spacing: 0.14em; text-transform: uppercase;
  color: rgba(245,240,232,0.5); font-weight: 600;
}
.nh-strip-right { flex-shrink: 0; }
.nh-strip-cta {
  display: flex; align-items: center; gap: 1rem;
  background: rgba(154,107,63,0.15);
  border: 1.5px solid rgba(154,107,63,0.4);
  padding: 1.4rem 2rem; text-decoration: none;
  transition: background 0.3s, border-color 0.3s, transform 0.2s;
}
.nh-strip-cta:hover {
  background: rgba(154,107,63,0.25);
  border-color: var(--bronze2); transform: translateY(-2px);
}
.nh-cta-icon { font-size: 1.8rem; }
.nh-cta-label {
  font-size: 0.6rem; letter-spacing: 0.18em; text-transform: uppercase;
  color: rgba(245,240,232,0.5); font-weight: 700; margin-bottom: 0.3rem;
}
.nh-cta-link {
  font-family: 'Playfair Display', serif;
  font-size: 1.05rem; font-weight: 700; color: var(--bronze2);
}


@media (max-width: 1024px) {
  .hero { grid-template-columns: 1fr; gap: 2rem; padding: 5.5rem 2rem 2rem; }
  .hero::after { display: none; }
  .dev-grid { grid-template-columns: 1fr 1fr; }
  .sec-grid { grid-template-columns: 1fr 1fr; }
  .section-inner { padding: 3rem 2rem; }
  .nh-strip-inner { padding: 2.5rem 2rem; }
  nav { padding: 1rem 2rem; }
}
@media (max-width: 768px) {
  nav { padding: 1rem 1.5rem; }
  .hero { padding: 5.5rem 1.5rem 2rem; }
  .hero-stats { gap: 1.5rem; flex-wrap: wrap; }
  .stat-val { font-size: 1.7rem; }
  .dev-grid { grid-template-columns: 1fr; }
  .sec-grid { grid-template-columns: 1fr; }
  .nh-strip-inner { flex-direction: column; padding: 2rem 1.5rem; }
  .nh-strip-stats { gap: 1.2rem; }
  .nh-strip-right { width: 100%; }
  .nh-strip-cta { justify-content: center; }
  .contact-inner { flex-direction: column; text-align: center; }
  .contact-btns { justify-content: center; }
  .hide-mobile { display: none !important; }
  footer { padding: 2.5rem 1.5rem; }
  .mobile-sticky { display: grid; }
  body { padding-bottom: 62px; }
  .section-inner { padding: 2.5rem 1.5rem; }
  .contact-strip { padding: 3rem 1.5rem; }
  .sec-tabs { flex-wrap: wrap; width: 100%; }
  .sec-tab { flex: 1; border-right: none; border-bottom: 1.5px solid var(--border2); }
  .more-properties-banner { flex-direction: column; }
  .btn-more-props { width: 100%; justify-content: center; }
}
</style>
</head>
<body>

<!-- ══ REFRESH BANNER ══ -->
<div id="refresh-banner" onclick="window.location.reload(true)">
  🔄 New listings have been added! Auto-refreshing in <span id="refresh-countdown">5</span>s — or <span>click here to refresh now →</span>
</div>

<!-- ══ NAV ══ -->
<nav>
  <div class="nav-brand">
    <div class="nav-brand-name">New Heights Real Estate</div>
    <div class="nav-brand-sub">Dubai · UAE</div>
  </div>
</nav>

<!-- ══ HERO ══ -->
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

    <!-- PROFILE CARD -->
    <div class="profile-card">
      <div class="photo-wrap">
        <div class="photo-circle">
          <img src="TB 1.jpg" alt="Taher Betwala" style="width:100%;height:100%;object-fit:cover;border-radius:50%;"/>
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

<!-- ══ NEW HEIGHTS COMPANY STRIP ══ -->
<div class="nh-strip-outer">
  <div class="nh-strip-inner">
    <div class="nh-strip-left">
      <div class="nh-strip-eyebrow">📍 Proudly Representing</div>
      <div class="nh-strip-name">New Heights Real Estate</div>
      <div class="nh-strip-tagline">Dubai's Premier Property Advisory Firm</div>
      <p class="nh-strip-desc">
        Backed by one of Dubai's most trusted property advisory firms, I bring you access to exclusive listings, early off-plan launches, and investment-grade secondary market deals. New Heights Real Estate has guided <strong>700+ happy clients</strong> across the emirate, from first-time buyers to seasoned investors, with a reputation built on transparency, speed, and results that speak for themselves.
      </p>
      <div class="nh-strip-stats">
        <div class="nh-stat"><span class="nh-stat-val">700+</span><span class="nh-stat-lbl">Happy Clients</span></div>
        <div class="nh-stat"><span class="nh-stat-val">1,500+</span><span class="nh-stat-lbl">Properties Sold</span></div>
        <div class="nh-stat"><span class="nh-stat-val">4.7 / 5</span><span class="nh-stat-lbl">Google Review Rating</span></div>
        <div class="nh-stat"><span class="nh-stat-val">10+</span><span class="nh-stat-lbl">Years of Excellence</span></div>
      </div>
    </div>
    <div class="nh-strip-right">
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

<!-- ══ DEVELOPERS ══ -->
<div class="section-outer dev-section" id="developers">
  <div class="section-inner">
    <div class="sec-eyebrow" style="justify-content:center;">Our Network</div>
    <h2 style="text-align:center;">Dubai's Top Developers  <br><em>All Under One Roof</em></h2>
    <p class="sec-subtitle" style="text-align:center;max-width:100%;">From iconic master communities to boutique luxury residences, I work across every major developer in Dubai so you always find the right fit. Click any card to visit their official website.</p>
    <div class="dev-grid">      <a class="dev-card" data-num="01" href="https://www.emaar.com" target="_blank" rel="noopener">
        <div class="dev-icon">🏙️</div>
        <div class="dev-name">Emaar Properties</div>
        <div class="dev-visit">↗ Visit emaar.com</div>
        <div class="dev-type">Master-Planned Communities</div>
        <div class="dev-desc">Dubai's most iconic developer, creators of Burj Khalifa, Dubai Mall, and Downtown Dubai. Trusted for world-class amenities and strong capital appreciation.</div>
        <div class="dev-areas">
          <span class="area-pill">Downtown Dubai</span><span class="area-pill">Dubai Marina</span>
          <span class="area-pill">Arabian Ranches</span><span class="area-pill">Creek Harbour</span>
        </div>
      </a>
      <a class="dev-card" data-num="02" href="https://www.damacproperties.com" target="_blank" rel="noopener">
        <div class="dev-icon">💎</div>
        <div class="dev-name">DAMAC Properties</div>
        <div class="dev-visit">↗ Visit damacproperties.com</div>
        <div class="dev-type">Luxury & Branded Residences</div>
        <div class="dev-desc">High-end developer with bold branded collaborations, Cavalli, Versace, Rotana. Popular with investors for premium finishes and strong rental returns.</div>
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
        <div class="dev-desc">Creator of Palm Jumeirah and The World Islands. Nakheel builds waterfront communities and family clusters, ideal for lifestyle buyers and long-term investors.</div>
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
        <div class="dev-desc">Renowned for in-house construction with zero outsourcing, delivering superior build quality and finish. Sobha Hartland in MBR City is their flagship green community.</div>
        <div class="dev-areas">
          <span class="area-pill">MBR City</span><span class="area-pill">Sobha Hartland</span>
          <span class="area-pill">Hartland II</span>
        </div>
      </a>
      <a class="dev-card" data-num="05" href="https://www.meraas.com" target="_blank" rel="noopener">
        <div class="dev-icon">🎨</div>
        <div class="dev-name">Meraas</div>
        <div class="dev-visit">↗ Visit meraas.com</div>
        <div class="dev-type">Lifestyle & Culture</div>
        <div class="dev-desc">Lifestyle-driven developer behind City Walk, Bluewaters Island, and Port De La Mer. Meraas blends culture, retail, and contemporary living in prime walkable areas.</div>
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
        <div class="dev-desc">A government-backed developer offering communities from affordable to mid-range. Trusted for consistent long-term value, solid infrastructure, and family-friendly layouts.</div>
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
        <div class="dev-desc">One of Dubai's fastest-growing developers, making luxury accessible with flexible payment plans, high-quality finishes, and strong ROI. Ideal for first-time buyers and savvy investors.</div>
        <div class="dev-areas">
          <span class="area-pill">Arjan</span><span class="area-pill">Jumeirah Village Circle</span>
          <span class="area-pill">Al Furjan</span><span class="area-pill">Sports City</span>
        </div>
      </a>
    </div>
  </div>
</div>

<!-- ══ PRIMARY LISTINGS ══ -->
<div class="section-outer listings-section" id="listings">
  <div class="section-inner">
    <div class="sec-eyebrow" style="justify-content:center;">Primary Market</div>
    <h2 style="text-align:center;">Current <em>Listings</em></h2>
    <p class="sec-subtitle" style="text-align:center;max-width:100%;">Browse available primary market properties across Dubai, updated regularly. Click Enquire on any listing to connect with me directly on WhatsApp with full property details.</p>
    <div class="filters">
      <button class="filter-btn active" onclick="filterListings('all',this)">All Properties</button>
      <button class="filter-btn" onclick="filterListings('sell',this)">For Sale</button>
      <button class="filter-btn" onclick="filterListings('rent',this)">For Rent</button>
      <button class="filter-btn" onclick="filterListings('offplan',this)">Off-Plan</button>
    </div>
    <div class="primary-grid" id="listingsBody"></div>
    <p class="availability-note">⚠ All listed properties are subject to availability at the time of enquiry. Listings are updated regularly, please connect directly for current status.</p>
    <div class="more-properties-banner">
      <div class="more-prop-text">
        <div class="more-prop-title">🔍 Looking for something not listed here?</div>
        <div class="more-prop-sub">These are just a selection, I have access to <strong>hundreds more properties</strong> across Dubai including exclusive off-market deals, new launches, and investor portfolios. Just tell me what you're looking for.</div>
      </div>
      <a href="https://wa.me/971556472153?text=Hi%20Taher!%20I%20checked%20your%20listings%20but%20didn't%20find%20exactly%20what%20I'm%20looking%20for.%20Can%20you%20help%20me%20find%20more%20options?%20%F0%9F%94%91" target="_blank" class="btn-more-props">💬 Ask for More Options</a>
    </div>
  </div>
</div>

<!-- ══ SECONDARY MARKET ══ -->
<div class="section-outer secondary-section" id="secondary">
  <div class="section-inner">
    <div class="sec-eyebrow" style="justify-content:center;">Secondary Market</div>
    <h2 style="text-align:center;">Secondary Market —<br><em>Direct Listings</em></h2>
    <p class="sec-subtitle" style="text-align:center;max-width:100%;">Exclusive secondary market properties, direct from owners and investors. Prices are negotiable. Click any property to enquire directly on WhatsApp with full details.</p>
    <div class="sec-tabs">
      <button class="sec-tab active" onclick="filterSecondary('all', this)">All Listings</button>
      <button class="sec-tab" onclick="filterSecondary('rent', this)">For Rent</button>
      <button class="sec-tab" onclick="filterSecondary('sell', this)">For Sale</button>
      <button class="sec-tab" onclick="filterSecondary('offplan', this)">Off-Plan Resale</button>
    </div>
    <div class="sec-grid" id="secGrid"></div>
    <p class="availability-note">⚠ All listed properties are subject to availability at the time of enquiry. Listings are updated regularly, please connect directly for current status.</p>
  </div>
</div>

<!-- ══ CONTACT STRIP ══ -->
<div class="contact-strip" id="contact">
  <div class="contact-inner">
    <div class="contact-left">
      <h2>Let's Find Your<br><em>Perfect Property</em></h2>
      <p>Reach out today - response within the hour.</p>
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
  <div class="footer-role">Property Consultant, Dubai</div>
  <div class="footer-company">New Heights Real Estate</div>
  <div class="social-row">
    <a href="https://www.instagram.com/habibi_chalodubai/" target="_blank" class="social-link">📸 Instagram</a>
    <a href="https://www.facebook.com/profile.php?id=61580013579727" target="_blank" class="social-link">👍 Facebook</a>
  </div>
  <div class="footer-divider"></div>
  <div class="footer-copy">© 2025 Taher Betwala · New Heights Real Estate · All Rights Reserved</div>
</footer>

<!-- ══ MOBILE STICKY ══ -->
<div class="mobile-sticky">
  <a href="https://wa.me/971556472153?text=Hey%20Taher!%20Found%20your%20profile%20%E2%80%94%20I%20think%20you're%20the%20right%20guy%20to%20find%20my%20dream%20home%20in%20Dubai!%20%F0%9F%94%91" target="_blank" class="mob-btn mob-btn-wa">💬 WhatsApp</a>
  <a href="tel:+971556472153" class="mob-btn mob-btn-call">📞 Call</a>
</div>

<script>
// ═══════════════════════════════════════════════════════════════════
//  VERSION STAMP — update this string whenever you add new listings.
//  The page compares this against what's stored in localStorage and
//  shows a "New listings available — refresh" banner if they differ.
// ═══════════════════════════════════════════════════════════════════
const LISTINGS_VERSION = "2026-05-28-v6";

(function checkVersion() {
  const stored = localStorage.getItem('listingsVersion');
  if (stored && stored !== LISTINGS_VERSION) {
    const banner = document.getElementById('refresh-banner');
    const countdown = document.getElementById('refresh-countdown');
    banner.style.display = 'block';
    document.querySelector('nav').style.top = '44px';
    let secs = 5;
    const tick = setInterval(() => {
      secs--;
      if (countdown) countdown.textContent = secs;
      if (secs <= 0) { clearInterval(tick); window.location.reload(true); }
    }, 1000);
  }
  localStorage.setItem('listingsVersion', LISTINGS_VERSION);
})();

// ═══════════════════════════════════════════════════════════════════
//   PRIMARY LISTINGS
// ═══════════════════════════════════════════════════════════════════
const listings = [
  // ── EXISTING ─────────────────────────────────────────────────────
  { id:1,  name:"Harbour Gate — Tower 1",          type:"Apartment",  developer:"Emaar",           location:"Creek Harbour",       beds:"1 BR",    size:"780",   price:"1,450,000",    status:"sell"    },
  { id:2,  name:"Sobha Hartland — Greens",          type:"Villa",      developer:"Sobha",           location:"MBR City",            beds:"4 BR",    size:"3,800", price:"6,500,000",    status:"sell"    },
  { id:3,  name:"Bluewaters Residences",            type:"Apartment",  developer:"Meraas",          location:"Bluewaters Island",   beds:"2 BR",    size:"1,400", price:"4,200,000",    status:"sell"    },
  { id:4,  name:"Address Harbour Point",            type:"Apartment",  developer:"Emaar",           location:"Creek Harbour",       beds:"2 BR",    size:"1,180", price:"2,800,000",    status:"sell"    },
  { id:5,  name:"Golf Place — Phase II",            type:"Villa",      developer:"Emaar",           location:"Dubai Hills Estate",  beds:"5 BR",    size:"5,200", price:"9,800,000",    status:"sell"    },
  { id:6,  name:"Cavalli Estates",                  type:"Villa",      developer:"DAMAC",           location:"DAMAC Hills",         beds:"6 BR",    size:"8,500", price:"18,500,000",   status:"sell"    },
  { id:7,  name:"Jumeirah Living — Marina Gate",    type:"Apartment",  developer:"Dubai Properties",location:"Dubai Marina",        beds:"3 BR",    size:"2,050", price:"5,100,000",    status:"sell"    },
  { id:8,  name:"Villanova — La Rosa 5",            type:"Townhouse",  developer:"Dubai Properties",location:"Dubailand",           beds:"3 BR",    size:"2,220", price:"2,150,000",    status:"sell"    },
  { id:9,  name:"DAMAC Volta",                      type:"Apartment",  developer:"DAMAC",           location:"Downtown Dubai",      beds:"2 BR",    size:"1,250", price:"18,000 / mo",  status:"rent"    },
  { id:10, name:"Palm Beach Towers",                type:"Apartment",  developer:"Nakheel",         location:"Palm Jumeirah",       beds:"3 BR",    size:"2,100", price:"35,000 / mo",  status:"rent"    },
  { id:11, name:"Mudon Al Ranim — Townhouse",       type:"Townhouse",  developer:"Dubai Properties",location:"Mudon",               beds:"4 BR",    size:"2,700", price:"22,000 / mo",  status:"rent"    },
  { id:12, name:"Creek Vistas Reserve",             type:"Apartment",  developer:"Sobha",           location:"MBR City",            beds:"1 BR",    size:"710",   price:"9,500 / mo",   status:"rent"    },
  { id:13, name:"City Walk Residences",             type:"Apartment",  developer:"Meraas",          location:"City Walk",           beds:"2 BR",    size:"1,350", price:"19,000 / mo",  status:"rent"    },
  { id:14, name:"Emaar Beachfront — Beach Vista",   type:"Apartment",  developer:"Emaar",           location:"Emaar Beachfront",    beds:"1 BR",    size:"820",   price:"13,000 / mo",  status:"rent"    },
  { id:15, name:"Elo — Phase 2",                    type:"Townhouse",  developer:"DAMAC",           location:"DAMAC Hills 2",       beds:"3 BR",    size:"1,900", price:"1,750,000",    status:"offplan" },
  { id:16, name:"Danube Opalz",                     type:"Apartment",  developer:"Danube",          location:"Arjan",               beds:"Studio",  size:"450",   price:"680,000",      status:"offplan" },
  { id:17, name:"Sobha Solis",                      type:"Apartment",  developer:"Sobha",           location:"Motor City",          beds:"1 BR",    size:"660",   price:"1,100,000",    status:"offplan" },
  { id:18, name:"Creek Waters 2",                   type:"Apartment",  developer:"Emaar",           location:"Creek Harbour",       beds:"2 BR",    size:"1,050", price:"2,350,000",    status:"offplan" },
  { id:19, name:"Danube Petalz — Phase 3",          type:"Apartment",  developer:"Danube",          location:"Jumeirah Village Circle", beds:"1 BR",size:"580",   price:"790,000",      status:"offplan" },
  { id:20, name:"Safa One — De GRISOGONO",          type:"Apartment",  developer:"DAMAC",           location:"Safa Park",           beds:"2 BR",    size:"1,320", price:"3,600,000",    status:"offplan" },
  { id:21, name:"Nakheel Bay Residences",           type:"Apartment",  developer:"Nakheel",         location:"Deira Islands",       beds:"2 BR",    size:"1,100", price:"1,950,000",    status:"offplan" },

  // ── NEW ADDITIONS ─────────────────────────────────────────────────
  { id:22, name:"J One — Business Bay",             type:"Apartment",  developer:"—",               location:"Business Bay",        beds:"2 BR",    size:"1,600", price:"3,300,000",    status:"sell",   note:"Was 3.8M · Furnished · 3 Bath · Motivated Seller" },
  { id:23, name:"Collective 2.0 Tower",             type:"Apartment",  developer:"Emaar",           location:"Dubai Hills",         beds:"1 BR",    size:"479",   price:"1,350,000",    status:"sell",   note:"Rented · Furnished · Community View · Investor Deal" },
  { id:24, name:"Binghatti Elite — Bulk Deal 🔥",  type:"Apartment",  developer:"Binghatti",       location:"Dubai Silicon Oasis", beds:"Studio",  size:"—",     price:"580,000",      status:"offplan",note:"Market Price 800K — Save AED 220K! Bulk (17 units) 580K · Separate 585K · Handover July 30, 2026" },
  { id:25, name:"Florine Beach Residences — Sobha Siniya Island", type:"Apartment", developer:"Sobha", location:"Siniya Island", beds:"1 BR", size:"513",  price:"1,165,000",    status:"offplan",note:"High Floor · Lagoon, Beach & Pool View · OP 1.217M · Market 1.465M · 40% Paid · Handover Sept 2028" },
  { id:26, name:"Rukan Townhouse",                  type:"Townhouse",  developer:"—",               location:"Rukan",               beds:"1 BR",    size:"—",     price:"1,050,000",    status:"sell",   note:"Fully Furnished · Rented 75K/6 cheques · Gross ROI 7.15% · Net ROI 6.85% · Direct community garden access" },
  { id:27, name:"AG Residence",                     type:"Apartment",  developer:"AG",              location:"Jumeirah Village Circle", beds:"2 BR", size:"1,141", price:"1,250,000",   status:"sell",   note:"Fully Furnished · Vacant on Transfer · Good Price Alert 🚨" },
  { id:28, name:"La Fontana Di Trevi",              type:"Apartment",  developer:"—",               location:"Arjan",               beds:"1 BR",    size:"920",   price:"850,000",      status:"sell",   note:"Fully Furnished · 2 Bath · 1 Covered Parking · Partially Upgraded · Spacious Layout" },
  { id:29, name:"Azizi Venice — Bulk Deal 🔥",     type:"Apartment",  developer:"Azizi",           location:"Dubai South",         beds:"Studio",  size:"—",     price:"450,000",      status:"offplan",note:"10 Units Bulk Purchase · 70% Paid · OP 604K · Handover Dec 2026 · Super Distressed Price ⚡" },
  { id:30, name:"Warehouse — Nad Al Hammar",        type:"Warehouse",  developer:"—",               location:"Nad Al Hammar",       beds:"Industrial",size:"20,551",price:"26,000,000", status:"sell",   note:"Brand New · Vacant · 180 KW Power · Rare Commercial Opportunity" },
];

// ═══════════════════════════════════════════════════════════════════
//   SECONDARY MARKET LISTINGS
// ═══════════════════════════════════════════════════════════════════
const secondaryListings = [

  // ── FOR RENT ────────────────────────────────────────────────────
  { id:"R1",  name:"Princess Tower",            area:"Dubai Marina",    type:"rent",    beds:"2 BR",   size:"1,200 sqft",  price:"AED 110,000/yr",  occupancy:"Vacant",  tag:"hot",  note:"Furnished"                          },
  { id:"R2",  name:"Downtown Views Tower 2",    area:"Downtown Dubai",  type:"rent",    beds:"2 BR",   size:"—",           price:"AED 200,000/yr",  occupancy:"Vacant",  tag:"hot",  note:"Luxury, Furnished, Fountain View"   },
  { id:"R3",  name:"Elegenz by Danube",         area:"JVC",             type:"rent",    beds:"1 BR + Study", size:"980 sqft", price:"AED 80,000/yr", occupancy:"Vacant", tag:"",    note:"Furnished"                          },
  { id:"R4",  name:"Marina Wharf",              area:"Dubai Marina",    type:"rent",    beds:"3 BR",   size:"1,300 sqft",  price:"AED 165,000/yr",  occupancy:"Vacant",  tag:"hot",  note:"Marina View"                        },
  { id:"R5",  name:"Marina Belvedere",          area:"Dubai Marina",    type:"rent",    beds:"2 BR + Maid", size:"1,500 sqft", price:"AED 110,000/yr", occupancy:"Vacant", tag:"", note:""                                   },
  { id:"R6",  name:"Princess Tower",            area:"Dubai Marina",    type:"rent",    beds:"1 BR",   size:"—",           price:"AED 80,000/yr",   occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"R7",  name:"Marina View Tower",         area:"Dubai Marina",    type:"rent",    beds:"Studio", size:"418 sqft",    price:"AED 68,000/yr",   occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"R8",  name:"Marina View Tower",         area:"Dubai Marina",    type:"rent",    beds:"2 BR",   size:"960 sqft",    price:"AED 110,000/yr",  occupancy:"Vacant",  tag:"",     note:"Furnished"                          },

  // ── FOR SALE ────────────────────────────────────────────────────
  { id:"S1",  name:"Springs — Type 4M",         area:"The Springs",     type:"sell",    beds:"2 BR + Study", size:"1,690 sqft", price:"AED 3,350,000", occupancy:"Vacant", tag:"hot", note:"Pool & Park View. Vacant on transfer" },
  { id:"S2",  name:"Crescent Tower",            area:"IMPZ",            type:"sell",    beds:"Studio", size:"500 sqft",    price:"AED 430,000",     occupancy:"Vacant",  tag:"",     note:"No Parking"                         },
  { id:"S3",  name:"Crescent Tower",            area:"IMPZ",            type:"sell",    beds:"Studio", size:"500 sqft",    price:"AED 475,000",     occupancy:"Rented",  tag:"",     note:"Rented 35K · With Parking"          },
  { id:"S4",  name:"Safeer Tower",              area:"Business Bay",    type:"sell",    beds:"Studio", size:"500 sqft",    price:"AED 720,000",     occupancy:"Vacant",  tag:"hot",  note:""                                   },
  { id:"S5",  name:"Ontario Tower",             area:"Business Bay",    type:"sell",    beds:"1 BR",   size:"810 sqft",    price:"AED 1,000,000",   occupancy:"Rented",  tag:"",     note:"Rented 90K — Investor Deal"         },
  { id:"S6",  name:"Paramount Tower A",         area:"Business Bay",    type:"sell",    beds:"2 BR",   size:"1,485 sqft",  price:"AED 2,250,000",   occupancy:"Vacant",  tag:"hot",  note:"Residential Tower"                  },
  { id:"S7",  name:"Lincoln Park Westside",     area:"Arjan",           type:"sell",    beds:"Studio", size:"—",           price:"AED 530,000",     occupancy:"Rented",  tag:"",     note:"Furnished · Rented 54K"             },
  { id:"S8",  name:"Escan Tower (x2 Units)",    area:"Dubai Marina",    type:"sell",    beds:"Studio", size:"—",           price:"AED 660,000 each", occupancy:"Vacant", tag:"hot",  note:"2 Units Available"                  },
  { id:"S9",  name:"Escan Tower",               area:"Dubai Marina",    type:"sell",    beds:"1 BR",   size:"760 sqft",    price:"AED 1,050,000",   occupancy:"Rented",  tag:"",     note:"Mid Floor"                          },
  { id:"S10", name:"May Residence",             area:"JVC",             type:"sell",    beds:"Studio", size:"400 sqft",    price:"AED 460,000",     occupancy:"Rented",  tag:"",     note:"Rented 40K"                         },
  { id:"S11", name:"May Residence",             area:"JVC",             type:"sell",    beds:"1 BR",   size:"1,217 sqft",  price:"AED 835,000",     occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"S12", name:"Suburbia",                  area:"Jebel Ali",       type:"sell",    beds:"1 BR",   size:"751 sqft",    price:"AED 650,000",     occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"S13", name:"Jebel Ali Hills — Plot",    area:"Jebel Ali Hills", type:"sell",    beds:"2 Plots",size:"—",           price:"AED 375/sqft",    occupancy:"—",       tag:"hot",  note:"Adjacent plots · Contact for sizes" },
  { id:"S14", name:"Hawthorn Cluster — Corner Villa Plot", area:"DAMAC Hills 2", type:"sell", beds:"Villa Plot", size:"2,643 sqft", price:"AED 1,390,000", occupancy:"—", tag:"",  note:""                                   },
  { id:"S15", name:"Hawthorn Cluster — Villa Plot",        area:"DAMAC Hills 2", type:"sell", beds:"Villa Plot", size:"1,881 sqft", price:"AED 900,000",   occupancy:"—", tag:"",  note:""                                   },
  { id:"S16", name:"Rabia Tower",               area:"Majan",           type:"sell",    beds:"2 BR",   size:"1,127 sqft",  price:"AED 1,000,000",   occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"S17", name:"Downtown Views 1",          area:"Downtown Dubai",  type:"sell",    beds:"1 BR",   size:"870 sqft",    price:"AED 2,250,000",   occupancy:"Rented",  tag:"hot",  note:"Rented 125K · Furnished · Near Dubai Mall" },
  { id:"S18", name:"Jebel Ali Hills — Plot P8", area:"Jebel Ali Hills", type:"sell",    beds:"Plot",   size:"9,688 sqft",  price:"AED 3,250,000",   occupancy:"—",       tag:"",     note:"Park Facing"                        },
  { id:"S19", name:"Al Furjan — 6 Bed Villa",  area:"Al Furjan",       type:"sell",    beds:"6 BR",   size:"9,400 sqft plot / 6,900 BUA", price:"AED 10,000,000", occupancy:"Vacant", tag:"hot", note:"Private Pool · Vacating Dec" },
  { id:"S20", name:"Haven by Aldar 2 — Townhouse", area:"Haven Falls",  type:"sell",    beds:"4 BR",   size:"3,105 sqft BUA / 2,762 sqft plot", price:"AED 4,350,000", occupancy:"Off-Plan", tag:"", note:"40% Paid · OP + DLD Included" },
  { id:"S21", name:"Marina Dec Tower",          area:"Dubai Marina",    type:"sell",    beds:"1 BR",   size:"823 sqft",    price:"AED 1,100,000",   occupancy:"Vacant",  tag:"",     note:"1st Floor"                          },
  { id:"S22", name:"Jebel Ali Hills — Plot P14",area:"Jebel Ali Hills", type:"sell",    beds:"Corner Plot", size:"13,000 sqft", price:"AED 325/sqft", occupancy:"—",    tag:"",     note:"Corner Plot"                        },
  { id:"S23", name:"Alvorada — Arabian Ranches 1", area:"Arabian Ranches", type:"sell", beds:"5 BR",  size:"9,300 sqft plot / 4,424 BUA", price:"AED 13,800,000", occupancy:"Vacant", tag:"hot", note:"Private Pool · Type C2"   },
  { id:"S24", name:"Palm Jumeirah Penthouse",   area:"Palm Jumeirah",   type:"sell",    beds:"Penthouse", size:"10,000 sqft", price:"AED 29,000,000", occupancy:"Vacant", tag:"hot", note:"Fully Upgraded"                    },
  { id:"S25", name:"Vida Downtown",             area:"Downtown Dubai",  type:"sell",    beds:"2 BR",   size:"—",           price:"AED 4,700,000",   occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"S26", name:"Camelia Prestige Townhouse",area:"DAMAC Hills 2",   type:"sell",    beds:"3 BR",   size:"1,924 sqft BUA / 1,208 plot", price:"AED 1,900,000", occupancy:"Off-Plan", tag:"", note:"Handover Jan 2026"         },
  { id:"S27", name:"DAMAC Lagoons — Malta",     area:"DAMAC Lagoons",   type:"sell",    beds:"4 BR",   size:"—",           price:"AED 2,750,000",   occupancy:"Vacant",  tag:"hot",  note:"Lagoon Proximity · Prime Location" },
  { id:"S28", name:"Silicon Heights 3",         area:"Dubai Silicon Oasis", type:"sell", beds:"1 BR", size:"700 sqft",    price:"AED 725,000",     occupancy:"Rented",  tag:"",     note:"Rented 52K"                         },
  { id:"S29", name:"Suburbia",                  area:"Jebel Ali",       type:"sell",    beds:"1 BR",   size:"751 sqft",    price:"AED 630,000",     occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"S30", name:"Remraam — Studio",          area:"Dubailand",       type:"sell",    beds:"Studio", size:"387 sqft",    price:"AED 480,000",     occupancy:"Rented",  tag:"",     note:"Furnished · Rented 42K"             },
  { id:"S31", name:"Remraam",                   area:"Dubailand",       type:"sell",    beds:"1 BR",   size:"665 sqft",    price:"AED 670,000",     occupancy:"Vacant",  tag:"",     note:""                                   },
  { id:"S32", name:"DAMAC Lagoons — Venice",    area:"DAMAC Lagoons",   type:"sell",    beds:"6 BR Villa", size:"5,073 sqft plot / 4,572 BUA", price:"AED 6,600,000", occupancy:"Vacant", tag:"hot", note:"Walking distance lagoon" },
  { id:"S33", name:"Emaar Oasis — Palace Ostra",area:"Emaar Oasis",     type:"sell",    beds:"5 BR",   size:"11,363 sqft plot / 8,000 BUA", price:"AED 15,800,000", occupancy:"Off-Plan", tag:"hot", note:"OP Price 14.98M · Selling 15.8M" },
  { id:"S34", name:"Royal Residence 2",         area:"Sports City",     type:"sell",    beds:"2 BR",   size:"1,154 sqft",  price:"AED 1,050,000",   occupancy:"Rented",  tag:"",     note:"1st Floor · Upgraded"               },
  { id:"S35", name:"Jebel Ali Hills — Plot P8 (Corner)", area:"Jebel Ali Hills", type:"sell", beds:"Corner Plot", size:"9,748 sqft", price:"AED 340/sqft", occupancy:"—", tag:"",  note:"Small corner — rare"                },
  { id:"S36", name:"Lago Vista",                area:"IMPZ",            type:"sell",    beds:"Studio", size:"496 sqft",    price:"AED 460,000",     occupancy:"Vacant",  tag:"",     note:"With Parking · Vacating Notice Served" },
  { id:"S37", name:"Fox Hill 6",                area:"Motor City",      type:"sell",    beds:"2 BR",   size:"2,000 sqft",  price:"AED 1,900,000",   occupancy:"Vacant",  tag:"",     note:"2.5 Bath · 2 Parking · Basement Storage · Road Facing" },
  { id:"S38", name:"Camelia 1 — Arabian Ranches 2", area:"Arabian Ranches 2", type:"sell", beds:"4 BR", size:"4,386 sqft", price:"AED 5,200,000",  occupancy:"Vacant",  tag:"hot",  note:"Corner Unit · Private Pool · Furnished · Below Market" },
  { id:"S39", name:"DAMAC Lagoons Morocco — Corner Villa", area:"DAMAC Lagoons", type:"sell", beds:"5 BR + Maid", size:"—", price:"AED 4,800,000", occupancy:"Off-Plan", tag:"distress", note:"Vastu Unit · Near Lagoon · Handover Q4 2026 · OP+DLD included" },
  { id:"S40", name:"Saheel — Arabian Ranches",  area:"Arabian Ranches", type:"sell",    beds:"5 BR + Maid", size:"—",   price:"AED 14,200,000",  occupancy:"Vacant",  tag:"hot",  note:"Fully Upgraded · Corner Plot · Negotiable" },
  { id:"S41", name:"Palace — Dubai Hills (Full Floor)", area:"Dubai Hills", type:"sell", beds:"Full Floor", size:"—",   price:"On Request",      occupancy:"Vacant",  tag:"",     note:"Can sell individually or as full floor" },

  // ── OFF-PLAN RESALE ─────────────────────────────────────────────
  { id:"O1",  name:"Azizi Venice",              area:"Dubai South",     type:"offplan", beds:"1 BR",   size:"—",           price:"Same as Capital",  occupancy:"Near Handover", tag:"hot", note:"40% Paid · 60% Remaining · No profit — same price" },
  { id:"O2",  name:"Azizi Grand",               area:"Dubai Sports City", type:"offplan", beds:"1 BR", size:"—",          price:"AED 770,000",     occupancy:"Off-Plan",  tag:"distress", note:"Below OP (was 800K) · Handover June 2026 · Big Layout" },
];

// ── PRIMARY LISTINGS RENDER ──
const statusMap = {
  sell:    { label:"For Sale",  cls:"badge-sell"    },
  rent:    { label:"For Rent",  cls:"badge-rent"    },
  offplan: { label:"Off-Plan",  cls:"badge-offplan" },
};

function buildWaLink(p) {
  const statusLabel = statusMap[p.status]?.label || p.status;
  const noteText = p.note ? `%0A%F0%9F%93%8C ${encodeURIComponent(p.note)}` : '';
  const msg =
    `Hi Taher! I'm interested in the following property:%0A` +
    `%F0%9F%8F%A0 *${encodeURIComponent(p.name)}*%0A` +
    `%F0%9F%93%8D Location: ${encodeURIComponent(p.location)}%0A` +
    `%F0%9F%9B%8F Type: ${p.type} | ${p.beds}${p.size && p.size !== '—' ? ' | ' + p.size + ' sqft' : ''}%0A` +
    `%F0%9F%92%B0 Price: AED ${p.price} | ${statusLabel}` +
    noteText +
    `%0ACan we discuss further? %F0%9F%94%91`;
  return `https://wa.me/971556472153?text=${msg}`;
}

function renderListings(data) {
  const grid = document.getElementById('listingsBody');
  grid.innerHTML = '';
  if (!data.length) {
    grid.innerHTML = `<div class="sec-empty" style="grid-column:1/-1">No listings found for this filter.</div>`;
    return;
  }
  data.forEach(p => {
    const s = statusMap[p.status] || statusMap.sell;
    const isHot = p.note && (p.note.includes('Save') || p.note.includes('Distress') || p.note.includes('Bulk') || p.note.includes('Motivated'));
    const ribbonHTML = isHot
      ? `<div style="position:absolute;top:12px;right:-1px;background:var(--bronze);color:#fff;font-size:0.6rem;letter-spacing:0.12em;text-transform:uppercase;font-weight:700;padding:0.22rem 0.8rem;">🔥 Hot Deal</div>`
      : '';
    grid.innerHTML += `
      <div class="sec-card" style="position:relative;overflow:hidden;">
        ${ribbonHTML}
        <div class="sec-card-top">
          <div class="sec-card-name">${p.name}</div>
          <div class="sec-card-badge"><span class="badge ${s.cls}">${s.label}</span></div>
        </div>
        <div class="sec-card-area">📍 ${p.location}</div>
        <div class="sec-card-details">
          <div class="sec-det-item">
            <div class="sec-det-label">Type</div>
            <div class="sec-det-val">${p.type}</div>
          </div>
          <div class="sec-det-item">
            <div class="sec-det-label">Developer</div>
            <div class="sec-det-val">${p.developer}</div>
          </div>
          <div class="sec-det-item">
            <div class="sec-det-label">Beds</div>
            <div class="sec-det-val">${p.beds}</div>
          </div>
          <div class="sec-det-item">
            <div class="sec-det-label">Size</div>
            <div class="sec-det-val">${p.size !== '—' ? p.size + ' sqft' : '—'}</div>
          </div>
          ${p.note ? `<div class="sec-det-item" style="grid-column:1/-1">
            <div class="sec-det-label">Notes</div>
            <div class="sec-det-val" style="font-weight:400;font-size:0.8rem;color:var(--taupe)">${p.note}</div>
          </div>` : ''}
        </div>
        <div class="sec-card-divider"></div>
        <div class="sec-card-price">AED ${p.price}</div>
        <div class="sec-card-footer">
          <div></div>
          <a href="${buildWaLink(p)}" target="_blank" class="sec-enquire-btn">💬 Enquire</a>
        </div>
      </div>`;
  });
}

function filterListings(type, btn) {
  document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  renderListings(type === 'all' ? listings : listings.filter(l => l.status === type));
}

renderListings(listings);

// ── SECONDARY LISTINGS RENDER ──
const secTypeMap = {
  rent:    { label:"For Rent",       cls:"badge-rent"    },
  sell:    { label:"For Sale",       cls:"badge-sell"    },
  offplan: { label:"Off-Plan Resale",cls:"badge-offplan" },
};
const occupancyMap = {
  "Vacant":       "badge-vacant",
  "Rented":       "badge-rented",
  "Off-Plan":     "badge-offplan",
  "Near Handover":"badge-offplan",
  "—":            "",
};

function buildSecWaLink(p) {
  const typeLabel = secTypeMap[p.type]?.label || p.type;
  const msg =
    `Hi Taher! I'm interested in the following property:%0A` +
    `%F0%9F%8F%A0 *${encodeURIComponent(p.name)}*%0A` +
    `%F0%9F%93%8D Area: ${encodeURIComponent(p.area)}%0A` +
    `%F0%9F%9B%8F Beds: ${p.beds}${p.size && p.size !== '—' ? ' | Size: ' + p.size : ''}%0A` +
    `%F0%9F%92%B0 Price: ${p.price} | ${typeLabel}%0A` +
    (p.note ? `%F0%9F%93%8C Note: ${encodeURIComponent(p.note)}%0A` : '') +
    `Can we discuss further? %F0%9F%94%91`;
  return `https://wa.me/971556472153?text=${msg}`;
}

function renderSecondary(data) {
  const grid = document.getElementById('secGrid');
  grid.innerHTML = '';
  if (!data.length) {
    grid.innerHTML = `<div class="sec-empty">No listings found for this filter.</div>`;
    return;
  }
  data.forEach(p => {
    const t = secTypeMap[p.type] || secTypeMap.sell;
    const occCls = occupancyMap[p.occupancy] || '';
    grid.innerHTML += `
      <div class="sec-card ${p.tag || ''}">
        <div class="sec-card-top">
          <div class="sec-card-name">${p.name}</div>
          <div class="sec-card-badge">
            <span class="badge ${t.cls}">${t.label}</span>
          </div>
        </div>
        <div class="sec-card-area">📍 ${p.area}</div>
        <div class="sec-card-details">
          <div class="sec-det-item">
            <div class="sec-det-label">Beds / Unit</div>
            <div class="sec-det-val">${p.beds}</div>
          </div>
          <div class="sec-det-item">
            <div class="sec-det-label">Size</div>
            <div class="sec-det-val">${p.size}</div>
          </div>
          <div class="sec-det-item">
            <div class="sec-det-label">Occupancy</div>
            <div class="sec-det-val">${p.occupancy}</div>
          </div>
          ${p.note ? `<div class="sec-det-item" style="grid-column:1/-1">
            <div class="sec-det-label">Notes</div>
            <div class="sec-det-val" style="font-weight:400;font-size:0.8rem;color:var(--taupe)">${p.note}</div>
          </div>` : ''}
        </div>
        <div class="sec-card-divider"></div>
        <div class="sec-card-price">${p.price}</div>
        <div class="sec-card-footer">
          <div class="sec-status-row">
            ${occCls ? `<span class="badge ${occCls}">${p.occupancy}</span>` : ''}
          </div>
          <a href="${buildSecWaLink(p)}" target="_blank" class="sec-enquire-btn">💬 Enquire</a>
        </div>
      </div>`;
  });
}

function filterSecondary(type, btn) {
  document.querySelectorAll('.sec-tab').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  renderSecondary(type === 'all' ? secondaryListings : secondaryListings.filter(l => l.type === type));
}

renderSecondary(secondaryListings);
</script>
</body>
</html>
