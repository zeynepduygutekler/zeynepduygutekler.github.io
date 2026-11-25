---
layout: archive
title: "Join Us"
permalink: /joinus/
author_profile: false
---

<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">

<style>
/* ── Full-width layout (same pattern as BASE Lab page) ── */
.page__title, h1.page__title { display: none !important; }
html, body { overflow-x: hidden; }
#main { padding-top: 0 !important; margin-top: 0 !important; }
.archive {
  width: 100% !important; float: none !important;
  padding-left: 0 !important; margin-left: 0 !important;
  padding-top: 0 !important; margin-top: 0 !important;
}
.page__content { margin-top: 0 !important; padding-top: 0 !important; }
.initial-content { padding-top: 0 !important; }

/* ── Section structure ── */
.ju-sec { margin-bottom: 44px; }
.ju-head { display: flex; align-items: center; gap: 10px; margin-bottom: 20px; }
.ju-bar { width: 28px; height: 4px; background: #2a9d8f; border-radius: 2px; flex-shrink: 0; }
.ju-head h2 { font-size: 1.3em; font-weight: 800; color: #0d2244; margin: 0; border: none; }

/* ── Featured funded position ── */
.ju-featured {
  background: linear-gradient(135deg, #0d2440 0%, #1a4870 100%);
  border-radius: 12px; padding: 28px 32px; margin-bottom: 40px;
  position: relative; overflow: hidden;
  box-shadow: 0 6px 24px rgba(13,36,64,0.22);
}
.ju-featured::after {
  content: ''; position: absolute; bottom: -50px; right: -50px;
  width: 180px; height: 180px; border-radius: 50%;
  background: rgba(42,157,143,0.13); pointer-events: none;
}
.ju-feat-badge {
  display: inline-flex; align-items: center; gap: 6px;
  background: #2a9d8f; color: #fff;
  font-size: 0.7em; font-weight: 700; letter-spacing: 0.09em;
  text-transform: uppercase; padding: 4px 13px; border-radius: 20px;
  margin-bottom: 14px;
}
.ju-featured h3 { color: #fff; font-size: 1.15em; font-weight: 700; margin: 0 0 10px; border: none; line-height: 1.4; }
.ju-featured p { color: rgba(255,255,255,0.85); font-size: 0.88em; line-height: 1.75; margin: 0 0 18px; }
.ju-feat-tags { display: flex; flex-wrap: wrap; gap: 7px; }
.ju-feat-tag {
  background: rgba(255,255,255,0.1); color: rgba(255,255,255,0.9);
  font-size: 0.74em; padding: 4px 10px; border-radius: 4px;
  border: 1px solid rgba(255,255,255,0.2);
}

/* ── Position cards ── */
.ju-cards { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; }
.ju-card {
  background: #fff; border: 1px solid #dde4ee; border-radius: 10px;
  padding: 20px 22px; border-top: 3px solid #2a9d8f;
  box-shadow: 0 2px 8px rgba(0,0,0,0.04); display: flex; flex-direction: column;
}
.ju-card.ju-slate { border-top-color: #457b9d; }
.ju-card h3 {
  display: flex; align-items: center; gap: 9px;
  font-size: 0.96em; font-weight: 700; color: #0d2244;
  margin: 0 0 10px; border: none;
}
.ju-card h3 i { color: #2a9d8f; width: 16px; text-align: center; }
.ju-card.ju-slate h3 i { color: #457b9d; }
.ju-card p { font-size: 0.83em; color: #444; line-height: 1.62; margin: 0 0 8px; }
.ju-card ul { margin: 4px 0 0; padding-left: 17px; }
.ju-card li { font-size: 0.82em; color: #444; line-height: 1.55; margin-bottom: 4px; }
.ju-card-link {
  display: inline-flex; align-items: center; gap: 5px;
  font-size: 0.78em; font-weight: 600; color: #2a9d8f !important;
  text-decoration: none !important; margin-top: auto; padding-top: 12px;
}
.ju-card.ju-slate .ju-card-link { color: #457b9d !important; }
.ju-card-link i { font-size: 0.85em; }

/* ── Scholarship pill tags ── */
.ju-schol-tags { display: flex; flex-wrap: wrap; gap: 7px; margin-top: 10px; }
.ju-schol-tag {
  display: inline-block; background: #f7fbff; border: 1px solid #c8dff0;
  border-radius: 20px; padding: 5px 13px;
  font-size: 0.77em; font-weight: 600;
  color: #1d3a5f !important; text-decoration: none !important;
  transition: background 0.15s, color 0.15s;
}
.ju-schol-tag:hover { background: #daeef9; color: #2a9d8f !important; }

/* ── Fellowship compact list ── */
.ju-fellow-list { list-style: none; padding: 0; margin: 0 0 14px; }
.ju-fellow-list li { margin-bottom: 8px; }
.ju-fellow-list a { font-size: 0.82em; font-weight: 600; color: #2a9d8f !important; text-decoration: none !important; }
.ju-fellow-list span { display: block; font-size: 0.74em; color: #777; margin-top: 1px; }

/* ── Scholarship table ── */
.ju-scholar-wrap { overflow-x: auto; margin: 10px 0 0; border-radius: 6px; border: 1px solid #dde6ef; }
.ju-scholar-table { width: 100%; border-collapse: collapse; font-size: 0.8em; }
.ju-scholar-table th { background: #0d2244; color: #fff; padding: 8px 12px; text-align: left; font-weight: 600; letter-spacing: 0.04em; white-space: nowrap; }
.ju-scholar-table td { padding: 7px 12px; border-bottom: 1px solid #eaecf0; vertical-align: top; color: #444; line-height: 1.5; }
.ju-scholar-table tr:last-child td { border-bottom: none; }
.ju-scholar-table tr:hover td { background: #f5fbfa; }
.ju-scholar-table .ju-st-cat { background: #f0f8f7; color: #2a9d8f; font-weight: 700; font-size: 0.85em; letter-spacing: 0.06em; padding: 5px 12px; }
.ju-scholar-table .ju-st-cat.ext { background: #f4f6f9; color: #111; }
.ju-st-name { font-weight: 600; color: #2a9d8f !important; text-decoration: none !important; }
.ju-st-sub { display: block; font-size: 0.88em; color: #888; margin-top: 1px; }

/* ── Requirements ── */
.ju-req-grid { display: grid; grid-template-columns: 1fr; gap: 10px; }
.ju-req {
  display: flex; align-items: flex-start; gap: 13px;
  background: #f5fafa; border: 1px solid #dceeed; border-radius: 8px; padding: 14px 16px;
}
.ju-req-ic {
  width: 34px; height: 34px; border-radius: 50%; flex-shrink: 0;
  background: linear-gradient(135deg, #2a9d8f, #1a7a6e);
  display: flex; align-items: center; justify-content: center;
  color: #fff; font-size: 0.78em;
}
.ju-req-body strong { display: block; font-size: 0.84em; color: #0d2244; margin-bottom: 3px; }
.ju-req-body span { font-size: 0.79em; color: #555; line-height: 1.5; }

/* ── How to Apply ── */
.ju-apply-card {
  background: #fff; border: 1px solid #dde4ee; border-radius: 10px;
  padding: 22px 26px; margin-bottom: 12px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.03);
}
.ju-apply-header { display: flex; align-items: center; gap: 14px; margin-bottom: 12px; }
.ju-apply-n {
  width: 34px; height: 34px; border-radius: 50%; flex-shrink: 0;
  background: linear-gradient(135deg, #2a9d8f, #1d3557);
  color: #fff; font-weight: 800; font-size: 0.86em;
  display: flex; align-items: center; justify-content: center;
}
.ju-apply-title { font-size: 1.0em; font-weight: 700; color: #0d2244; margin: 0; }
.ju-apply-body { font-size: 0.86em; color: #444; line-height: 1.72; }
.ju-apply-body a { color: #2a9d8f !important; font-weight: 600; }
.ju-apply-body code {
  background: #f0f4f8; padding: 2px 7px; border-radius: 4px;
  font-size: 0.9em; color: #1d3557; border: 1px solid #dce4f0;
}
.ju-checklist { list-style: none; padding: 0; margin: 14px 0 0; }
.ju-checklist li {
  display: flex; gap: 11px; align-items: flex-start;
  padding: 10px 14px; border-radius: 7px;
  background: #f8fbff; border: 1px solid #e8eef8;
  margin-bottom: 7px; font-size: 0.83em; color: #333; line-height: 1.55;
}
.ju-checklist li i { color: #2a9d8f; margin-top: 2px; flex-shrink: 0; }
.ju-checklist strong { color: #0d2244; }
.ju-routes { list-style: none; padding: 0; margin: 14px 0 0; }
.ju-routes li {
  display: flex; gap: 11px; align-items: flex-start;
  padding: 9px 0; border-bottom: 1px solid #f0f3f7;
  font-size: 0.84em; color: #333; line-height: 1.55;
}
.ju-routes li:last-child { border-bottom: none; }
.ju-routes li i { color: #2a9d8f; margin-top: 2px; flex-shrink: 0; width: 14px; text-align: center; }
.ju-routes li a { color: #2a9d8f !important; font-weight: 600; }

/* ── Note ── */
.ju-note {
  background: linear-gradient(135deg, #f0f8f7, #e4f2f0);
  border-left: 4px solid #2a9d8f; border-radius: 0 8px 8px 0;
  padding: 18px 24px; margin-top: 28px;
  font-size: 0.87em; color: #333; line-height: 1.75;
}
.ju-note strong { color: #0d2244; }

/* ── Accordion positions ── */
.ju-acc {
  background: #fff; border: 1px solid #dde4ee; border-radius: 10px;
  margin-bottom: 10px; border-top: 3px solid #2a9d8f; overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,0.04);
}
.ju-acc.ju-slate { border-top-color: #457b9d; }
.ju-acc > summary {
  display: flex; align-items: center; gap: 12px;
  padding: 16px 22px; cursor: pointer; list-style: none; user-select: none;
}
.ju-acc > summary::-webkit-details-marker { display: none; }
.ju-acc-icon { font-size: 0.96em; color: #2a9d8f; width: 18px; text-align: center; flex-shrink: 0; }
.ju-acc.ju-slate .ju-acc-icon { color: #457b9d; }
.ju-acc-title { font-size: 0.96em; font-weight: 700; color: #0d2244; flex: 1; }
.ju-acc-badge {
  font-size: 0.72em; font-weight: 600; padding: 3px 11px; border-radius: 20px;
  background: #e8f7f5; color: #2a9d8f; flex-shrink: 0;
}
.ju-acc.ju-slate .ju-acc-badge { background: #edf3f8; color: #457b9d; }
.ju-acc-arrow { color: #bbb; font-size: 0.78em; transition: transform 0.2s; flex-shrink: 0; }
.ju-acc[open] > summary .ju-acc-arrow { transform: rotate(180deg); }
.ju-acc-body { padding: 0 22px 20px; border-top: 1px solid #f0f3f7; }
.ju-sub-acc {
  margin: 10px 0 4px; border: 1px solid #e0e8f0; border-radius: 8px; overflow: hidden;
}
.ju-sub-acc > summary {
  padding: 9px 14px; cursor: pointer; list-style: none; display: flex; align-items: center;
  font-size: 0.80em; font-weight: 700; color: #0d2244; background: #f8fbff; gap: 6px;
}
.ju-sub-acc > summary::-webkit-details-marker { display: none; }
.ju-sub-arrow { margin-left: auto; color: #bbb; font-size: 0.82em; transition: transform 0.2s; }
.ju-sub-acc[open] > summary .ju-sub-arrow { transform: rotate(180deg); }
.ju-sub-acc-body { padding: 8px 14px 12px; }

@media (max-width: 760px) {
  .ju-cards, .ju-req-grid { grid-template-columns: 1fr; }
  .ju-featured { padding: 22px 20px; }
  .ju-wrap { padding: 24px 20px !important; }
}
</style>

<div class="ju-wrap" style="padding: 8px 52px;">

<!-- ── Header ── -->
<div style="display:flex; align-items:center; gap:28px; margin-bottom:28px; padding:28px 32px; border-radius:14px; overflow:hidden; position:relative; background-image:url('/images/bl-banner.png'); background-size:cover; background-position:center 40%; box-shadow:0 4px 18px rgba(0,0,0,0.10); flex-wrap:wrap;">
  <div style="position:absolute; inset:0; background:rgba(255,255,255,0.40);"></div>
  <img src="/images/ntu-base-logo.png" alt="NTU Singapore — BASE Lab" style="height:150px; object-fit:contain; flex-shrink:0; position:relative; z-index:1;">
  <div style="position:relative; z-index:1;">
    <h1 style="font-size:2em; font-weight:800; color:#0d2244; margin:0 0 5px; line-height:1.15; border:none;">Join Us</h1>
    <p style="font-size:0.88em; color:#457b9d; margin:0; font-weight:600; letter-spacing:0.01em;">BASE Lab @ NTU Singapore</p>
  </div>
</div>

<!-- ── Intro ── -->
<div style="margin-bottom:36px; padding-bottom:28px; border-bottom:1px solid #eaecf0;">
  <p style="font-size:1.0em; color:#2a3a4a; line-height:1.82; margin:0 0 12px;"><strong><a href="https://zeynepduygutekler.github.io/baselab/" target="_blank" style="color:#2a9d8f;">BASE Lab @ NTU Singapore</a></strong> welcomes motivated researchers interested in advancing AI-driven solutions for intelligent and sustainable built environments. We offer opportunities for PhD students, postdoctoral researchers, and visiting researchers to pursue impactful research, develop new ideas, and contribute to real-world applications.</p>
  <p style="font-size:1.0em; color:#2a3a4a; line-height:1.82; margin:0 0 12px;">Our team is also actively engaged in international research collaborations with leading researchers and institutions worldwide, including the University of Oxford and Loughborough University in the United Kingdom.</p>
  <p style="font-size:0.92em; color:#6a7a8a; line-height:1.72; margin:0;"><strong>Explore our current openings and find the right opportunity for you below.</strong></p>
</div>

<!-- ══════════════════════════════
     FEATURED FUNDED POSITION
══════════════════════════════ -->
<div class="ju-featured">
  <div class="ju-feat-badge"><i class="fas fa-star"></i>&nbsp; PhD + Postdoc Positions — Open Now</div>
  <h3>Agentic AI &amp; Large Language Models for Intelligent Buildings</h3>
  <p>We are recruiting <strong>two PhD students and two postdoctoral researchers</strong> for a funded project developing a human-centric agentic AI system for next-generation building automation. The project integrates large language models (LLMs), multimodal sensing, and domain knowledge to enable buildings to learn occupant preferences, reason about environmental conditions, and adapt operations to enhance human comfort and energy efficiency. See the requirements below.</p>
  <div class="ju-feat-tags">
    <span class="ju-feat-tag"><i class="fas fa-robot" style="margin-right:4px;"></i>Agentic AI Systems</span>
    <span class="ju-feat-tag">Large Language Models</span>
    <span class="ju-feat-tag">Multimodal Sensing</span>
    <span class="ju-feat-tag">Personalised Building Control</span>
  </div>
</div>

<!-- ══════════════════════════════
     OPEN POSITIONS
══════════════════════════════ -->
<div class="ju-sec">
  <div class="ju-head"><div class="ju-bar"></div><h2>Open Positions</h2></div>
  <!-- PhD -->
  <details class="ju-acc">
    <summary><i class="fas fa-graduation-cap ju-acc-icon"></i><span class="ju-acc-title">PhD Students</span><span class="ju-acc-badge">Actively Recruiting · Aug 2027</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 10px;">Open to Singaporeans, Singapore PRs, and international students with a strong background in engineering, data science, built environment, or a related field. Actively recruiting for the <strong>August 2027 intake</strong>.</p>
      <div style="margin-top:10px;">

        <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:0 0 6px; text-transform:uppercase; letter-spacing:0.07em;"><i class="fas fa-university" style="color:#2a9d8f; margin-right:5px;"></i>NTU MAE PhD Programme</p>
        <p style="font-size:0.82em; color:#444; margin:0 0 10px; line-height:1.62;">The primary route for PhD admission at NTU. Successful applicants are considered for the <a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU Research Scholarship (RSS)</a> — covering tuition and a monthly stipend.</p>
        <div style="background:#f0f8f7; border:1px solid #c8e6e2; border-radius:7px; padding:12px 15px; margin-bottom:12px;">
          <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:0 0 7px;">How it works</p>
          <ul style="margin:0; padding-left:16px;">
            <li style="font-size:0.82em; color:#444; margin-bottom:5px;">Contact me first — email your CV and a research statement. See <a href="#how-to-apply" style="color:#2a9d8f;font-weight:600;">How to Apply</a> below.</li>
            <li style="font-size:0.82em; color:#444; margin-bottom:5px;">Apply via the <a href="https://www.ntu.edu.sg/education/graduate-programme/mae-phd" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU graduate admissions portal</a></li>
            <li style="font-size:0.82em; color:#444;">Shortlisted candidates will be invited for an interview</li>
          </ul>
        </div>
        <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:0 0 5px;">Intake Deadlines</p>
        <ul style="margin:0 0 8px; padding-left:17px;">
          <li style="font-size:0.82em; color:#444; margin-bottom:4px;">August 2027 Intake: deadline <strong>31 January</strong> (portal opens 1 Oct 2026)</li>
          <li style="font-size:0.82em; color:#444; margin-bottom:4px;">January 2028 Intake: deadline <strong>31 July</strong> (portal opens 1 Jun 2027)</li>
        </ul>
        <p style="font-size:0.79em; color:#555; margin:0 0 20px; line-height:1.65;">Before starting this process, please read through the <a href="https://www.ntu.edu.sg/admissions/graduate/radmissionguide?utm" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU Graduate Admission Guidelines</a> carefully to understand the full process, eligibility, and document requirements.</p>

        <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:0 0 6px; text-transform:uppercase; letter-spacing:0.07em;"><i class="fas fa-award" style="color:#2a9d8f; margin-right:5px;"></i>Other PhD Scholarships</p>
        <p style="font-size:0.79em; color:#666; margin:0 0 10px; line-height:1.55;">The following scholarships are either <strong>NTU-awarded</strong> or <strong>externally funded</strong>, each requiring a separate application. All follow NTU's August or January intake cycles. Check each official website for current deadlines and eligibility — if interested, email me your CV indicating your intended scholarship.</p>
        <details class="ju-sub-acc">
          <summary><i class="fas fa-list" style="color:#2a9d8f;"></i> View scholarships <i class="fas fa-chevron-down ju-sub-arrow"></i></summary>
          <div class="ju-sub-acc-body">
            <div class="ju-scholar-wrap">
              <table class="ju-scholar-table">
                <thead>
                  <tr>
                    <th>Scholarship</th>
                    <th>Eligibility</th>
                    <th>Typical Deadline</th>
                    <th>Details</th>
                  </tr>
                </thead>
                <tbody>
                  <tr><td colspan="4" class="ju-st-cat ext">NTU-AWARDED</td></tr>
                  <tr>
                    <td><a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships/npgs" target="_blank" class="ju-st-name">NPGS</a><span class="ju-st-sub">Nanyang President's Graduate Scholarship</span></td>
                    <td>All nationalities</td>
                    <td>Nomination only (1 Nov – 31 Dec)</td>
                    <td>Full tuition, monthly stipend, and annual conference allowance. Outstanding academic record and research potential; Highest Distinction or equivalent.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships/pga" target="_blank" class="ju-st-name">PGA</a><span class="ju-st-sub">Provost's Graduate Award</span></td>
                    <td>All nationalities</td>
                    <td>Nomination only (~1 Nov – 31 Dec)</td>
                    <td>Additional monthly allowance on top of RSS. Highest Distinction or equivalent; exceptional research potential.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.ntu.edu.sg/graduate-college/admissions/scholarships/yunqi-phd-scholarship-in-science-and-technology" target="_blank" class="ju-st-name">Yunqi PhD Scholarship</a><span class="ju-st-sub">Science &amp; Technology</span></td>
                    <td>All nationalities</td>
                    <td>Aligns with NTU PhD intake deadlines (31 Jan for Aug; 31 Jul for Jan) — check <a href="https://www.ntu.edu.sg/graduate-college/admissions/scholarships/yunqi-phd-scholarship-in-science-and-technology" target="_blank" style="color:#2a9d8f;">NTU portal</a></td>
                    <td>Full tuition and monthly stipend for PhD candidates in science and technology at NTU.</td>
                  </tr>
                  <tr><td colspan="4" class="ju-st-cat ext">EXTERNALLY FUNDED</td></tr>
                  <tr>
                    <td><a href="https://aisingapore.org/research/phd-fellowship-programme/" target="_blank" class="ju-st-name">AISG PhD Fellowship</a><span class="ju-st-sub">AI Singapore</span></td>
                    <td>All nationalities (SG/PR/ASEAN encouraged)</td>
                    <td>Annual (~Oct) — nomination by supervisor; check <a href="https://aisingapore.org/research/phd-fellowship-programme/" target="_blank" style="color:#2a9d8f;">AISG website</a></td>
                    <td>Full tuition, monthly stipend, and conference travel support. Focused on AI fundamental research. Nomination-based.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.a-star.edu.sg/scholarships/home/scholarships/ags--scholarship" target="_blank" class="ju-st-name">A*STAR Graduate Scholarship (AGS)</a><span class="ju-st-sub">A*STAR</span></td>
                    <td>All nationalities</td>
                    <td>Round 1: 1 Nov–1 Feb &nbsp;|&nbsp; Round 2: 1 Jun–10 Aug</td>
                    <td>Full tuition, monthly stipend, and overseas research attachment support. International awardees commit to 3 years of work in Singapore post-graduation.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.a-star.edu.sg/Scholarships" target="_blank" class="ju-st-name">SINGA</a><span class="ju-st-sub">Singapore International Graduate Award</span></td>
                    <td>International students</td>
                    <td>Annual (~Jun for Jan intake)</td>
                    <td>Full tuition, monthly stipend, and one-time airfare grant. Joint A*STAR–NTU PhD programme.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.psc.gov.sg/scholarships/postgraduate-scholarships/lee-kuan-yew-scholarship" target="_blank" class="ju-st-name">Lee Kuan Yew Scholarship</a><span class="ju-st-sub">Public Service Commission</span></td>
                    <td>Singapore citizens only</td>
                    <td>Annual (~Jan–Mar) — check <a href="https://www.psc.gov.sg/scholarships/postgraduate-scholarships/lee-kuan-yew-scholarship" target="_blank" style="color:#2a9d8f;">PSC website</a></td>
                    <td>Full tuition and generous annual allowance for up to 5 years. Highly competitive; no bond requirement.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" class="ju-st-name">EDB Industrial Postgraduate Programme (IPP)</a><span class="ju-st-sub">EDB + Industry Partner</span></td>
                    <td>Singapore citizens &amp; PRs</td>
                    <td>Ongoing — check <a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" style="color:#2a9d8f;">NTU portal</a></td>
                    <td>Industry co-funded PhD with an EDB industry partner. Applied research focus relevant to energy, built environment, and AI.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.csc.edu.cn/studyabroad" target="_blank" class="ju-st-name">China Scholarship Council (CSC)</a><span class="ju-st-sub">Chinese Government</span></td>
                    <td>Chinese citizens</td>
                    <td>Annual (~Mar–Apr); apply to CSC and NTU separately</td>
                    <td>Covers tuition, monthly stipend, one round-trip airfare, and health insurance. Students apply to CSC and NTU independently.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" class="ju-st-name">LPDP–NTU Graduate Scholarship</a><span class="ju-st-sub">Indonesian Government</span></td>
                    <td>Indonesian citizens</td>
                    <td>Multiple rounds (~Feb, Jun, Oct) — check <a href="https://www.lpdp.kemenkeu.go.id" target="_blank" style="color:#2a9d8f;">LPDP website</a></td>
                    <td>Full tuition, monthly stipend, and research support. Indonesia's prestigious government scholarship; NTU is a supported partner institution.</td>
                  </tr>
                  <tr>
                    <td><a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" class="ju-st-name">VinGroup Graduate Scholarship</a><span class="ju-st-sub">VinGroup (Vietnam)</span></td>
                    <td>Vietnamese citizens</td>
                    <td>Annual — check <a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" style="color:#2a9d8f;">NTU portal</a></td>
                    <td>Tuition and monthly stipend for STEM PhD students at NTU. Funded by Vietnam's VinGroup foundation.</td>
                  </tr>
                  <tr><td colspan="4" class="ju-st-cat ext">SELF-FUNDED / PART-TIME</td></tr>
                  <tr>
                    <td><span class="ju-st-name" style="color:#444; cursor:default;">Self-Funded PhD</span><span class="ju-st-sub">All nationalities</span></td>
                    <td>All nationalities</td>
                    <td>Apply at any time</td>
                    <td>Self-funded applicants are welcome and should note this clearly in their cover letter. Please contact me to discuss your circumstances before applying.</td>
                  </tr>
                  <tr>
                    <td><span class="ju-st-name" style="color:#444; cursor:default;">Part-Time PhD</span><span class="ju-st-sub">Working professionals</span></td>
                    <td>Subject to NTU eligibility</td>
                    <td>Apply at any time</td>
                    <td>Part-time PhD study may be available to working professionals, subject to NTU's admission requirements. Please contact me to discuss suitability.</td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </details>

      </div>
    </div>
  </details>

  <!-- Postdoc -->
  <details class="ju-acc">
    <summary><i class="fas fa-microscope ju-acc-icon"></i><span class="ju-acc-title">Postdoctoral Researchers</span><span class="ju-acc-badge">2 Funded Positions</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 6px;"><strong>Project-funded openings:</strong> We have two funded Postdoctoral positions on our current project on agentic AI and LLMs for intelligent buildings. See the featured position at the top of this page and follow the steps in <a href="#how-to-apply" style="color:#2a9d8f;font-weight:600;">How to Apply</a> below.</p>
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:0 0 8px;"><strong>External fellowship positions:</strong> We also welcome applications from candidates holding or applying for independent fellowships. If interested, check the requirements and get in touch.</p>
      <details class="ju-sub-acc">
        <summary><i class="fas fa-list" style="color:#2a9d8f;"></i> View fellowship opportunities <i class="fas fa-chevron-down ju-sub-arrow"></i></summary>
        <div class="ju-sub-acc-body">
          <div class="ju-scholar-wrap">
            <table class="ju-scholar-table">
              <thead>
                <tr>
                  <th>Fellowship</th>
                  <th>Eligibility</th>
                  <th>Typical Deadline</th>
                  <th>Details</th>
                </tr>
              </thead>
              <tbody>
                <tr><td colspan="4" class="ju-st-cat ext">NTU-BASED</td></tr>
                <tr>
                  <td><a href="https://www.ntu.edu.sg/research/research-careers/lee-kuan-yew-postdoctoral-fellowship-(lkypdf)" target="_blank" class="ju-st-name">Lee Kuan Yew Postdoctoral Fellowship</a><span class="ju-st-sub">Nanyang Technological University</span></td>
                  <td>All nationalities; early-career researchers</td>
                  <td>25 Nov – 10 Feb — check <a href="https://www.ntu.edu.sg/research/research-careers/lee-kuan-yew-postdoctoral-fellowship-(lkypdf)" target="_blank" style="color:#2a9d8f;">NTU website</a></td>
                  <td>Prestigious NTU fellowship for outstanding early-career researchers. Covers full salary, research allowances, and travel support.</td>
                </tr>
                <tr>
                  <td><a href="https://www.ntu.edu.sg/research/research-careers/presidential-postdoctoral-fellowship-(ppf)" target="_blank" class="ju-st-name">Presidential Postdoctoral Fellowship (PPF)</a><span class="ju-st-sub">Nanyang Technological University</span></td>
                  <td>All nationalities; within 5 years of PhD</td>
                  <td>Varies by scheme (~31 Dec for Wallenberg) — check <a href="https://www.ntu.edu.sg/research/research-careers/presidential-postdoctoral-fellowship-(ppf)" target="_blank" style="color:#2a9d8f;">NTU website</a></td>
                  <td>Competitive salary, up to SGD $100,000/year research grant, and housing support. Includes Wallenberg-NTU PPF (AI &amp; autonomous systems) and SP Group–NTU PPF (energy &amp; power systems) schemes.</td>
                </tr>
                <tr>
                  <td><a href="https://www.ntu.edu.sg/research/research-careers/the-eric-and-wendy-schmidt-ai-in-science-postdoctoral-fellowship" target="_blank" class="ju-st-name">Schmidt AI in Science Fellowship</a><span class="ju-st-sub">Eric &amp; Wendy Schmidt / NTU</span></td>
                  <td>All nationalities; within 3 years of PhD; AI applied to engineering or natural sciences</td>
                  <td>Annual (deadline 31 Dec) — check <a href="https://www.ntu.edu.sg/research/research-careers/the-eric-and-wendy-schmidt-ai-in-science-postdoctoral-fellowship" target="_blank" style="color:#2a9d8f;">NTU website</a></td>
                  <td>Two-year fellowship covering salary, travel, and AI training. Research cannot be in computer science itself.</td>
                </tr>
                <tr>
                  <td><a href="https://www.ntu.edu.sg/research/research-careers/ntu-ai-for-x-postdoctoral-fellowship" target="_blank" class="ju-st-name">NTU AI-for-X Postdoctoral Fellowship (AI4X)</a><span class="ju-st-sub">Nanyang Technological University</span></td>
                  <td>All nationalities; early-career researchers</td>
                  <td>Annual (deadline ~30 Oct) — check <a href="https://www.ntu.edu.sg/research/research-careers/ntu-ai-for-x-postdoctoral-fellowship" target="_blank" style="color:#2a9d8f;">NTU website</a></td>
                  <td>Fellowship for early-career researchers applying AI to diverse domains. Supports independent AI-driven research.</td>
                </tr>
                <tr>
                  <td><a href="https://www.nrf.gov.sg/grants/nrff/" target="_blank" class="ju-st-name">NRF Fellowship</a><span class="ju-st-sub">National Research Foundation, Singapore</span></td>
                  <td>All nationalities; early-career researchers</td>
                  <td>Annual (~Aug–Sep) — check <a href="https://www.nrf.gov.sg/grants/nrff/" target="_blank" style="color:#2a9d8f;">NRF website</a></td>
                  <td>Highly competitive national fellowship for establishing an independent research programme. Comes with a substantial 5-year grant.</td>
                </tr>
                <tr>
                  <td><a href="https://www.a-star.edu.sg/Scholarships" target="_blank" class="ju-st-name">A*STAR Research Fellowship Singapore</a><span class="ju-st-sub">Agency for Science, Technology and Research</span></td>
                  <td>Singapore citizens &amp; PRs</td>
                  <td>Annual — check <a href="https://www.a-star.edu.sg/Scholarships" target="_blank" style="color:#2a9d8f;">A*STAR website</a></td>
                  <td>Supports postdoctoral research at A*STAR institutes or local universities, with a focus on applied research.</td>
                </tr>
                <tr>
                  <td><a href="https://marie-sklodowska-curie-actions.ec.europa.eu/" target="_blank" class="ju-st-name">Marie Skłodowska-Curie Actions (MSCA)</a><span class="ju-st-sub">European Commission</span></td>
                  <td>All nationalities</td>
                  <td>Annual (~Sep–Nov) — check <a href="https://marie-sklodowska-curie-actions.ec.europa.eu/" target="_blank" style="color:#2a9d8f;">EU website</a></td>
                  <td>EU Horizon programme supporting international mobility. Covers salary, travel, and research cost allowances.</td>
                </tr>
                <tr>
                  <td><a href="https://www.humboldt-foundation.de/" target="_blank" class="ju-st-name">Alexander von Humboldt Research Fellowship</a><span class="ju-st-sub">Alexander von Humboldt Foundation</span></td>
                  <td>All nationalities; researchers based outside Germany</td>
                  <td>Rolling — apply at any time</td>
                  <td>Internationally recognised fellowship for extended research stays. Open to all career stages; covers salary and research costs.</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </details>
      <p style="font-size:0.80em; color:#6a7a8a; line-height:1.62; margin:12px 0 0; border-top:1px solid #f0f3f7; padding-top:10px;"><i class="fas fa-clock" style="color:#457b9d; margin-right:5px;"></i><strong>Timeline:</strong> The hiring process of international candidates typically takes 3–5 months from initial contact to start date, depending on administrative and visa requirements. Singaporeans and SPRs may have a shorter lead time.</p>
    </div>
  </details>

  <!-- Research Assistants -->
  <details class="ju-acc ju-slate">
    <summary><i class="fas fa-flask ju-acc-icon"></i><span class="ju-acc-title">Research Assistants</span><span class="ju-acc-badge">Rolling Basis</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 10px;">We hire Research Assistants on short-term contracts or on an hourly basis for candidates with relevant experience. These positions are suited to recent graduates looking to gain research experience before a PhD, or those with strong technical skills who want to contribute to active projects in AI, sensing, and building systems. If you have relevant experience and are interested in contributing, please get in touch with your CV and a brief description of your background.</p>
      <p style="font-size:0.80em; color:#6a7a8a; line-height:1.62; margin:0; border-top:1px solid #f0f3f7; padding-top:10px;"><i class="fas fa-clock" style="color:#457b9d; margin-right:5px;"></i><strong>Timeline:</strong> The hiring process of international candidates typically takes 3–5 months from initial contact to start date, depending on administrative and visa requirements. Singaporeans and SPRs may have a shorter lead time.</p>
    </div>
  </details>

  <!-- Visiting -->
  <details class="ju-acc ju-slate">
    <summary><i class="fas fa-globe-asia ju-acc-icon"></i><span class="ju-acc-title">Visiting Students &amp; Researchers</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 8px;">We welcome self-funded visiting students and researchers from partner universities. NTU's <strong>Non-Graduating, Non-Exchange (NGNE) programme</strong> supports research visits of up to two years. Please email me well in advance to discuss a proposed research plan. Visits work best when there is a clear, mutually beneficial research agenda.</p>
      <a href="https://www.ntu.edu.sg/education/student-exchanges/visiting-research" target="_blank" class="ju-card-link"><i class="fas fa-external-link-alt"></i> NTU Visiting Research (NGNE)</a>
    </div>
  </details>

  <!-- Masters -->
  <details class="ju-acc ju-slate">
    <summary><i class="fas fa-book-open ju-acc-icon"></i><span class="ju-acc-title">Master's Students (NTU)</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 8px;">We welcome NTU Master's students interested in research on AI, sensing, building systems, occupant behaviour, or energy. Two routes are available:</p>
      <p style="font-size:0.82em; font-weight:700; color:#0d2244; margin:10px 0 3px; text-transform:uppercase; letter-spacing:0.06em;"><a href="https://www.ntu.edu.sg/mae/admissions/graduate-programmes" target="_blank" style="color:#0d2244;">MSc / MEng by Research</a></p>
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:0 0 8px;">NTU offers two annual intakes (August and January). Applications are typically due 4–6 months before the intended start date. If you are interested, please get in touch well ahead of the deadline. Send your CV, academic transcript, and a short cover letter describing your research interests and why you would like to join BASE Lab. See the <a href="https://www.ntu.edu.sg/admissions/graduate/radmissionguide" target="_blank" style="color:#2a9d8f;">NTU Graduate Admissions Guide</a> for details.</p>
      <p style="font-size:0.82em; font-weight:700; color:#0d2244; margin:10px 0 3px; text-transform:uppercase; letter-spacing:0.06em;">MSc by Coursework (Dissertation / Independent Project)</p>
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:0 0 8px;">If you are already enrolled in an NTU MSc programme and are looking for a dissertation supervisor or an independent research project, please get in touch at the start of each semester to discuss available topics and project fit.</p>
      <p style="font-size:0.79em; color:#888; line-height:1.6; margin:10px 0 0;"><i class="fas fa-info-circle" style="color:#457b9d; margin-right:4px;"></i>Master's programmes are self-funded. BASE Lab does not provide tuition fee support or a stipend for Master's students unless a specific funded project is available.</p>
    </div>
  </details>

  <!-- Undergrad -->
  <details class="ju-acc ju-slate">
    <summary><i class="fas fa-user-graduate ju-acc-icon"></i><span class="ju-acc-title">Undergraduate Researchers (NTU)</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 8px;">NTU undergraduates are welcome to get involved in research through the following programmes:</p>
      <p style="font-size:0.82em; font-weight:700; color:#0d2244; margin:10px 0 3px; text-transform:uppercase; letter-spacing:0.06em;"><a href="https://www.ntu.edu.sg/mae/admissions/current-students/undergraduate/final-year-project" target="_blank" style="color:#0d2244;">Final Year Project (FYP)</a></p>
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:0 0 8px;">We offer FYP topics in areas such as AI for building energy management, occupant sensing and behaviour modelling, agentic systems for smart buildings, and data-driven HVAC optimisation. If you are interested, reach out early — project slots are limited and filled on a first-come basis.</p>
      <p style="font-size:0.82em; font-weight:700; color:#0d2244; margin:10px 0 3px; text-transform:uppercase; letter-spacing:0.06em;"><a href="https://www.ntu.edu.sg/education/undergraduate-research-experience-on-campus-(ureca)" target="_blank" style="color:#0d2244;">URECA (Undergraduate Research Experience on Campus)</a></p>
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:0 0 8px;">URECA provides a funded research opportunity for high-achieving undergraduates to work on live research projects alongside the team. We welcome applications from motivated students who can commit consistently to the project.</p>
      <p style="font-size:0.82em; font-weight:700; color:#0d2244; margin:10px 0 3px; text-transform:uppercase; letter-spacing:0.06em;">Independent Research Project (IRP) &amp; Summer Research</p>
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:0 0 8px;">Students interested in short-term or summer research attachments are welcome to get in touch. Please note that BASE Lab cannot provide financial support for self-funded summer research at this time.</p>
      <p style="font-size:0.79em; color:#888; line-height:1.6; margin:10px 0 0;"><i class="fas fa-paper-plane" style="color:#457b9d; margin-right:4px;"></i>To apply for any of the above, email me with your CV, academic transcript, and a short paragraph on the research area that interests you most and why.</p>
    </div>
  </details>
</div>

<!-- ══════════════════════════════
     WHAT WE LOOK FOR
══════════════════════════════ -->
<div class="ju-sec">
  <div class="ju-head"><div class="ju-bar"></div><h2>What We Look For</h2></div>
  <p style="font-size:0.92em; color:#555; line-height:1.72; margin:0 0 16px;">We welcome applicants with diverse backgrounds who share a strong interest in AI, sensing, and sustainable built environments.</p>
  <div class="ju-req-grid">
    <div class="ju-req">
      <div class="ju-req-ic"><i class="fas fa-university"></i></div>
      <div class="ju-req-body">
        <strong>Academic Background</strong>
        <span>A bachelor's or master's degree in Engineering, Computer Science, Data Science, or a related field is required for PhD applicants. Postdoctoral applicants must hold a PhD in a relevant discipline. A strong academic record is expected for both.</span>
      </div>
    </div>
    <div class="ju-req">
      <div class="ju-req-ic"><i class="fas fa-code"></i></div>
      <div class="ju-req-body">
        <strong>Programming &amp; Technical Skills</strong>
        <span>Proficiency in Python is essential. For PhD applicants, experience with ML frameworks such as PyTorch, TensorFlow, or scikit-learn is an advantage. Postdoctoral candidates are expected to demonstrate strong hands-on experience with ML/DL frameworks, data analysis tools, and ideally familiarity with LLMs or agentic AI systems.</span>
      </div>
    </div>
    <div class="ju-req">
      <div class="ju-req-ic"><i class="fas fa-brain"></i></div>
      <div class="ju-req-body">
        <strong>Research Experience &amp; Domain Interest</strong>
        <span>A strong background in AI, sensing, sustainable built environments, or energy systems. Prior research experience and thesis work are advantageous for PhD applicants; publications in reputable journals are a plus. Postdoctoral candidates should have a strong publication record and demonstrated ability to lead independent research.</span>
      </div>
    </div>
    <div class="ju-req">
      <div class="ju-req-ic"><i class="fas fa-users"></i></div>
      <div class="ju-req-body">
        <strong>Communication &amp; Collaboration</strong>
        <span>Excellent written and verbal communication in English, with the ability to clearly articulate research ideas and direction. We look for self-motivated researchers who work well both independently and as part of a team, and who bring intellectual rigour, curiosity, openness to feedback, and a genuine commitment to meaningful research.</span>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════
     HOW TO APPLY
══════════════════════════════ -->
<div class="ju-sec">
  <div class="ju-head"><div class="ju-bar"></div><h2 id="how-to-apply">How to Apply</h2></div>

  <div class="ju-apply-card">
    <div class="ju-apply-header">
      <div class="ju-apply-n">1</div>
      <div class="ju-apply-title">Get in touch</div>
    </div>
    <div class="ju-apply-body">
      Email <a href="mailto:zeynep.tekler@ntu.edu.sg"><strong>zeynep.tekler@ntu.edu.sg</strong></a> with subject: <code>[PhD/Postdoc/Visiting Researcher – Programme] Your Name</code>
      <ul style="margin:10px 0 0; padding-left:18px;">
        <li style="font-size:0.92em; color:#444; margin-bottom:6px; line-height:1.6;"><strong>CV</strong> — education, research experience, publications (if any), and two referee contacts</li>
        <li style="font-size:0.92em; color:#444; margin-bottom:6px; line-height:1.6;"><strong>Research statement</strong> — one page on why BASE Lab, your research interests, and the direction you hope to pursue</li>
        <li style="font-size:0.92em; color:#444; line-height:1.6;"><strong>Relevant work</strong> — links to publications, code, or a personal website (optional but welcome)</li>
      </ul>
    </div>
  </div>

  <div class="ju-apply-card">
    <div class="ju-apply-header">
      <div class="ju-apply-n">2</div>
      <div class="ju-apply-title">Follow the application route</div>
    </div>
    <div class="ju-apply-body">
      After an initial exchange and confirming a mutual fit, follow the next steps:
      <ul style="margin:10px 0 0; padding-left:18px;">
        <li style="font-size:0.92em; color:#444; margin-bottom:6px; line-height:1.6;"><strong>PhD:</strong> <a href="https://www.ntu.edu.sg/education/graduate-programme/mae-phd#admission" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU MAE PhD Programme</a> or relevant scholarship route</li>
        <li style="font-size:0.92em; color:#444; margin-bottom:6px; line-height:1.6;"><strong>Postdoc and RA:</strong> email me directly to discuss your background and fit, then apply through the NTU Workday portal for <a href="https://ntu.wd3.myworkdayjobs.com/Careers/job/NTU-Main-Campus-Singapore/Research-Fellow--AI---Data-Science-for-Sustainable-Built-Environment-_R00026486" target="_blank" style="color:#2a9d8f;font-weight:600;">Research Fellow (RF)</a> or <a href="https://ntu.wd3.myworkdayjobs.com/Careers/job/NTU-Main-Campus-Singapore/Senior-Research-Fellow--AI---Data-Science-for-Sustainable-Built-Environment-_R00026485" target="_blank" style="color:#2a9d8f;font-weight:600;">Senior Research Fellow (SRF)</a></li>
        <li style="font-size:0.92em; color:#444; margin-bottom:6px; line-height:1.6;"><strong>Visiting researchers:</strong> <a href="https://www.ntu.edu.sg/education/student-exchanges/visiting-research" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU NGNE application process</a></li>
        <li style="font-size:0.92em; color:#444; line-height:1.6;"><strong>NTU Master's &amp; undergraduates:</strong> get in touch to discuss dissertation, FYP, or URECA projects</li>
      </ul>
    </div>
  </div>

  <div class="ju-apply-card">
    <div class="ju-apply-header">
      <div class="ju-apply-n">3</div>
      <div class="ju-apply-title">Check deadlines early</div>
    </div>
    <div class="ju-apply-body">
      Scholarship and fellowship deadlines may differ from the standard admission calendar. Check the relevant official websites early to confirm eligibility and deadlines.
    </div>
  </div>
</div>

<div class="ju-note">
  <strong><i class="fas fa-envelope" style="color:#2a9d8f; margin-right:7px;"></i>A Note on Enquiries</strong><br>
  I review every application carefully, however due to the high volume of applications, only shortlisted candidates will be contacted. I particularly welcome applications from candidates with a strong research background, a proven track record of publications in reputable journals, and research interests that closely align with the work of BASE Lab. I look forward to hearing from motivated researchers who are eager to contribute to our ongoing research.
</div>

</div>
