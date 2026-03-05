<html lang="en"><head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bridging the Gap — Paramedic Informatics Infographic</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&amp;family=DM+Sans:wght@300;400;500;600&amp;family=DM+Mono:wght@400;500&amp;display=swap" rel="stylesheet">
<style>
  :root {
    --navy:    #0F2240;
    --navy2:   #1C3557;
    --teal:    #1A8A9B;
    --teal2:   #24AABF;
    --teal3:   #6DCFDB;
    --amber:   #E8963A;
    --offwhite:#F4F8FB;
    --ltblue:  #D6EBF2;
    --white:   #FFFFFF;
    --grey:    #6B7B8D;
    --text:    #1A2B3C;
  }
  * { margin:0; padding:0; box-sizing:border-box; }
  body { font-family:'DM Sans',sans-serif; background:var(--offwhite); color:var(--text); width:900px; margin:0 auto; padding-top:52px; }


  /* HEADER */
  .header { background:var(--navy); padding:52px 56px 44px; position:relative; overflow:hidden; }
  .header::before { content:''; position:absolute; top:-60px; right:-60px; width:340px; height:340px; border-radius:50%; background:radial-gradient(circle,rgba(26,138,155,.25) 0%,transparent 70%); }
  .header::after  { content:''; position:absolute; bottom:-80px; left:200px; width:500px; height:200px; border-radius:50%; background:radial-gradient(circle,rgba(36,170,191,.12) 0%,transparent 70%); }
  .header-tag { font-family:'DM Mono',monospace; font-size:11px; letter-spacing:3px; color:var(--teal3); text-transform:uppercase; margin-bottom:18px; }
  .header h1  { font-family:'Playfair Display',serif; font-size:52px; font-weight:900; color:var(--white); line-height:1.05; margin-bottom:14px; position:relative; z-index:1; }
  .header h1 span { color:var(--teal2); }
  .header-sub { font-size:16px; font-weight:300; color:rgba(255,255,255,.7); max-width:580px; line-height:1.6; position:relative; z-index:1; }
  .header-pills { display:flex; gap:10px; margin-top:28px; position:relative; z-index:1; flex-wrap:wrap; }
  .pill { background:rgba(26,138,155,.25); border:1px solid rgba(36,170,191,.4); color:var(--teal3); padding:5px 14px; border-radius:20px; font-size:12px; font-weight:500; letter-spacing:.5px; }

  /* LAYOUT */
  .body { padding:0 40px 60px; }

  /* SECTION LABELS */
  .section-label { display:flex; align-items:center; gap:14px; margin:44px 0 20px; }
  .section-num   { font-family:'Playfair Display',serif; font-size:48px; font-weight:900; color:var(--teal); line-height:1; opacity:.35; min-width:36px; }
  .section-title { font-family:'Playfair Display',serif; font-size:22px; font-weight:700; color:var(--navy2); border-bottom:2.5px solid var(--teal); padding-bottom:6px; flex:1; }

  /* PROBLEM */
  .problem-grid { display:grid; grid-template-columns:1fr 1fr; gap:16px; margin-bottom:8px; }
  .problem-card { background:var(--white); border:1px solid #D4E6F0; border-left:4px solid var(--teal); padding:18px 20px; border-radius:0 8px 8px 0; box-shadow:0 2px 12px rgba(15,34,64,.06); }
  .problem-card p { font-size:13.5px; line-height:1.65; color:#2A3D50; }
  .problem-card strong { color:var(--navy2); font-weight:600; }
  .problem-card .hl { color:var(--teal); font-weight:600; }

  /* DUAL HARM */
  .dual-harm { background:var(--navy); border-radius:12px; padding:28px 32px; margin:20px 0; display:grid; grid-template-columns:1fr auto 1fr; align-items:center; gap:20px; }
  .harm-box { text-align:center; padding:20px; border-radius:8px; }
  .harm-box.breach   { background:rgba(192,57,43,.2);  border:1px solid rgba(192,57,43,.4); }
  .harm-box.withhold { background:rgba(232,150,58,.2); border:1px solid rgba(232,150,58,.4); }
  .harm-svg { margin-bottom:10px; display:flex; justify-content:center; }
  .harm-box h3 { font-size:13px; font-weight:700; letter-spacing:1px; text-transform:uppercase; margin-bottom:6px; }
  .harm-box.breach h3   { color:#E87F73; }
  .harm-box.withhold h3 { color:var(--amber); }
  .harm-box p { font-size:12px; color:rgba(255,255,255,.65); line-height:1.5; }
  .harm-vs { font-family:'Playfair Display',serif; font-size:28px; font-weight:900; color:rgba(255,255,255,.2); text-align:center; }
  .dual-harm-label { grid-column:1/-1; text-align:center; font-size:13px; color:rgba(255,255,255,.5); font-style:italic; margin-top:4px; }

  /* EXPANSION PANEL */
  .expansion { background:var(--navy); border-radius:12px; margin:20px 0 8px; overflow:hidden; box-shadow:0 4px 20px rgba(15,34,64,.15); }
  .expansion-trigger { display:flex; align-items:center; justify-content:space-between; padding:20px 28px; cursor:pointer; user-select:none; gap:16px; transition:background 0.2s; }
  .expansion-trigger:hover { background:rgba(36,170,191,.08); }
  .expansion-trigger-left { display:flex; align-items:center; gap:16px; pointer-events:none; }
  .expansion-tag { font-family:'DM Mono',monospace; font-size:10px; letter-spacing:2px; text-transform:uppercase; color:var(--teal3); background:rgba(26,138,155,.25); border:1px solid rgba(36,170,191,.3); padding:3px 10px; border-radius:12px; flex-shrink:0; }
  .expansion-title-static { font-family:'Playfair Display',serif; font-size:17px; font-weight:700; color:var(--white); pointer-events:none; }
  .expansion-chevron { color:var(--teal2); font-size:22px; transition:transform 0.3s; flex-shrink:0; line-height:1; pointer-events:none; }
  .expansion.open .expansion-chevron { transform:rotate(180deg); }
  .expansion-body { display:none; padding:0 28px 28px; border-top:1px solid rgba(36,170,191,.2); }
  .expansion.open .expansion-body { display:block; }
  .exp-intro { font-size:13px; color:rgba(255,255,255,.55); font-style:italic; line-height:1.6; padding:16px 0 20px; }
  .exp-grid { display:grid; grid-template-columns:repeat(3,1fr); gap:14px; }
  .exp-card { background:rgba(255,255,255,.05); border:1px solid rgba(36,170,191,.25); border-top:3px solid var(--teal2); border-radius:8px; padding:18px 16px; }
  .exp-card-num { font-family:'Playfair Display',serif; font-size:32px; font-weight:900; color:var(--teal3); opacity:.35; line-height:1; margin-bottom:4px; }
  .exp-card h4 { font-size:12px; font-weight:700; color:var(--teal2); margin-bottom:10px; text-transform:uppercase; letter-spacing:.5px; }
  .exp-card p  { font-size:12px; color:rgba(255,255,255,.65); line-height:1.6; }
  .exp-card p strong { color:rgba(255,255,255,.9); font-weight:600; }
  .exp-summary { margin-top:18px; padding:16px 20px; background:rgba(26,138,155,.15); border-left:3px solid var(--teal2); border-radius:0 8px 8px 0; }
  .exp-summary p { font-size:13px; color:rgba(255,255,255,.75); line-height:1.65; font-style:italic; }

  /* STATS */
  .stats-row { display:grid; grid-template-columns:repeat(3,1fr); gap:14px; margin:20px 0; }
  .stat-card  { background:var(--white); border:1px solid #D4E6F0; border-radius:10px; padding:20px 18px; text-align:center; box-shadow:0 2px 12px rgba(15,34,64,.05); }
  .stat-num   { font-family:'Playfair Display',serif; font-size:38px; font-weight:900; color:var(--teal); line-height:1; margin-bottom:6px; }
  .stat-num sup { font-size:20px; }
  .stat-label { font-size:12px; color:var(--grey); line-height:1.5; font-weight:500; }
  .stat-cite  { font-size:10.5px; color:#9BAAB8; font-style:italic; margin-top:10px; padding-top:8px; border-top:1px solid #E2EEF4; line-height:1.5; }

  /* INTEROP */
  .interop-def { background:var(--ltblue); border-left:4px solid var(--teal); border-radius:0 10px 10px 0; padding:18px 22px; margin:16px 0 20px; }
  .interop-def p { font-size:13.5px; line-height:1.7; color:var(--navy2); }
  .interop-def em { font-style:italic; }
  .interop-def .cite { font-size:11px; color:var(--grey); margin-top:6px; }

  /* DOMAINS */
  /* FLASHCARDS */
  .flashcard-grid { display:grid; grid-template-columns:repeat(3,1fr); gap:16px; margin:16px 0; }
  .flashcard-wrap { perspective:1000px; height:180px; cursor:pointer; }
  .flashcard-inner {
    position:relative; width:100%; height:100%;
    transform-style:preserve-3d;
    transition:transform 0.55s cubic-bezier(.4,0,.2,1);
  }
  .flashcard-wrap.flipped .flashcard-inner { transform:rotateY(180deg); }
  .flashcard-front, .flashcard-back {
    position:absolute; inset:0;
    backface-visibility:hidden;
    -webkit-backface-visibility:hidden;
    border-radius:12px;
    display:flex; flex-direction:column;
    align-items:center; justify-content:center;
    padding:20px;
    box-shadow:0 4px 16px rgba(15,34,64,.10);
  }
  .flashcard-front {
    background:var(--white);
    border:1px solid #D4E6F0;
    border-top:4px solid var(--teal2);
  }
  .flashcard-front svg { margin-bottom:14px; }
  .flashcard-front h4 {
    font-family:'Playfair Display',serif;
    font-size:20px; font-weight:700;
    color:var(--navy2); text-align:center;
  }
  .flashcard-hint {
    font-size:10px; color:var(--teal3);
    font-family:'DM Mono',monospace;
    letter-spacing:1.5px; text-transform:uppercase;
    margin-top:10px; opacity:0.7;
  }
  .flashcard-back {
    background:var(--teal);
    border:1px solid var(--teal2);
    transform:rotateY(180deg);
  }
  .flashcard-back p {
    font-size:13px; color:white;
    line-height:1.6; text-align:center;
    font-weight:400;
  }
  /* keep old domain-card styles in case referenced elsewhere */
  .domain-card-hd { display:flex; align-items:center; gap:9px; margin-bottom:6px; }
  .domain-card h4 { font-size:13px; font-weight:700; color:var(--navy2); }
  .domain-card p  { font-size:11.5px; color:var(--grey); line-height:1.5; }

  /* HFI TABLE */
  /* HFI FLASHCARDS */
  .hfi-grid-top    { display:grid; grid-template-columns:repeat(4,1fr); gap:16px; margin:16px 0 0; }
  .hfi-grid-bottom { display:grid; grid-template-columns:repeat(3,1fr); gap:16px; margin:0 0 16px; width:75%; }
  .hfi-card-wrap { perspective:1000px; height:190px; cursor:pointer; }
  .hfi-card-inner {
    position:relative; width:100%; height:100%;
    transform-style:preserve-3d;
    transition:transform 0.55s cubic-bezier(.4,0,.2,1);
  }
  .hfi-card-wrap.flipped .hfi-card-inner { transform:rotateY(180deg); }
  .hfi-card-front, .hfi-card-back {
    position:absolute; inset:0;
    backface-visibility:hidden;
    -webkit-backface-visibility:hidden;
    border-radius:12px;
    display:flex; flex-direction:column;
    align-items:center; justify-content:center;
    padding:18px 16px; text-align:center;
    box-shadow:0 4px 16px rgba(15,34,64,.10);
  }
  .hfi-card-front {
    background:var(--navy);
    border:1px solid rgba(36,170,191,.3);
    border-top:4px solid var(--teal2);
  }
  .hfi-card-front svg { margin-bottom:12px; }
  .hfi-card-front h4 {
    font-family:'Playfair Display',serif;
    font-size:19px; font-weight:700;
    color:var(--white);
  }
  .hfi-card-hint {
    font-size:10px; color:var(--teal3);
    font-family:'DM Mono',monospace;
    letter-spacing:1.5px; text-transform:uppercase;
    margin-top:10px; opacity:0.6;
  }
  .hfi-card-back {
    background:var(--teal);
    border:1px solid var(--teal2);
    transform:rotateY(180deg);
  }
  .hfi-card-back p {
    font-size:14px; color:white;
    line-height:1.6; font-weight:500;
    font-style:italic;
  }
  .hfi-td-inner { display:flex; align-items:center; gap:9px; }

  /* PHASES */
  .phases { display:flex; gap:0; margin:16px 0; position:relative; }
  .phases::before { content:''; position:absolute; top:36px; left:36px; right:36px; height:3px; background:linear-gradient(90deg,var(--teal) 0%,var(--teal2) 100%); z-index:0; }
  .phase { flex:1; display:flex; flex-direction:column; align-items:center; text-align:center; padding:0 8px; position:relative; z-index:1; }
  .phase-num { width:52px; height:52px; border-radius:50%; background:var(--teal); display:flex; align-items:center; justify-content:center; font-family:'Playfair Display',serif; font-size:22px; font-weight:900; color:white; margin-bottom:12px; box-shadow:0 0 0 4px var(--offwhite),0 0 0 6px var(--teal3); flex-shrink:0; }
  .phase-card { background:var(--white); border:1px solid #D4E6F0; border-radius:8px; padding:14px 10px; margin-top:10px; width:100%; box-shadow:0 2px 10px rgba(15,34,64,.05); }
  .phase-title { font-size:12px; font-weight:700; color:var(--navy2); margin-bottom:7px; text-transform:uppercase; letter-spacing:.5px; }
  .phase-desc  { font-size:11px; color:var(--grey); line-height:1.55; }

  /* WHY GRID */
  .why-grid { display:grid; grid-template-columns:1fr 1fr; gap:14px; margin:16px 0; }
  .why-card { display:flex; gap:14px; background:var(--white); border:1px solid #D4E6F0; border-radius:10px; padding:16px 18px; box-shadow:0 2px 10px rgba(15,34,64,.05); align-items:flex-start; }
  .why-icon-wrap { width:42px; height:42px; flex-shrink:0; background:var(--ltblue); border-radius:10px; display:flex; align-items:center; justify-content:center; }
  .why-card h4 { font-size:13px; font-weight:700; color:var(--navy2); margin-bottom:5px; }
  .why-card p  { font-size:12px; color:var(--grey); line-height:1.55; }

  /* CLOSING */
  .closing { background:var(--navy); border-radius:12px; margin:28px 0 8px; padding:32px 36px; position:relative; overflow:hidden; }
  .closing::after { content:''; position:absolute; right:-40px; bottom:-40px; width:200px; height:200px; border-radius:50%; background:radial-gradient(circle,rgba(26,138,155,.3) 0%,transparent 70%); }
  .closing-quotes { display:flex; flex-direction:column; gap:16px; margin-bottom:24px; }
  .closing-q { display:flex; gap:14px; align-items:flex-start; }
  .closing-bar { width:3px; flex-shrink:0; background:var(--teal2); border-radius:2px; align-self:stretch; min-height:20px; }
  .closing-q p { font-size:13.5px; color:rgba(255,255,255,.75); font-style:italic; line-height:1.65; }
  .closing-cta { font-family:'Playfair Display',serif; font-size:24px; font-weight:700; color:var(--teal2); position:relative; z-index:1; }

  .divider { height:1px; background:linear-gradient(90deg,transparent,var(--teal3),transparent); margin:8px 0; }
  .footer { text-align:center; padding:18px 0 8px; font-size:11px; color:var(--grey); border-top:1px solid #D4E6F0; line-height:1.8; }
</style>
</head>
<body>


<!-- HEADER -->
<div class="header">
  <div class="header-tag">Executive Master of Health Informatics • 2026 • K. Brianna Wilson </div>
  <h1 spellcheck="true">Bridging <span>the Gap</span></h1>
  <p class="header-sub" spellcheck="true">Paramedics, Health Informatics &amp; the Imperative for Continuity of Care: A bidirectional, patient-following data framework</p>
  <div class="header-pills">
    <span class="pill">Prehospital Care</span>
    <span class="pill">Health Data Interoperability</span>
    <span class="pill">Community Paramedicine</span>
    <span class="pill">HL7 / FHIR</span>
    <span class="pill">Patient-Centred Design</span>
  </div>
</div>

<div class="body">

<!-- 01 THE PROBLEM -->
<div class="section-label">
  <div class="section-num">01</div>
  <div class="section-title" spellcheck="true">The Problem: Paramedics Excluded from the Data Ecosystem</div>
</div>
<div class="problem-grid">
  <div class="problem-card"><p spellcheck="true">Paramedics are the <strong>first clinical contact</strong> in most emergency episodes — yet they arrive on scene with <span class="hl">no access to medical history, medications, allergies, or prior 911 interactions.</span>&nbsp;</p></div>
  <div class="problem-card"><p spellcheck="true">Patients are forced to <strong>retell their story</strong> at every step: dispatch → paramedic → triage → nurse →&nbsp;physician → specialist.&nbsp;</p></div>
  <div class="problem-card"><p spellcheck="true">Health data today is <span class="hl">custodian-centric, not patient-centric.</span> Each organization holds its own version of the patient record.</p></div>
  <div class="problem-card"><p spellcheck="true">The 911 system is <strong>burdened by non-emergent calls</strong> because patients lack primary care access. Without richer information, paramedics have only one option: transport to an ED.</p></div>
</div>

<div class="dual-harm">
  <div class="harm-box breach">
    <div class="harm-svg">
      <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#E87F73" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round">
        <rect x="3" y="11" width="18" height="11" rx="2"></rect>
        <path d="M7 11V7a5 5 0 0 1 9.9-1"></path>
      </svg>
    </div>
    <h3 spellcheck="true">Harm #1 — Breach</h3>
    <p spellcheck="true">Exposing patient data violates privacy and erodes trust in the healthcare system</p>
  </div>
  <div class="harm-vs">vs</div>
  <div class="harm-box withhold">
    <div class="harm-svg">
      <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#E8963A" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round">
        <path d="M17.94 17.94A10.07 10.07 0 0 1 12 20c-7 0-11-8-11-8a18.45 18.45 0 0 1 5.06-5.94"></path>
        <path d="M9.9 4.24A9.12 9.12 0 0 1 12 4c7 0 11 8 11 8a18.5 18.5 0 0 1-2.16 3.19"></path>
        <line x1="1" y1="1" x2="23" y2="23"></line>
      </svg>
    </div>
    <h3 spellcheck="true">Harm #2 — Withhold</h3>
    <p spellcheck="true">Withholding patient data forces providers to make decisions without the information they need</p>
  </div>
  <p class="dual-harm-label" spellcheck="true">Both are serious. The system concentrates on the first while largely tolerating the second. — CPSA, Interoperability Saves Lives (2023)</p>
</div>

<!-- EXPANSION PANEL -->
<div class="expansion" id="data-expansion">
  <div class="expansion-trigger" onclick="this.parentElement.classList.toggle('open')">
    <div class="expansion-trigger-left">
      <span class="expansion-tag">Expand</span>
      <span class="expansion-title-static">What Data Access Makes Possible: Beyond the Emergency Department</span>
    </div>
    <span class="expansion-chevron">⌄</span>
  </div>
  <div class="expansion-body">
    <p class="exp-intro" spellcheck="true">Data gives paramedics the tools to change the healthcare system in three concrete directions.</p>
    <div class="exp-grid">
      <div class="exp-card">
        <div class="exp-card-num">01</div>
        <h4 spellcheck="true">Smart Destination Routing</h4>
        <p spellcheck="true">A paramedic who can access data turns a default transport into an informed clinical decision.<div><br></div><div>- geriatric patients</div><div>- cardiac patients</div><div>- mental health patients</div><div>- dialysis patients</div></p>
      </div>
      <div class="exp-card">
        <div class="exp-card-num">02</div>
        <h4 spellcheck="true">Care Coaching &amp; Pathway Redirection</h4>
        <p spellcheck="true">For low-acuity calls, a paramedic with access to a patient’s record and a <strong>telehealth or primary care link</strong> can redirect the patient toward the right pathway rather than defaulting to transport.&nbsp;</p>
      </div>
      <div class="exp-card">
        <div class="exp-card-num">03</div>
        <h4 spellcheck="true">Direct Reporting to Primary Care</h4>
        <p spellcheck="true">When a paramedic responds to a call, the patient’s family physician almost never finds out. A <strong>structured prehospital encounter report</strong> sent automatically to the primary care provider creates a longitudinal picture between physician visits and enables <strong>proactive case management</strong> for frequent callers.</p>
      </div>
    </div>
    <div class="exp-summary">
      <p spellcheck="true">Together, these three capabilities reframe the paramedic as an intelligent first point of contact in a connected care system while unburdening the ED.</p>
    </div>
  </div>
</div>

<!-- 02 THE SCALE -->
<div class="section-label">
  <div class="section-num">02</div>
  <div class="section-title" spellcheck="true">The Scale: Why This Matters Now</div>
</div>
<div class="stats-row">
  <div class="stat-card">
    <div class="stat-num" spellcheck="true">5.1<sup>M</sup></div>
    <div class="stat-label" spellcheck="true">Annual 911 EMS calls in Canada — every one initiated without paramedic EHR access</div>
    <div class="stat-cite" spellcheck="true">Canadian Institute for Health Information (CIHI). <em>Emergency and Ambulatory Care.</em> Ottawa: CIHI, 2023.</div>
  </div>
  <div class="stat-card">
    <div class="stat-num" spellcheck="true">$10<sup>B+</sup></div>
    <div class="stat-label" spellcheck="true">Estimated annual cost of poor health data interoperability in Canada</div>
    <div class="stat-cite" spellcheck="true">Wealth of Information: Health Data Economics. CIHI, 2025.</div>
  </div>
  <div class="stat-card">
    <div class="stat-num" spellcheck="true">15–30<sup>%</sup></div>
    <div class="stat-label" spellcheck="true">Of ED visits estimated as avoidable with better prehospital triage and information access</div>
    <div class="stat-cite" spellcheck="true">Canadian Institute for Health Information. <em>How Canada Compares: Results From the Commonwealth Fund’s 2023 International Health Policy Survey.</em> Ottawa: CIHI, 2023.</div>
  </div>
</div>

<!-- 03 WHAT HAS BEEN TRIED -->
<div class="section-label">
  <div class="section-num">03</div>
  <div class="section-title">What Has Been Tried </div>
</div>
<p style="font-size:13px;color:var(--grey);margin-bottom:18px;font-style:italic;padding-left:4px;">This problem has been recognized for decades. What approaches exist? </p>

<div style="display:grid;grid-template-columns:1fr 1fr;gap:14px;margin-bottom:14px;">

  <!-- Canada -->
  <div style="background:var(--white);border:1px solid #D4E6F0;border-radius:10px;overflow:hidden;box-shadow:0 2px 12px rgba(15,34,64,.06);">
    <div style="background:var(--navy);padding:14px 18px;display:flex;align-items:center;gap:12px;">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="3" width="20" height="14" rx="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg>
      <div>
        <div style="font-family:'DM Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--teal3);margin-bottom:2px;">Canada</div>
        <div style="font-family:'Playfair Display',serif;font-size:16px;font-weight:700;color:white;">ePCR Systems</div>
      </div>
      <div style="margin-left:auto;background:rgba(232,127,115,.2);border:1px solid rgba(232,127,115,.4);border-radius:20px;padding:3px 10px;font-size:10px;font-weight:700;color:#E87F73;font-family:'DM Mono',monospace;letter-spacing:1px;">PARTIAL</div>
    </div>
    <div style="padding:14px 18px;">
      <p style="font-size:12px;color:#2A3D50;line-height:1.65;margin-bottom:10px;">Canadian paramedic services have adopted ePCR systems that digitize prehospital documentation. The information gets captured but it does not travel with the patient. - Built as <strong>closed, proprietary systems with no interoperability requirements.</strong></p>
      <div style="background:var(--offwhite);border-left:3px solid var(--teal);border-radius:0 6px 6px 0;padding:10px 13px;">
        <p style="font-size:11.5px;color:var(--grey);line-height:1.6;font-style:italic;">In Burnaby, the hospital has a connected system that pulls call records by ambulance unit number. Unreliable. The connection exists — it just stops at the jurisdictional boundary.</p>
      </div>
    </div>
  </div>

  <!-- UK -->
  <div style="background:var(--white);border:1px solid #D4E6F0;border-radius:10px;overflow:hidden;box-shadow:0 2px 12px rgba(15,34,64,.06);">
    <div style="background:var(--navy);padding:14px 18px;display:flex;align-items:center;gap:12px;">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/></svg>
      <div>
        <div style="font-family:'DM Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--teal3);margin-bottom:2px;">United Kingdom</div>
        <div style="font-family:'Playfair Display',serif;font-size:16px;font-weight:700;color:white;">NHS Summary Care Record</div>
      </div>
      <div style="margin-left:auto;background:rgba(232,150,58,.2);border:1px solid rgba(232,150,58,.4);border-radius:20px;padding:3px 10px;font-size:10px;font-weight:700;color:var(--amber);font-family:'DM Mono',monospace;letter-spacing:1px;">CLOSER</div>
    </div>
    <div style="padding:14px 18px;">
      <p style="font-size:12px;color:#2A3D50;line-height:1.65;">NHS paramedics have <strong>read-only access to patient Summary Care Records</strong> </p>
      <p style="font-size:12px;color:#2A3D50;line-height:1.65;margin-top:8px;">But the model is <strong>unidirectional</strong> — paramedics can read, but cannot contribute back to the record in real time. </p>
    </div>
  </div>

  <!-- Singapore -->
  <div style="background:var(--white);border:1px solid #D4E6F0;border-radius:10px;overflow:hidden;box-shadow:0 2px 12px rgba(15,34,64,.06);grid-column:1/-1;">
    <div style="background:var(--teal);padding:14px 18px;display:flex;align-items:center;gap:12px;">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
      <div>
        <div style="font-family:'DM Mono',monospace;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:rgba(255,255,255,.7);margin-bottom:2px;">Singapore</div>
        <div style="font-family:'Playfair Display',serif;font-size:16px;font-weight:700;color:white;">OMNII — The Proof of Concept</div>
      </div>
      <div style="margin-left:auto;background:rgba(255,255,255,.2);border:1px solid rgba(255,255,255,.4);border-radius:20px;padding:3px 10px;font-size:10px;font-weight:700;color:white;font-family:'DM Mono',monospace;letter-spacing:1px;">LIVE</div>
    </div>
    <div style="padding:14px 18px;display:grid;grid-template-columns:1fr 1fr 1fr;gap:12px;">
      <div style="background:var(--offwhite);border-radius:8px;padding:12px 14px;border-top:3px solid var(--teal2);">
        <div style="font-size:11px;font-weight:700;color:var(--navy2);margin-bottom:5px;">Built With Frontline Clinicians</div>
        <div style="font-size:11px;color:var(--grey);line-height:1.6;">Developed collaboratively with SCDF paramedics, MOH physicians, and ED nurses — co-designed from the start.</div>
      </div>
      <div style="background:var(--offwhite);border-radius:8px;padding:12px 14px;border-top:3px solid var(--teal2);">
        <div style="font-size:11px;font-weight:700;color:var(--navy2);margin-bottom:5px;">Real-Time Patient Record Access</div>
        <div style="font-size:11px;color:var(--grey);line-height:1.6;">Paramedics retrieve full patient health records en route to the hospital — before they arrive on scene.</div>
      </div>
      <div style="background:var(--offwhite);border-radius:8px;padding:12px 14px;border-top:3px solid var(--teal2);">
        <div style="font-size:11px;font-weight:700;color:var(--navy2);margin-bottom:5px;">Live Vitals Streamed to ED</div>
        <div style="font-size:11px;color:var(--grey);line-height:1.6;">Vital signs transmit directly to the receiving emergency department before the patient arrives.</div>
      </div>
    </div>
    <div style="padding:0 18px 14px;">
      <div style="background:var(--navy);border-radius:8px;padding:12px 16px;">
        <p style="font-size:12px;color:rgba(255,255,255,.8);line-height:1.65;font-style:italic;">Canada is not waiting on technology. OMNII proves the vision is operational. What is missing is the governance decision to build it here.</p>
      </div>
    </div>
  </div>

</div>

<!-- 04 SOLUTION -->
<div class="section-label">
  <div class="section-num">04</div>
  <div class="section-title" spellcheck="true">Proposed Solution: A Bidirectional, Patient-Following Data Framework</div>
</div>
<p style="font-size:13px;color:var(--grey);margin-bottom:22px;font-style:italic;padding-left:4px;">Data must flow with the patient from the moment a 911 call is initiated — and feedback must flow back to paramedics after care is complete.</p>
<div class="phases">
  <div class="phase"><div class="phase-num">1</div><div class="phase-card"><div class="phase-title" spellcheck="true">Dispatch</div><div class="phase-desc" spellcheck="true">Patient record opened at first 911 call. History, meds &amp; allergies populated before paramedics arrive on scene.</div></div></div>
  <div class="phase"><div class="phase-num">2</div><div class="phase-card"><div class="phase-title" spellcheck="true">Prehospital</div><div class="phase-desc" spellcheck="true">Paramedics access the full record in real time. Vitals, assessments &amp; treatment added and transmitted live.</div></div></div>
  <div class="phase"><div class="phase-num">3</div><div class="phase-card"><div class="phase-title" spellcheck="true">Smart Routing</div><div class="phase-desc" spellcheck="true">Enriched data enables direct transport to the right unit — psych, cardiac, geriatric — bypassing unnecessary ED processing.</div></div></div>
  <div class="phase"><div class="phase-num">4</div><div class="phase-card"><div class="phase-title" spellcheck="true">Handoff</div><div class="phase-desc" spellcheck="true">Receiving team is fully briefed before arrival. Seamless handover replaces the repeated retelling of the patient story.</div></div></div>
  <div class="phase"><div class="phase-num">5</div><div class="phase-card"><div class="phase-title" spellcheck="true">Outcome Loop</div><div class="phase-desc" spellcheck="true">Post-discharge summary returned to paramedics. Diagnoses &amp; outcomes close the loop and fuel clinical learning.</div></div></div>
</div>

<!-- 05 WHY IT WORKS -->
<div class="section-label">
  <div class="section-num">05</div>
  <div class="section-title" spellcheck="true">Why It Will Work</div>
</div>
<div class="why-grid">
  <div class="why-card">
    <div class="why-icon-wrap"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1"></rect><line x1="9" y1="12" x2="15" y2="12"></line><line x1="9" y1="16" x2="13" y2="16"></line></svg></div>
    <div><h4 spellcheck="true">Evidence Base</h4><p spellcheck="true">Community paramedicine with integrated data access shows improved outcomes, reduced ED use, and higher patient satisfaction (Bigham et al., 2013; Dainty et al., 2018).</p></div>
  </div>
  <div class="why-card">
    <div class="why-icon-wrap"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M17.8 19.2L16 11l3.5-3.5C21 6 21 4 19 4c-1 0-2 1-3.5 2.5L9 11 2.8 9.2c-.6-.2-.6-1 0-1.2L21 3l-2 18c-.2.6-1 .6-1.2 0z"></path></svg></div>
    <div><h4 spellcheck="true">Aviation</h4><p spellcheck="true">Aviation coordinates thousands of aircraft globally via a single interoperable standard, mandated by governance, not technology. Healthcare can do the same.</p></div>
  </div>
  <div class="why-card">
    <div class="why-icon-wrap"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="1" y="4" width="22" height="16" rx="2"></rect><line x1="1" y1="10" x2="23" y2="10"></line></svg></div>
    <div><h4 spellcheck="true">Banking</h4><p spellcheck="true">Your debit card works at any ATM worldwide through technical standards + regulatory mandates. Patient data can follow patients the same way.</p></div>
  </div>
  <div class="why-card">
    <div class="why-icon-wrap"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><polyline points="17 1 21 5 17 9"></polyline><path d="M3 11V9a4 4 0 0 1 4-4h14"></path><polyline points="7 23 3 19 7 15"></polyline><path d="M21 13v2a4 4 0 0 1-4 4H3"></path></svg></div>
    <div><h4 spellcheck="true">Bidirectional Learning</h4><p spellcheck="true">When paramedics receive outcome feedback — diagnoses, treatments, discharge — their clinical knowledge grows. Closing the loop elevates the entire profession.</p></div>
  </div>
  <div class="why-card">
    <div class="why-icon-wrap"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><line x1="3" y1="22" x2="21" y2="22"></line><line x1="6" y1="18" x2="6" y2="11"></line><line x1="10" y1="18" x2="10" y2="11"></line><line x1="14" y1="18" x2="14" y2="11"></line><line x1="18" y1="18" x2="18" y2="11"></line><polygon points="12 2 20 7 4 7"></polygon></svg></div>
    <div><h4 spellcheck="true">Governance-First Design</h4><p spellcheck="true">Prior efforts failed by deploying technology into fragmented governance. This framework builds policy and legislative alignment before any procurement.</p></div>
  </div>
  <div class="why-card">
    <div class="why-icon-wrap"><svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"></path></svg></div>
    <div><h4 spellcheck="true">The Moral Imperative</h4><p spellcheck="true">Withholding clinical data from frontline providers is an active, preventable harm. As stewards of health data, we are obligated to act.</p></div>
  </div>
</div>

<div class="divider"></div>

<!-- CLOSING -->
<div class="closing">
  <div class="closing-quotes">
    <div class="closing-q"><div class="closing-bar"></div><p spellcheck="true">Paramedics are the first clinical touch in a patient’s care journey — yet the last to have access to their information.</p></div>
    <div class="closing-q"><div class="closing-bar"></div><p spellcheck="true">A healthcare system that withholds data from its frontline providers is a system that accepts preventable harm.</p></div>
    <div class="closing-q"><div class="closing-bar"></div><p spellcheck="true">The system is changing. Paramedics must not be consulted at the end; they must be at the table from the beginning.</p></div>
  </div>
  <div class="closing-cta" spellcheck="true">A robust Canadian health data ecosystem includes Paramedics.</div>
</div>

</div>

<div class="footer">
  <div style="text-align:left; max-width:820px; margin:0 auto; padding:20px 0 12px;">
    <p style="font-size:12px; font-weight:700; color:var(--navy2); text-transform:uppercase; letter-spacing:1.5px; margin-bottom:14px;">References</p>
    <ol style="font-size:11px; color:var(--grey); line-height:1.9; padding-left:18px;">
      <li>1 in 7 visits to the emergency department are for conditions that could potentially have been managed in primary care | CIHI. Accessed March 2, 2026. <a href="https://www.cihi.ca/en/news/1-in-7-visits-to-the-emergency-department-are-for-conditions-that-could-potentially-have-been" style="color:var(--teal);">cihi.ca</a></li>
      <li>Kuo MH, Kushniruk A, Borycki E. A Comparison of National Health Data Interoperability Approaches in Taiwan, Denmark and Canada.</li>
      <li>Dainty KN, Seaton MB, Drennan IR, Morrison LJ. Home Visit-Based Community Paramedicine and Its Potential Role in Improving Patient-Centered Primary Care: A Grounded Theory Study and Framework. Health Serv Res. 2018;53(5):3455-3470. doi:10.1111/1475-6773.12855.</li>
      <li>Brend Y. Canada's health-care system has a data problem, experts say. And it puts patients at risk. <em>CBC News.</em> November 17, 2022. Accessed March 1, 2026. <a href="https://www.cbc.ca/news/canada/health-data-canada-sharing-information-1.6652770" style="color:var(--teal);">cbc.ca</a></li>
      <li>Continuity of Patient Care. Health Quality Alberta. Accessed March 2, 2026. <a href="https://hqa.ca/reports/continuity-of-patient-care-2/" style="color:var(--teal);">hqa.ca</a></li>
      <li>Digital Health Information Exchange | Ontario Health. Accessed March 1, 2026. <a href="https://www.ontariohealth.ca/digital/standards/info-exchange" style="color:var(--teal);">ontariohealth.ca</a></li>
      <li>Bigham BL, Kennedy SM, Drennan I, Morrison LJ. Expanding Paramedic Scope of Practice in the Community: A Systematic Review of the Literature. <em>Prehospital Emergency Care.</em> 2013;17(3):361-372. doi:10.3109/10903127.2013.792890</li>
      <li>Monico L. HL7 FHIR. Canada Health Infoway. Accessed March 1, 2026. <a href="https://infocentral.infoway-inforoute.ca/en/standards/canadian/fhir" style="color:var(--teal);">infocentral.infoway-inforoute.ca</a></li>
      <li>New digital platform for paramedics and hospitals to share patient data in real time. <em>CNA.</em> Accessed March 2, 2026. <a href="https://www.channelnewsasia.com/singapore/digital-platform-scdf-moh-hospitals-patients-omnii-2132121" style="color:var(--teal);">channelnewsasia.com</a></li>
      <li>Pan-Canadian Health Data Charter. October 12, 2023. Accessed March 1, 2026. <a href="https://www.canada.ca/en/health-canada/corporate/transparency/health-agreements/shared-health-priorities/working-together-bilateral-agreements/pan-canadian-data-charter.html" style="color:var(--teal);">canada.ca</a></li>
      <li>Allana A, Pinto AD. Paramedics Have Untapped Potential to Address Social Determinants of Health in Canada. <em>Healthc Policy.</em> 2021;16(3):67-75. doi:10.12927/hcpol.2021.26432</li>
      <li>Booker MJ, Simmonds RL, Purdy S. Patients who call emergency ambulances for primary care problems: a qualitative study of the decision-making process. <em>Emerg Med J.</em> 2014;31(6):448-452. doi:10.1136/emermed-2012-202124</li>
      <li>Lau F, Partridge C, Hauser M. A pan-Canadian health informatics education strategy. AMIA Annu Symp Proc. 2003;2003:386-390. https://pmc.ncbi.nlm.nih.gov/articles/PMC1480046/</li>
<li>Rees G, Nowell L, Risling T. Shaping the future of digital health education in Canada: prioritizing competencies for health care professionals using the Quintuple Aim. JMIR Med Educ. 2025;11:e75904. doi:10.2196/75904</li>
      <li>Benny G. Provider-centric models of care in which most consumers of healthcare are passive. <em>Internal Medicine Journal.</em> 2015;45(8):795-797. doi:10.1111/imj.12828</li>
      <li>Wealth of Information: Health Data Economics | CIHI. Accessed March 1, 2026. <a href="https://www.cihi.ca/en/wealth-of-information-health-data-economics" style="color:var(--teal);">cihi.ca</a></li>
    </ol>
    <p style="text-align:center; margin-top:18px; padding-top:14px; border-top:1px solid #D4E6F0; font-size:11px; color:var(--grey);">University of Toronto Executive Master of Health Informatics &nbsp;&middot;&nbsp; 2026 &nbsp;&middot;&nbsp; K. Brianna Wilson </p>
  </div>
</div>
<br>
<br>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Infrastructure Framework — Paramedic Informatics</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --navy:    #0F2240;
    --navy2:   #1C3557;
    --teal:    #1A8A9B;
    --teal2:   #24AABF;
    --teal3:   #6DCFDB;
    --amber:   #E8963A;
    --offwhite:#F4F8FB;
    --ltblue:  #D6EBF2;
    --white:   #FFFFFF;
    --grey:    #6B7B8D;
  }
  * { margin:0; padding:0; box-sizing:border-box; }
  body { font-family:'DM Sans',sans-serif; background:var(--offwhite); color:#1A2B3C; width:900px; margin:0 auto; padding:40px; }

  /* HEADER */
  .header {
    background:var(--navy); border-radius:14px;
    padding:36px 44px 32px; margin-bottom:28px;
    position:relative; overflow:hidden;
  }
  .header::before { content:''; position:absolute; top:-60px; right:-60px; width:300px; height:300px; border-radius:50%; background:radial-gradient(circle,rgba(26,138,155,.3) 0%,transparent 70%); }
  .header-tag { font-family:'DM Mono',monospace; font-size:10px; letter-spacing:3px; color:var(--teal3); text-transform:uppercase; margin-bottom:12px; }
  .header h1 { font-family:'Playfair Display',serif; font-size:38px; font-weight:900; color:var(--white); line-height:1.1; margin-bottom:10px; position:relative; z-index:1; }
  .header h1 span { color:var(--teal2); }
  .header-sub { font-size:13px; color:rgba(255,255,255,.6); line-height:1.6; position:relative; z-index:1; max-width:520px; }

  /* SEQUENCE BANNER */
  .seq-banner {
    background:var(--ltblue); border:1px solid rgba(26,138,155,.3);
    border-left:4px solid var(--teal2);
    border-radius:0 10px 10px 0;
    padding:14px 20px; margin-bottom:24px;
    font-size:13px; color:var(--navy2); line-height:1.6;
  }
  .seq-banner strong { color:var(--teal); }

  /* QUADRANT GRID */
  .quad-grid { display:grid; grid-template-columns:1fr 1fr; gap:16px; margin-bottom:24px; }

  .quad {
    background:var(--white);
    border:1px solid #D4E6F0;
    border-radius:12px;
    overflow:hidden;
    box-shadow:0 4px 18px rgba(15,34,64,.07);
  }

  /* Quad header */
  .quad-header {
    padding:18px 22px 14px;
    display:flex; align-items:center; gap:14px;
    border-bottom:1px solid #E8F4F8;
  }
  .quad-icon-wrap {
    width:46px; height:46px; border-radius:12px;
    display:flex; align-items:center; justify-content:center;
    flex-shrink:0;
  }
  .quad-header-text {}
  .quad-order {
    font-family:'DM Mono',monospace;
    font-size:9px; letter-spacing:2px; text-transform:uppercase;
    margin-bottom:2px;
  }
  .quad-title {
    font-family:'Playfair Display',serif;
    font-size:18px; font-weight:700; color:var(--navy2);
  }

  /* Colour theming per quadrant */
  .quad.people .quad-header  { background:#F0FAFB; }
  .quad.people .quad-icon-wrap { background:rgba(26,138,155,.12); }
  .quad.people .quad-order   { color:var(--teal); }
  .quad.people .quad-title   { color:#0F4D5A; }

  .quad.process .quad-header { background:#FFF8EE; }
  .quad.process .quad-icon-wrap { background:rgba(232,150,58,.12); }
  .quad.process .quad-order  { color:var(--amber); }
  .quad.process .quad-title  { color:#6B3B00; }

  .quad.tech .quad-header    { background:#EEF2FF; }
  .quad.tech .quad-icon-wrap { background:rgba(99,102,241,.12); }
  .quad.tech .quad-order     { color:#6366F1; }
  .quad.tech .quad-title     { color:#2D2F7A; }

  .quad.org .quad-header     { background:#F3F0FF; }
  .quad.org .quad-icon-wrap  { background:rgba(139,92,246,.12); }
  .quad.org .quad-order      { color:#8B5CF6; }
  .quad.org .quad-title      { color:#3B1F6B; }

  /* Quad body */
  .quad-body { padding:16px 22px 20px; }

  .quad-item {
    display:flex; gap:10px; align-items:flex-start;
    padding:9px 0;
    border-bottom:1px solid #F0F5F8;
  }
  .quad-item:last-child { border-bottom:none; padding-bottom:0; }

  .quad-dot {
    width:7px; height:7px; border-radius:50%;
    flex-shrink:0; margin-top:6px;
  }
  .quad.people  .quad-dot { background:var(--teal2); }
  .quad.process .quad-dot { background:var(--amber); }
  .quad.tech    .quad-dot { background:#6366F1; }
  .quad.org     .quad-dot { background:#8B5CF6; }

  .quad-item-content {}
  .quad-item-label {
    font-size:12px; font-weight:700; color:var(--navy2);
    margin-bottom:2px;
  }
  .quad-item-desc {
    font-size:11.5px; color:var(--grey); line-height:1.55;
  }

  /* BOTTOM CALLOUT */
  .callout {
    background:var(--navy); border-radius:12px;
    padding:24px 32px;
    display:grid; grid-template-columns:1fr auto;
    align-items:center; gap:24px;
  }
  .callout-text {}
  .callout-label {
    font-family:'DM Mono',monospace; font-size:9px;
    letter-spacing:2.5px; text-transform:uppercase;
    color:var(--teal3); margin-bottom:8px;
  }
  .callout-quote {
    font-family:'Playfair Display',serif;
    font-size:17px; font-weight:700; color:var(--white);
    line-height:1.45;
  }
  .callout-quote span { color:var(--teal2); }
  .seq-pills { display:flex; flex-direction:column; gap:8px; }
  .seq-pill {
    display:flex; align-items:center; gap:8px;
    background:rgba(255,255,255,.06);
    border:1px solid rgba(36,170,191,.2);
    border-radius:8px; padding:6px 14px;
    white-space:nowrap;
  }
  .seq-pill-num {
    font-family:'DM Mono',monospace;
    font-size:11px; font-weight:600;
    color:var(--teal3);
  }
  .seq-pill-name {
    font-size:11px; font-weight:600; color:rgba(255,255,255,.7);
  }

  /* FOOTER */
  .footer {
    text-align:center; margin-top:20px;
    font-size:10.5px; color:var(--grey);
    border-top:1px solid #D4E6F0; padding-top:14px;
  }
</style>
</head>
<body>

<!-- HEADER -->
<div class="header">
  <div class="header-tag">U of T EMHI &bull; 2026</div>
  <h1>Infrastructure for <span>System Change</span></h1>
  <p class="header-sub">Four categories of infrastructure</p>
</div>

<!-- FOUR QUADRANTS -->
<div class="quad-grid">

  <!-- PEOPLE -->
  <div class="quad people">
    <div class="quad-header">
      <div class="quad-icon-wrap">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
      </div>
      <div class="quad-header-text">
        <div class="quad-order">01 &mdash; First</div>
        <div class="quad-title">People</div>
      </div>
    </div>
    <div class="quad-body">
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Clinical Informaticist</div>
          <div class="quad-item-desc">Bridge between prehospital care and health IT </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Health IT Project Manager</div>
          <div class="quad-item-desc">Someone who has navigated data sharing agreements</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Change Management Lead</div>
          <div class="quad-item-desc">Understands frontline clinical culture </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Data Analyst / Biostatistician</div>
          <div class="quad-item-desc">Designs outcome measurement and produces publishable, policy-relevant evidence</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Privacy &amp; Legal Advisor (Embedded)</div>
          <div class="quad-item-desc">Working to enable sharing </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Frontline Paramedics (Co-designers)</div>
          <div class="quad-item-desc">Compensated, involved throughout — their operational knowledge is irreplaceable</div>
        </div>
      </div>
    </div>
  </div>

  <!-- PROCESS -->
  <div class="quad process">
    <div class="quad-header">
      <div class="quad-icon-wrap">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#E8963A" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><polyline points="9 11 12 14 22 4"/><path d="M21 12v7a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11"/></svg>
      </div>
      <div class="quad-header-text">
        <div class="quad-order">02 &mdash; Second</div>
        <div class="quad-title">Process</div>
      </div>
    </div>
    <div class="quad-body">
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Data Sharing Agreement</div>
          <div class="quad-item-desc">Legally reviewed, signed by EMS and hospital partners</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Privacy Impact Assessment</div>
          <div class="quad-item-desc">Completed and on file before a single patient record is accessed</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Clinical Workflow Design</div>
          <div class="quad-item-desc">Paramedics and ED staff co-define how and when data is accessed</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Structured Training Program</div>
          <div class="quad-item-desc">Not just how to use the platform — why the information matters clinically</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Joint QI Committee</div>
          <div class="quad-item-desc">Paramedic and hospital representation — meets regularly to identify and solve problems early</div>
        </div>
      </div>
    </div>
  </div>

  <!-- TECHNOLOGY -->
  <div class="quad tech">
    <div class="quad-header">
      <div class="quad-icon-wrap">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#6366F1" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="3" width="20" height="14" rx="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg>
      </div>
      <div class="quad-header-text">
        <div class="quad-order">03 &mdash; Third</div>
        <div class="quad-title">Technology</div>
      </div>
    </div>
    <div class="quad-body">
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">HL7 FHIR-Compliant ePCR Platform</div>
          <div class="quad-item-desc">Several exist in the Canadian market — selected for FHIR compliance </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">API Connection to Provincial EHR / Hospital EMR</div>
          <div class="quad-item-desc">Built on FHIR R4 — technically straightforward </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Medical Device Integration</div>
          <div class="quad-item-desc">Vital signs and ECG data captured automatically </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Role-Based Access Control</div>
          <div class="quad-item-desc">Paramedics see what they need, access is logged, audit trail satisfies privacy requirements</div>
        </div>
      </div>
    </div>
  </div>

  <!-- ORGANIZATIONAL -->
  <div class="quad org">
    <div class="quad-header">
      <div class="quad-icon-wrap">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#8B5CF6" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><line x1="3" y1="22" x2="21" y2="22"/><line x1="6" y1="18" x2="6" y2="11"/><line x1="10" y1="18" x2="10" y2="11"/><line x1="14" y1="18" x2="14" y2="11"/><line x1="18" y1="18" x2="18" y2="11"/><polygon points="12 2 20 7 4 7"/></svg>
      </div>
      <div class="quad-header-text">
        <div class="quad-order">04 &mdash; Fourth</div>
        <div class="quad-title">Organizational</div>
      </div>
    </div>
    <div class="quad-body">
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Joint Governance Committee</div>
          <div class="quad-item-desc">Paramedic, hospital, and health authority decision-making authority</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Executive Sponsorship (Both Sides)</div>
          <div class="quad-item-desc">Paramedic and hospital leadership — willing to remove barriers</div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Escalation Path for Data Disputes</div>
          <div class="quad-item-desc">A defined process when a privacy officer says no </div>
        </div>
      </div>
      <div class="quad-item">
        <div class="quad-dot"></div>
        <div class="quad-item-content">
          <div class="quad-item-label">Sustainability Plan</div>
          <div class="quad-item-desc">Pathway to operational funding before the pilot ends </div>
        </div>
      </div>
    </div>
  </div>

</div>

<!-- 06 INTEROPERABILITY -->
<div class="section-label">
  <div class="section-num">06</div>
  <div class="section-title" spellcheck="true">Health Data Interoperability: The Foundation</div>
</div>
<div class="interop-def">
  <p spellcheck="true"><em>“The ability of different information systems, devices and applications to access, exchange, integrate and cooperatively use data in a coordinated manner to optimize the health of individuals and populations.”</em></p>
  <p class="cite" spellcheck="true">— CPSA, Interoperability Saves Lives (2023) &nbsp;·&nbsp; </p>
</div>
<div class="flashcard-grid">

  <div class="flashcard-wrap" onclick="this.classList.toggle('flipped')">
    <div class="flashcard-inner">
      <div class="flashcard-front">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>
        <h4 spellcheck="true">Safe</h4>
        <span class="flashcard-hint">tap to reveal</span>
      </div>
      <div class="flashcard-back">
        <p spellcheck="true">Reduces adverse events caused by missing or inaccurate patient data at point of care</p>
      </div>
    </div>
  </div>

  <div class="flashcard-wrap" onclick="this.classList.toggle('flipped')">
    <div class="flashcard-inner">
      <div class="flashcard-front">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>
        <h4 spellcheck="true">Effective</h4>
        <span class="flashcard-hint">tap to reveal</span>
      </div>
      <div class="flashcard-back">
        <p spellcheck="true">Enables evidence-based decisions informed by a complete patient medical history</p>
      </div>
    </div>
  </div>

  <div class="flashcard-wrap" onclick="this.classList.toggle('flipped')">
    <div class="flashcard-inner">
      <div class="flashcard-front">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon></svg>
        <h4 spellcheck="true">Efficient</h4>
        <span class="flashcard-hint">tap to reveal</span>
      </div>
      <div class="flashcard-back">
        <p spellcheck="true">Eliminates redundant testing, documentation, and the repeated retelling of stories</p>
      </div>
    </div>
  </div>

  <div class="flashcard-wrap" onclick="this.classList.toggle('flipped')">
    <div class="flashcard-inner">
      <div class="flashcard-front">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><line x1="2" y1="12" x2="22" y2="12"></line><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path></svg>
        <h4 spellcheck="true">Equitable</h4>
        <span class="flashcard-hint">tap to reveal</span>
      </div>
      <div class="flashcard-back">
        <p spellcheck="true">Ensures equal information access for all providers — including prehospital teams</p>
      </div>
    </div>
  </div>

  <div class="flashcard-wrap" onclick="this.classList.toggle('flipped')">
    <div class="flashcard-inner">
      <div class="flashcard-front">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><polyline points="12 6 12 12 16 14"></polyline></svg>
        <h4 spellcheck="true">Timely</h4>
        <span class="flashcard-hint">tap to reveal</span>
      </div>
      <div class="flashcard-back">
        <p spellcheck="true">Faster interventions, smarter triage routing, and direct-to-unit transport decisions</p>
      </div>
    </div>
  </div>

  <div class="flashcard-wrap" onclick="this.classList.toggle('flipped')">
    <div class="flashcard-inner">
      <div class="flashcard-front">
        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#1A8A9B" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
        <h4 spellcheck="true">Person-Centred</h4>
        <span class="flashcard-hint">tap to reveal</span>
      </div>
      <div class="flashcard-back">
        <p spellcheck="true">Data follows the patient — not the institution, not the custodian</p>
      </div>
    </div>
  </div>

</div>

<!--07 HUMAN FACTOR -->
<div class="section-label">
  <div class="section-num">07</div>
  <div class="section-title" spellcheck="true">Human Factor Interoperability: The Prerequisite</div>
</div>
<p style="font-size:13px;color:var(--grey);margin-bottom:14px;font-style:italic;padding-left:4px;">"We recognize that the fundamental challenge we face is not one of technology, rather it is one of culture." - Dr. Vivek Goel </p>
<!-- HFI top row: 4 cards -->
<div class="hfi-grid-top">

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path><polyline points="9 22 9 12 15 12 15 22"></polyline></svg>
        <h4 spellcheck="true">Governance</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Is anyone accountable for connecting the system?</p></div>
    </div>
  </div>

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line></svg>
        <h4 spellcheck="true">Legislation</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Does the law allow paramedics to access patient data?</p></div>
    </div>
  </div>

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="3"></circle><path d="M19.07 4.93a10 10 0 0 1 0 14.14M4.93 4.93a10 10 0 0 0 0 14.14"></path></svg>
        <h4 spellcheck="true">Regulation</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Are health IT vendors required to build for interoperability?</p></div>
    </div>
  </div>

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
        <h4 spellcheck="true">Policy</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Have organizations committed to sharing data across boundaries?</p></div>
    </div>
  </div>

</div>

<!-- HFI bottom row: 3 cards -->
<div class="hfi-grid-bottom">

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"></path><path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"></path></svg>
        <h4 spellcheck="true">Literacy</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Does the workforce understand why this matters?</p></div>
    </div>
  </div>

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12 19.79 19.79 0 0 1 1.61 3.34 2 2 0 0 1 3.6 1.18h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.85a16 16 0 0 0 6.29 6.29l.95-.95a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7a2 2 0 0 1 1.73 2.03z"></path></svg>
        <h4 spellcheck="true">Communication</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Are stakeholders talking openly about who is responsible?</p></div>
    </div>
  </div>

  <div class="hfi-card-wrap" onclick="this.classList.toggle('flipped')">
    <div class="hfi-card-inner">
      <div class="hfi-card-front">
        <svg width="38" height="38" viewBox="0 0 24 24" fill="none" stroke="#6DCFDB" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>
        <h4 spellcheck="true">Culture</h4>
        <span class="hfi-card-hint">tap to reveal</span>
      </div>
      <div class="hfi-card-back"><p spellcheck="true">Does the system put patients ahead of organizational territory?</p></div>
    </div>
  </div>

</div>


<!-- FOOTER -->
<div class="footer">
  U of T EMHI &nbsp;&middot;&nbsp; 2026 &nbsp;&middot;&nbsp; Bridging the Gap: Paramedics, Health Informatics &amp; the Imperative for Continuity of Care
</div>

</body>
</html>

</body></html>
