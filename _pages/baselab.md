---
layout: archive
title: "BASE Lab"
permalink: /baselab/
author_profile: false
---

<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">

<style>
/* ── Hide title, kill top gap, prevent horizontal scroll ── */
.page__title, h1.page__title { display: none !important; }
html, body { overflow-x: hidden; }
#main        { padding-top: 0 !important; margin-top: 0 !important; }
/* Force full-width archive — removes MM's 83% sidebar-aware rule so breakout is symmetric */
.archive {
  width: 100% !important; float: none !important;
  padding-left: 0 !important; margin-left: 0 !important;
  padding-top: 0 !important; margin-top: 0 !important;
}
.page__content { margin-top: 0 !important; padding-top: 0 !important; }
.initial-content { padding-top: 0 !important; }

/* ══════════════════════════════
   HERO
══════════════════════════════ */
.bl-hero {
  position: relative;
  width: 100vw; margin-left: calc(-50vw + 50%);
  min-height: clamp(450px, 36vw, 640px); overflow: hidden;
  margin-top: 0; margin-bottom: 0;
}
.bl-hero-bg {
  position: absolute; inset: 0;
  width: 100%; height: 100%;
  object-fit: cover; object-position: center top; display: block;
}
.bl-hero-fade {
  position: absolute; inset: 0;
  background: linear-gradient(
    to right,
    rgba(255,255,255,0.68)  0%,
    rgba(255,255,255,0.58) 42%,
    rgba(255,255,255,0.12) 66%,
    rgba(255,255,255,0.00) 78%
  );
}
.bl-hero-content {
  position: relative; z-index: 2;
  width: 52%; padding: 40px 36px 48px 52px;
  display: flex; flex-direction: column; justify-content: flex-start;
  min-height: clamp(450px, 36vw, 640px); box-sizing: border-box;
}
.bl-hero-logo { display: block; width: 480px; max-width: 100%; height: auto; margin-bottom: 20px; }
.bl-hero-eyebrow { font-size: 0.76em; font-weight: 700; letter-spacing: 0.16em; text-transform: uppercase; color: #1b8278; margin-bottom: 10px; }
.bl-hero h1 { font-size: 2.7em; font-weight: 800; color: #0d2244; margin: 0 0 14px; line-height: 1.1; letter-spacing: -0.025em; border: none; }
.bl-hero h1 .acc { color: #2a9d8f; }
.bl-hero-tagline { font-size: 1.02em; color: #1e2d4a; line-height: 1.7; margin: 0; }

/* ══════════════════════════════
   BREAKOUT — all sections span full viewport width,
   left edge aligns with hero content (52px from viewport)
══════════════════════════════ */
.bl-breakout {
  width: 100vw; margin-left: calc(-50vw + 50%);
  box-sizing: border-box;
  padding-left: 52px; padding-right: 52px;
}

/* ══════════════════════════════
   SECTION HEADER
══════════════════════════════ */
.bl-section-head { display: flex; align-items: center; gap: 12px; margin-bottom: 14px; }
.bl-bar { width: 32px; height: 4px; background: #2a9d8f; border-radius: 2px; flex-shrink: 0; }
.bl-section-head h2 { font-size: 1.7em; font-weight: 800; color: #0d2244; margin: 0; border: none; }

/* ══════════════════════════════
   MISSION
══════════════════════════════ */
.bl-mission { padding-top: 32px; padding-bottom: 44px; padding-right: 80px; border-bottom: 1px solid #eaecf0; }
.bl-mission-grid {
  display: grid; grid-template-columns: 1fr 340px;
  gap: 48px; align-items: start;
}
.bl-mission-text { padding-right: 84px; }
.bl-mission-text p { font-size: 1.02em; color: #333; line-height: 1.85; margin: 0 0 16px; }
.bl-mission-text p:last-child { margin: 0; }
.bl-hl { color: #2a9d8f; font-weight: 700; }

/* ── Orbit diagram ── */
.bl-diagram { width: 300px; height: 300px; flex-shrink: 0; position: relative; }
.bl-orb-ring { position: absolute; inset: 0; width: 100%; height: 100%; }
.bl-orb-center {
  position: absolute; top: 50%; left: 50%;
  transform: translate(-50%,-50%);
  width: 80px; height: 80px; border-radius: 50%;
  background: #fff; border: 2px solid #2a9d8f;
  box-shadow: 0 0 0 6px rgba(42,157,143,0.12), 0 4px 18px rgba(42,157,143,0.22);
  display: flex; align-items: center; justify-content: center; overflow: hidden;
}
.bl-orb-center img { width: 58px; height: auto; object-fit: contain; }
.bl-on {
  position: absolute; top: 50%; left: 50%;
  margin: -22px; width: 44px; height: 44px;
}
.n0 { transform: rotate(0deg)   translateY(-108px) rotate(0deg); }
.n1 { transform: rotate(45deg)  translateY(-108px) rotate(-45deg); }
.n2 { transform: rotate(90deg)  translateY(-108px) rotate(-90deg); }
.n3 { transform: rotate(135deg) translateY(-108px) rotate(-135deg); }
.n4 { transform: rotate(180deg) translateY(-108px) rotate(-180deg); }
.n5 { transform: rotate(225deg) translateY(-108px) rotate(-225deg); }
.n6 { transform: rotate(270deg) translateY(-108px) rotate(-270deg); }
.n7 { transform: rotate(315deg) translateY(-108px) rotate(-315deg); }
.bl-on-ic {
  width: 44px; height: 44px; border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  font-size: 0.9em; color: #fff;
  border: 2.5px solid rgba(255,255,255,0.9);
  box-shadow: 0 2px 10px rgba(0,0,0,0.25);
}
.bl-on-lbl { position: absolute; white-space: nowrap; }
.bl-on-title {
  display: block; font-size: 12.5px;
  font-weight: 700; color: #1e3a5f; line-height: 1.3;
}
.bl-on-sub {
  display: block; font-size: 9.5px;
  font-weight: 400; color: #6b8fb0; line-height: 1.35;
  font-style: italic;
}
.n0 .bl-on-lbl { bottom: calc(100% + 5px); left: 50%; transform: translateX(-50%); text-align: center; }
.n1 .bl-on-lbl { bottom: calc(100% + 3px); left: calc(100% + 5px); }
.n2 .bl-on-lbl { top: 50%; left: calc(100% + 6px); transform: translateY(-50%); }
.n3 .bl-on-lbl { top: calc(100% + 3px); left: calc(100% + 5px); }
.n4 .bl-on-lbl { top: calc(100% + 5px); left: 50%; transform: translateX(-50%); text-align: center; }
.n5 .bl-on-lbl { top: calc(100% + 3px); right: calc(100% + 5px); text-align: right; }
.n6 .bl-on-lbl { top: 50%; right: calc(100% + 6px); transform: translateY(-50%); text-align: right; }
.n7 .bl-on-lbl { bottom: calc(100% + 3px); right: calc(100% + 5px); text-align: right; }

/* ══════════════════════════════
   RESEARCH THRUSTS
══════════════════════════════ */
.bl-thrusts { padding-top: 44px; padding-bottom: 52px; }
.bl-thrusts .bl-section-head { margin-bottom: 22px; }
.bl-thrusts-grid {
  display: grid; grid-template-columns: repeat(4,minmax(0,1fr));
  gap: 16px;
}
.bl-thrust {
  min-width: 0; /* prevent grid blowout */
  background: #fff; border: 1px solid #e0e4ec;
  border-radius: 10px; overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  transition: box-shadow .2s, transform .2s;
  display: flex; flex-direction: column;
}
.bl-thrust:hover { box-shadow: 0 6px 22px rgba(0,0,0,0.10); transform: translateY(-2px); }

/* Image header on each thrust card */
.bl-thrust-img { height: 152px; overflow: hidden; flex-shrink: 0; }
.bl-thrust-img img {
  width: 100%; height: 100%;
  object-fit: cover; object-position: center 30%;
  display: block; transition: transform .5s ease;
}
.bl-thrust:hover .bl-thrust-img img { transform: scale(1.05); }

.bl-thrust-top { padding: 14px 16px 12px; border-bottom: 1px solid #f0f2f6; }
.bl-thrust-header { display: flex; align-items: center; gap: 10px; margin-bottom: 8px; }
.bl-thrust-num { font-size: 0.72em; font-weight: 800; color: #2a9d8f; letter-spacing: 0.07em; text-transform: uppercase; line-height: 1.2; margin: 0; }
.bl-thrust-icon {
  width: 40px; height: 40px; border-radius: 9px; flex-shrink: 0;
  display: flex; align-items: center; justify-content: center;
  font-size: 1em; color: #fff;
}
.ti1 { background: linear-gradient(135deg,#457b9d,#1d3557); }
.ti2 { background: linear-gradient(135deg,#457b9d,#1d3557); }
.ti3 { background: linear-gradient(135deg,#457b9d,#1d3557); }
.ti4 { background: linear-gradient(135deg,#457b9d,#1d3557); }
.bl-thrust-title { font-size: 0.88em; font-weight: 700; color: #0d2244; line-height: 1.42; }
.bl-thrust-body  { padding: 12px 16px 14px; flex: 1; }
.bl-thrust-tagline { font-size: 0.8em; color: #555; line-height: 1.6; margin-bottom: 10px; font-style: italic; }
.bl-al { font-size: 0.65em; font-weight: 700; text-transform: uppercase; letter-spacing: 0.1em; color: #2a9d8f; margin-bottom: 6px; }
.bl-areas { list-style: none; padding: 0; margin: 0; }
.bl-areas li { font-size: 0.76em; color: #444; line-height: 1.58; padding-left: 20px; position: relative; margin-bottom: 1px; }
.bl-areas li::before { content: '—'; position: absolute; left: 0; color: #ccc; }

/* ── Responsive ── */
@media (max-width: 1200px) {
  .bl-breakout { padding-left: 40px; padding-right: 40px; }
  .bl-hero-content { width: 58%; padding: 36px 28px 40px 40px; }
  .bl-hero-logo { width: 380px; }
  .bl-mission-grid { grid-template-columns: 1fr 300px; gap: 40px; }
  .bl-diagram { width: 300px; }
}
@media (max-width: 960px) {
  .bl-breakout { padding-left: 24px; padding-right: 24px; }
  .bl-hero { min-height: 340px; }
  .bl-hero-content { width: 78%; padding: 26px 18px 30px 24px; min-height: 340px; }
  .bl-hero-logo { width: 260px; }
  .bl-hero h1 { font-size: 2.0em; }
  .bl-mission-grid { grid-template-columns: 1fr; }
  .bl-diagram { width: 280px; margin: 24px auto 0; }
  .bl-thrusts-grid { grid-template-columns: 1fr 1fr; }
}
@media (max-width: 560px) {
  .bl-hero h1 { font-size: 1.55em; }
  .bl-hero-logo { width: 210px; }
  .bl-thrusts-grid { grid-template-columns: 1fr; }
}
</style>

<!-- HERO -->
<div class="bl-hero">
  <img class="bl-hero-bg" src="/images/bl-banner-green.jpg?v=9" alt="BASE Lab — NTU Singapore">
  <div class="bl-hero-fade"></div>
  <div class="bl-hero-content">
    <img src="/images/ntu-base-logo.png" class="bl-hero-logo" alt="NTU Singapore — BASE Lab">
    <div class="bl-hero-eyebrow">BASE LAB @ NTU SINGAPORE</div>
    <h1>Building <span class="acc">Adaptive</span><br>Systems &amp; Environments</h1>
    <p class="bl-hero-tagline"><em>Intelligent, sustainable, and human-centred built environments</em></p>
  </div>
</div>

<!-- MISSION -->
<div class="bl-breakout bl-mission">
  <div class="bl-section-head">
    <div class="bl-bar"></div>
    <h2>Our Mission</h2>
  </div>
  <div class="bl-mission-grid">
    <div class="bl-mission-text">
      <p>BASE Lab develops intelligent and adaptive systems that enable built environments to <span class="bl-hl">sense</span>, <span class="bl-hl">learn</span>, <span class="bl-hl">predict</span>, and <span class="bl-hl">respond</span> to the needs of people and changing environmental conditions.</p>
      <p>We work at the intersection of artificial intelligence, building science, and human-centred approaches to translate data-driven research into real-world building applications. Our research aims to improve building performance, energy efficiency, and occupant wellbeing, creating more <strong>responsive and sustainable built environments</strong>.</p>
    </div>
    <div class="bl-diagram">
      <svg class="bl-orb-ring" viewBox="0 0 300 300" xmlns="http://www.w3.org/2000/svg">
        <line x1="150" y1="150" x2="150" y2="42"  stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="226" y2="74"  stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="258" y2="150" stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="226" y2="226" stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="150" y2="258" stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="74"  y2="226" stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="42"  y2="150" stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <line x1="150" y1="150" x2="74"  y2="74"  stroke="#dde6ef" stroke-width="1" stroke-dasharray="2 3"/>
        <circle cx="150" cy="150" r="108" fill="none" stroke="#c8d8e8" stroke-width="1.5" stroke-dasharray="3 3"/>
        <circle cx="150" cy="42"  r="3.5" fill="#b8ccdf"/>
        <circle cx="226" cy="74"  r="3.5" fill="#b8ccdf"/>
        <circle cx="258" cy="150" r="3.5" fill="#b8ccdf"/>
        <circle cx="226" cy="226" r="3.5" fill="#b8ccdf"/>
        <circle cx="150" cy="258" r="3.5" fill="#b8ccdf"/>
        <circle cx="74"  cy="226" r="3.5" fill="#b8ccdf"/>
        <circle cx="42"  cy="150" r="3.5" fill="#b8ccdf"/>
        <circle cx="74"  cy="74"  r="3.5" fill="#b8ccdf"/>
      </svg>
      <div class="bl-orb-center"><img src="/images/bl-baselogo.png" alt="BASE Lab"></div>
      <div class="bl-on n0"><div class="bl-on-ic" style="background:linear-gradient(135deg,#2a9d8f,#1a7a6e)"><i class="fas fa-users"></i></div><div class="bl-on-lbl"><span class="bl-on-title">People</span><span class="bl-on-sub">Occupants, comfort &amp; wellbeing</span></div></div>
      <div class="bl-on n1"><div class="bl-on-ic" style="background:linear-gradient(135deg,#52b788,#2d6a4f)"><i class="fas fa-leaf"></i></div><div class="bl-on-lbl"><span class="bl-on-title">Sustainability</span><span class="bl-on-sub">Net-zero &amp; carbon resilience</span></div></div>
      <div class="bl-on n2"><div class="bl-on-ic" style="background:linear-gradient(135deg,#e76f51,#c94b2e)"><i class="fas fa-city"></i></div><div class="bl-on-lbl"><span class="bl-on-title">Buildings</span><span class="bl-on-sub">Rooms to urban districts</span></div></div>
      <div class="bl-on n3"><div class="bl-on-ic" style="background:linear-gradient(135deg,#40916c,#1b4332)"><i class="fas fa-wind"></i></div><div class="bl-on-lbl"><span class="bl-on-title">Environment</span><span class="bl-on-sub">IEQ, climate &amp; outdoor air</span></div></div>
      <div class="bl-on n4"><div class="bl-on-ic" style="background:linear-gradient(135deg,#f4a261,#e76f51)"><i class="fas fa-bolt"></i></div><div class="bl-on-lbl"><span class="bl-on-title">Energy</span><span class="bl-on-sub">Efficiency &amp; renewables</span></div></div>
      <div class="bl-on n5"><div class="bl-on-ic" style="background:linear-gradient(135deg,#457b9d,#1d3557)"><i class="fas fa-cogs"></i></div><div class="bl-on-lbl"><span class="bl-on-title">Operations</span><span class="bl-on-sub">Adaptive intelligent control</span></div></div>
      <div class="bl-on n6"><div class="bl-on-ic" style="background:linear-gradient(135deg,#5b8db8,#3a6186)"><i class="fas fa-database"></i></div><div class="bl-on-lbl"><span class="bl-on-title">Sensing &amp; Data</span><span class="bl-on-sub">Multimodal sensing &amp; fusion</span></div></div>
      <div class="bl-on n7"><div class="bl-on-ic" style="background:linear-gradient(135deg,#264653,#2c3e50)"><i class="fas fa-brain"></i></div><div class="bl-on-lbl"><span class="bl-on-title">AI &amp; Analytics</span><span class="bl-on-sub">Learning &amp; prediction</span></div></div>
    </div>
  </div>
</div>

<!-- RESEARCH THRUSTS — images above each card title, no separate strip -->
<div class="bl-breakout bl-thrusts">
  <div class="bl-section-head">
    <div class="bl-bar"></div>
    <h2>Research Thrusts &amp; Areas</h2>
  </div>
  <div class="bl-thrusts-grid">

    <div class="bl-thrust">
      <div class="bl-thrust-img"><img src="/images/bl-thrust-1.jpg?v=3" alt="AI &amp; Predictive Building Analytics"></div>
      <div class="bl-thrust-top">
        <div class="bl-thrust-header">
          <div class="bl-thrust-icon ti1"><i class="fas fa-chart-bar"></i></div>
          <div class="bl-thrust-num">01 — INTELLIGENCE</div>
        </div>
        <div class="bl-thrust-title">Artificial Intelligence &amp; Predictive Building Analytics</div>
      </div>
      <div class="bl-thrust-body">
        <div class="bl-thrust-tagline">Developing data-driven intelligence to understand and anticipate building performance and changing conditions.</div>
        <div class="bl-al">Research Areas</div>
        <ul class="bl-areas">
          <li>Machine learning and predictive analytics</li>
          <li>Multimodal sensing and data fusion</li>
          <li>Building performance forecasting and fault diagnostics</li>
          <li>Digital twins and intelligent building models</li>
        </ul>
      </div>
    </div>

    <div class="bl-thrust">
      <div class="bl-thrust-img"><img src="/images/bl-thrust-2.jpg?v=3" alt="Human-Centred &amp; Living Environments"></div>
      <div class="bl-thrust-top">
        <div class="bl-thrust-header">
          <div class="bl-thrust-icon ti2"><i class="fas fa-users"></i></div>
          <div class="bl-thrust-num">02 — PEOPLE</div>
        </div>
        <div class="bl-thrust-title">Human-Centred and Comfortable Environments</div>
      </div>
      <div class="bl-thrust-body">
        <div class="bl-thrust-tagline">Understanding human needs and creating indoor environments that support comfort, health and wellbeing.</div>
        <div class="bl-al">Research Areas</div>
        <ul class="bl-areas">
          <li>Occupant behaviour, preferences and occupancy</li>
          <li>Personalised thermal comfort</li>
          <li>Indoor environmental quality, health and wellbeing</li>
          <li>Human-building interaction</li>
        </ul>
      </div>
    </div>

    <div class="bl-thrust">
      <div class="bl-thrust-img"><img src="/images/bl-thrust-3.jpg?v=3" alt="Intelligent Building Operations &amp; Control"></div>
      <div class="bl-thrust-top">
        <div class="bl-thrust-header">
          <div class="bl-thrust-icon ti3"><i class="fas fa-cogs"></i></div>
          <div class="bl-thrust-num">03 — OPERATIONS</div>
        </div>
        <div class="bl-thrust-title">Intelligent Building Operations &amp; Control</div>
      </div>
      <div class="bl-thrust-body">
        <div class="bl-thrust-tagline">Translating intelligence into automated decisions and responsive building operations.</div>
        <div class="bl-al">Research Areas</div>
        <ul class="bl-areas">
          <li>Predictive and adaptive control strategies</li>
          <li>HVAC and indoor climate optimisation</li>
          <li>Building automation and integration</li>
          <li>Fault-tolerant and self-correcting systems</li>
        </ul>
      </div>
    </div>

    <div class="bl-thrust">
      <div class="bl-thrust-img"><img src="/images/bl-thrust-4.jpg?v=5" alt="Sustainable Energy Systems &amp; Decarbonisation"></div>
      <div class="bl-thrust-top">
        <div class="bl-thrust-header">
          <div class="bl-thrust-icon ti4"><i class="fas fa-solar-panel"></i></div>
          <div class="bl-thrust-num">04 — SUSTAINABILITY</div>
        </div>
        <div class="bl-thrust-title">Sustainable Energy Systems &amp; Decarbonisation</div>
      </div>
      <div class="bl-thrust-body">
        <div class="bl-thrust-tagline">Reducing building energy use and carbon emissions through efficient and flexible energy systems.</div>
        <div class="bl-al">Research Areas</div>
        <ul class="bl-areas">
          <li>Building energy efficiency and management</li>
          <li>Demand response and energy flexibility</li>
          <li>Renewable energy integration and building-to-grid interaction</li>
          <li>Net-zero buildings and decarbonisation strategies</li>
        </ul>
      </div>
    </div>

  </div>
</div>
