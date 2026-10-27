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
  <p style="font-size:1.0em; color:#2a3a4a; line-height:1.82; margin:0 0 12px;"><strong>BASE Lab @ NTU Singapore</strong> welcomes motivated researchers interested in advancing AI-driven solutions for intelligent and sustainable built environments. We offer opportunities for PhD students, postdoctoral researchers, and visiting researchers to pursue impactful research, develop new ideas, and contribute to real-world applications.</p>
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
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 10px;">Open to Singaporeans, Singapore PRs, and international students with a strong background in engineering, computer science, data science, or a related field. Actively recruiting for the <strong>August 2027 intake</strong>.</p>
      <div style="display:grid; grid-template-columns: 1fr 1fr; gap: 12px 36px; margin-top:10px;">

        <div style="border-right: 1px solid #eaecf0; padding-right: 32px; min-width: 0;">
          <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:0 0 6px; text-transform:uppercase; letter-spacing:0.07em;"><i class="fas fa-university" style="color:#2a9d8f; margin-right:5px;"></i>NTU MAE PhD Programme</p>
          <p style="font-size:0.82em; color:#444; margin:0 0 10px; line-height:1.62;">The primary route for PhD admission at NTU. Successful applicants are considered for the <strong>NTU Research Scholarship (RSS)</strong> and <strong>Provost's Graduate Award (PGA)</strong> — covering tuition and a monthly stipend.</p>
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
          <p style="font-size:0.79em; color:#555; margin:0; line-height:1.65;">Before starting this process, please read through the <a href="https://www.ntu.edu.sg/admissions/graduate/radmissionguide?utm" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU Graduate Admission Guidelines</a> carefully to understand the full process, eligibility, and document requirements.</p>
        </div>

        <div style="min-width: 0;">
          <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:0 0 6px; text-transform:uppercase; letter-spacing:0.07em;"><i class="fas fa-award" style="color:#2a9d8f; margin-right:5px;"></i>Other PhD Scholarships</p>
          <p style="font-size:0.79em; color:#666; margin:0 0 10px; line-height:1.55;">The following scholarships require separate applications and may have different deadlines. Please check the <a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU Scholarships portal</a> for current opportunities. If you are interested in any of these scholarships, please email me your CV and indicate your intended scholarship.</p>
          <details class="ju-sub-acc">
            <summary><i class="fas fa-list" style="color:#2a9d8f;"></i> View scholarships <i class="fas fa-chevron-down ju-sub-arrow"></i></summary>
            <div class="ju-sub-acc-body">
              <ul style="margin:6px 0 0; padding-left:16px;">
                <li style="margin-bottom:10px; line-height:1.5;">
                  <a href="https://www.ntu.edu.sg/admissions/graduate/financialmatters/scholarships/npgs" target="_blank" style="color:#2a9d8f;font-weight:600;font-size:0.88em;">Nanyang President's Graduate Scholarship (NPGS)</a>
                  <span style="display:block;font-size:0.85em;color:#444;font-style:normal;margin-top:2px;">Open to all nationalities. Covers full tuition, monthly stipend, and annual conference allowance. Nomination-based by NTU.</span>
                </li>
                <li style="margin-bottom:10px; line-height:1.5;">
                  <a href="https://aisingapore.org/research/phd-fellowship-programme/" target="_blank" style="color:#2a9d8f;font-weight:600;font-size:0.88em;">AISG PhD Fellowship</a>
                  <span style="display:block;font-size:0.85em;color:#444;font-style:normal;margin-top:2px;">Open to all nationalities; SG citizens, PRs and ASEAN applicants especially encouraged. Covers full tuition, monthly stipend, and conference travel support. Focused on AI fundamental research. Nomination-based.</span>
                </li>
                <li style="margin-bottom:10px; line-height:1.5;">
                  <a href="https://www.a-star.edu.sg/scholarships/home/scholarships/ags--scholarship" target="_blank" style="color:#2a9d8f;font-weight:600;font-size:0.88em;">A*STAR Graduate Scholarship (AGS)</a>
                  <span style="display:block;font-size:0.85em;color:#444;font-style:normal;margin-top:2px;">Open to all nationalities. Covers full tuition, monthly stipend, and overseas research attachment support. International applicants commit to 3 years of work in Singapore after graduation.</span>
                </li>
                <li style="margin-bottom:10px; line-height:1.5;">
                  <a href="https://www.psc.gov.sg/scholarships/postgraduate-scholarships/lee-kuan-yew-scholarship" target="_blank" style="color:#2a9d8f;font-weight:600;font-size:0.88em;">Lee Kuan Yew Scholarship</a>
                  <span style="display:block;font-size:0.85em;color:#444;font-style:normal;margin-top:2px;">Singapore citizens only. Covers full tuition and a generous annual allowance for up to 5 years (PhD). Highly competitive with no bond requirement.</span>
                </li>
                <li style="margin-bottom:10px; line-height:1.5;">
                  <a href="https://www.a-star.edu.sg/Scholarships" target="_blank" style="color:#2a9d8f;font-weight:600;font-size:0.88em;">Singapore International Graduate Award (SINGA)</a>
                  <span style="display:block;font-size:0.85em;color:#444;font-style:normal;margin-top:2px;">For international students. Joint A*STAR–NTU PhD programme. Covers full tuition, monthly stipend, and a one-time airfare grant.</span>
                </li>
                <li style="margin-bottom:4px; line-height:1.5;">
                  <a href="https://www.ntu.edu.sg/graduate-college/admissions/scholarships/yunqi-phd-scholarship-in-science-and-technology" target="_blank" style="color:#2a9d8f;font-weight:600;font-size:0.88em;">Yunqi PhD Scholarship in Science &amp; Technology</a>
                  <span style="display:block;font-size:0.85em;color:#444;font-style:normal;margin-top:2px;">Open to all nationalities. Covers full tuition and a monthly stipend for PhD candidates in science and technology at NTU.</span>
                </li>
              </ul>
            </div>
          </details>
          <p style="font-size:0.79em; font-weight:700; color:#0d2244; margin:16px 0 5px; text-transform:uppercase; letter-spacing:0.06em;">Self-Funded &amp; Part-Time PhD</p>
          <p style="font-size:0.79em; color:#666; line-height:1.6; margin:0;">Self-funded applicants are welcome to apply. Part-time PhD study may be available to working professionals, subject to NTU's admission requirements. Please contact me to discuss your circumstances and suitability before applying.</p>
        </div>

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
          <ul style="margin:6px 0 0; padding-left:17px;">
            <li style="font-size:0.86em; color:#444; margin-bottom:8px; line-height:1.6;"><a href="https://www.ntu.edu.sg/research/research-careers" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU Postdoctoral Fellowship</a> — NTU's competitive internal fellowship for researchers within 3 years of their PhD. Covers full salary and a research budget.</li>
            <li style="font-size:0.86em; color:#444; margin-bottom:8px; line-height:1.6;"><a href="https://www.ntu.edu.sg/research/research-careers/lee-kuan-yew-postdoctoral-fellowship-(lkypdf)" target="_blank" style="color:#2a9d8f;font-weight:600;">Lee Kuan Yew Postdoctoral Fellowship</a> — NTU's prestigious fellowship for outstanding early-career researchers. Covers full salary, research allowances, and travel support.</li>
            <li style="font-size:0.86em; color:#444; margin-bottom:8px; line-height:1.6;"><a href="https://www.nrf.gov.sg/grants/nrff/" target="_blank" style="color:#2a9d8f;font-weight:600;">NRF Fellowship (Singapore)</a> — Highly competitive national fellowship supporting early-career researchers in establishing an independent research programme in Singapore. Comes with a substantial 5-year grant.</li>
            <li style="font-size:0.86em; color:#444; margin-bottom:8px; line-height:1.6;"><a href="https://www.a-star.edu.sg/Scholarships" target="_blank" style="color:#2a9d8f;font-weight:600;">A*STAR Research Fellowship Singapore</a> — For Singapore citizens and PRs. Supports postdoctoral research at A*STAR institutes or local universities, with a focus on applied research.</li>
            <li style="font-size:0.86em; color:#444; margin-bottom:8px; line-height:1.6;"><a href="https://marie-sklodowska-curie-actions.ec.europa.eu/" target="_blank" style="color:#2a9d8f;font-weight:600;">Marie Skłodowska-Curie Actions (MSCA)</a> — EU Horizon programme open to researchers of any nationality. Supports international mobility with salary, travel, and research cost allowances.</li>
            <li style="font-size:0.86em; color:#444; margin-bottom:8px; line-height:1.6;"><a href="https://www.humboldt-foundation.de/" target="_blank" style="color:#2a9d8f;font-weight:600;">Alexander von Humboldt Research Fellowship</a> — Internationally recognised fellowship for researchers outside Germany to conduct extended research stays. Open to all career stages and nationalities.</li>
            <li style="font-size:0.86em; color:#444; line-height:1.6;"><a href="https://www.ntu.edu.sg/research/research-careers/ntu-ai-for-x-postdoctoral-fellowship" target="_blank" style="color:#2a9d8f;font-weight:600;">NTU AI-for-X Postdoctoral Fellowship (AI4X)</a> — NTU fellowship for early-career researchers applying AI to diverse domains. Supports independent research with a focus on AI-driven applications.</li>
          </ul>
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
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 0;">NTU MSc and MEng students interested in dissertations or collaborative research in AI, sensing, building systems, or energy are welcome to reach out. Please attach your academic transcript and a short paragraph on your area of interest.</p>
    </div>
  </details>

  <!-- Undergrad -->
  <details class="ju-acc ju-slate">
    <summary><i class="fas fa-user-graduate ju-acc-icon"></i><span class="ju-acc-title">Undergraduate Researchers (NTU)</span><i class="fas fa-chevron-down ju-acc-arrow"></i></summary>
    <div class="ju-acc-body">
      <p style="font-size:0.83em; color:#444; line-height:1.62; margin:12px 0 0;">NTU undergraduates interested in <strong>Final Year Projects (FYP)</strong> or <strong>URECA</strong> research are encouraged to reach out. Please include your transcript and a sentence or two on which research topic interests you most.</p>
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
        <span>A strong background in AI, sensing, sustainable built environments, or energy systems. Prior research experience and thesis work are advantageous for PhD applicants; publications are a plus. Postdoctoral candidates should have a strong publication record and demonstrated ability to lead independent research.</span>
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
        <li style="font-size:0.92em; color:#444; margin-bottom:6px; line-height:1.6;"><strong>Postdoc and RA:</strong> email me directly to discuss your background and fit</li>
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
  I review every application carefully, but due to the high volume of applications only shortlisted candidates will be contacted. I encourage applications that demonstrate a strong research background and a clear alignment with BASE Lab's research interests. I look forward to hearing from motivated researchers who are excited to contribute to our work at BASE Lab.
</div>

</div>
