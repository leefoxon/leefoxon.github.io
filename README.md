<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Citation Group — Workforce Risk Survey: Key Findings & Marketing Opportunities</title>
<style>
  :root {
    --pink: #E91E63;
    --magenta: #D81B60;
    --purple: #9C27B0;
    --orange: #FF6B35;
    --teal: #00BCD4;
    --dark: #37474F;
    --mid: #607D8B;
    --light: #ECEFF1;
    --white: #FFFFFF;
    --grad-primary: linear-gradient(135deg, #E91E63 0%, #9C27B0 100%);
    --grad-accent: linear-gradient(135deg, #D81B60 0%, #FF6B35 100%);
    --grad-teal: linear-gradient(135deg, #9C27B0 0%, #00BCD4 100%);
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: 'Segoe UI', Arial, sans-serif; color: var(--dark); background: #F8F9FA; font-size: 15px; line-height: 1.6; }

  /* ── Hero ── */
  .hero {
    background: var(--grad-primary);
    padding: 64px 48px 56px;
    color: white;
    position: relative;
    overflow: hidden;
  }
  .hero::before {
    content: '';
    position: absolute; top: -80px; right: -80px;
    width: 400px; height: 400px;
    border-radius: 50%;
    background: rgba(255,255,255,0.06);
  }
  .hero::after {
    content: '';
    position: absolute; bottom: -60px; left: 200px;
    width: 260px; height: 260px;
    border-radius: 50%;
    background: rgba(255,255,255,0.04);
  }
  .hero-label { font-size: 13px; font-weight: 600; letter-spacing: 2px; text-transform: uppercase; opacity: 0.8; margin-bottom: 14px; }
  .hero h1 { font-size: 42px; font-weight: 700; line-height: 1.15; margin-bottom: 12px; }
  .hero-sub { font-size: 18px; opacity: 0.9; margin-bottom: 32px; max-width: 680px; }
  .hero-meta { display: flex; gap: 32px; flex-wrap: wrap; }
  .hero-meta-item { display: flex; flex-direction: column; }
  .hero-meta-item .val { font-size: 28px; font-weight: 700; }
  .hero-meta-item .lbl { font-size: 12px; opacity: 0.75; text-transform: uppercase; letter-spacing: 1px; }

  /* ── Nav ── */
  .toc {
    background: white;
    border-bottom: 1px solid var(--light);
    padding: 0 48px;
    position: sticky; top: 0; z-index: 100;
    box-shadow: 0 2px 8px rgba(55,71,79,0.08);
  }
  .toc-inner { display: flex; gap: 0; overflow-x: auto; }
  .toc a { display: block; padding: 16px 20px; font-size: 13px; font-weight: 600; color: var(--mid); text-decoration: none; white-space: nowrap; border-bottom: 3px solid transparent; transition: all 0.2s; }
  .toc a:hover { color: var(--pink); border-bottom-color: var(--pink); }

  /* ── Layout ── */
  .content { max-width: 1200px; margin: 0 auto; padding: 56px 48px; }

  /* ── Section header ── */
  .section-divider {
    background: var(--grad-accent);
    color: white;
    padding: 20px 48px;
    margin: 56px -48px 40px;
    display: flex; align-items: center; gap: 16px;
  }
  .section-divider .num { font-size: 36px; font-weight: 700; opacity: 0.5; }
  .section-divider h2 { font-size: 22px; font-weight: 700; }

  /* ── Cards ── */
  .cards { display: grid; gap: 20px; }
  .cards-2 { grid-template-columns: repeat(2, 1fr); }
  .cards-3 { grid-template-columns: repeat(3, 1fr); }
  .cards-4 { grid-template-columns: repeat(4, 1fr); }

  .card {
    background: white; border-radius: 10px;
    padding: 24px; box-shadow: 0 2px 8px rgba(55,71,79,0.08);
  }
  .card-pink  { border-left: 5px solid var(--pink); }
  .card-purple{ border-left: 5px solid var(--purple); }
  .card-teal  { border-left: 5px solid var(--teal); }
  .card-orange{ border-left: 5px solid var(--orange); }
  .card-grad  { background: var(--grad-primary); color: white; border: none; }
  .card h3 { font-size: 15px; font-weight: 700; margin-bottom: 8px; color: var(--dark); }
  .card-grad h3 { color: white; }
  .card p  { font-size: 14px; color: var(--mid); line-height: 1.6; }
  .card-grad p { color: rgba(255,255,255,0.88); }

  /* ── KPI cards ── */
  .kpi { text-align: center; padding: 28px 20px; }
  .kpi .num { font-size: 48px; font-weight: 800; line-height: 1; margin-bottom: 8px; }
  .kpi .desc { font-size: 13px; font-weight: 600; text-transform: uppercase; letter-spacing: 0.5px; }
  .kpi-pink  .num { color: var(--pink); }
  .kpi-purple .num { color: var(--purple); }
  .kpi-teal  .num { color: var(--teal); }
  .kpi-orange .num { color: var(--orange); }

  /* ── Finding blocks ── */
  .finding {
    background: white; border-radius: 10px;
    padding: 28px 32px; margin-bottom: 20px;
    box-shadow: 0 2px 8px rgba(55,71,79,0.07);
    border-left: 6px solid var(--pink);
    display: flex; gap: 24px; align-items: flex-start;
  }
  .finding .f-num {
    font-size: 32px; font-weight: 800; color: var(--pink);
    line-height: 1; min-width: 44px;
  }
  .finding h3 { font-size: 17px; font-weight: 700; margin-bottom: 6px; color: var(--dark); }
  .finding p  { font-size: 14px; color: var(--mid); line-height: 1.65; }
  .finding .stat { display: inline-block; background: rgba(233,30,99,0.08); color: var(--pink); font-weight: 700; font-size: 13px; padding: 3px 10px; border-radius: 20px; margin: 6px 4px 0 0; }
  .finding .stat-purple { background: rgba(156,39,176,0.1); color: var(--purple); }
  .finding .stat-orange { background: rgba(255,107,53,0.1); color: var(--orange); }
  .finding .stat-teal   { background: rgba(0,188,212,0.1);  color: var(--teal); }

  /* ── Bar chart ── */
  .bar-chart { margin: 24px 0; }
  .bar-row { display: flex; align-items: center; gap: 12px; margin-bottom: 10px; }
  .bar-label { width: 260px; font-size: 13px; color: var(--dark); flex-shrink: 0; text-align: right; }
  .bar-track { flex: 1; height: 28px; background: var(--light); border-radius: 4px; overflow: hidden; }
  .bar-fill  { height: 100%; border-radius: 4px; display: flex; align-items: center; padding-left: 10px; color: white; font-size: 12px; font-weight: 700; transition: width 0.3s; }
  .bar-pink   { background: var(--grad-primary); }
  .bar-purple { background: var(--purple); }
  .bar-teal   { background: var(--teal); }
  .bar-orange { background: var(--orange); }
  .bar-dark   { background: var(--dark); }

  /* ── Opportunity cards ── */
  .opp {
    background: white; border-radius: 12px; padding: 28px;
    box-shadow: 0 3px 12px rgba(55,71,79,0.1);
    margin-bottom: 24px;
  }
  .opp-header { display: flex; align-items: flex-start; gap: 16px; margin-bottom: 16px; }
  .opp-icon { width: 48px; height: 48px; border-radius: 10px; display: flex; align-items: center; justify-content: center; font-size: 22px; flex-shrink: 0; }
  .opp-icon-pink   { background: rgba(233,30,99,0.1); }
  .opp-icon-purple { background: rgba(156,39,176,0.1); }
  .opp-icon-teal   { background: rgba(0,188,212,0.1);  }
  .opp-icon-orange { background: rgba(255,107,53,0.1); }
  .opp-title h3 { font-size: 18px; font-weight: 700; color: var(--dark); margin-bottom: 4px; }
  .opp-title .opp-type { font-size: 12px; font-weight: 600; text-transform: uppercase; letter-spacing: 1px; }
  .opp-type-pink   { color: var(--pink); }
  .opp-type-purple { color: var(--purple); }
  .opp-type-teal   { color: var(--teal); }
  .opp-type-orange { color: var(--orange); }
  .opp-body { font-size: 14px; color: var(--mid); line-height: 1.7; margin-bottom: 16px; }
  .tag-row { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 12px; }
  .tag { font-size: 12px; font-weight: 600; padding: 4px 12px; border-radius: 20px; }
  .tag-audience { background: rgba(233,30,99,0.1); color: var(--pink); }
  .tag-channel  { background: rgba(156,39,176,0.1); color: var(--purple); }
  .tag-format   { background: rgba(0,188,212,0.1);  color: var(--teal); }
  .tag-message  { background: rgba(255,107,53,0.1); color: var(--orange); }
  .opp-divider  { border: none; border-top: 1px solid var(--light); margin: 14px 0; }
  .diag-idea { background: rgba(156,39,176,0.05); border-radius: 8px; padding: 14px 16px; margin-top: 12px; }
  .diag-idea h4 { font-size: 13px; font-weight: 700; color: var(--purple); margin-bottom: 6px; }
  .diag-idea p  { font-size: 13px; color: var(--mid); }

  /* ── Two-col list ── */
  .two-col-list { columns: 2; gap: 24px; }
  .two-col-list li { font-size: 14px; color: var(--mid); margin-bottom: 6px; padding-left: 4px; break-inside: avoid; }

  /* ── Table ── */
  .data-table { width: 100%; border-collapse: collapse; margin: 20px 0; font-size: 13px; }
  .data-table th { background: var(--pink); color: white; padding: 10px 14px; text-align: left; font-weight: 600; }
  .data-table td { padding: 10px 14px; border-bottom: 1px solid var(--light); }
  .data-table tr:nth-child(even) td { background: rgba(236,239,241,0.5); }
  .data-table .hi { color: var(--pink); font-weight: 700; }
  .data-table .md { color: var(--orange); font-weight: 600; }

  /* ── Paradox callout ── */
  .paradox {
    background: var(--grad-primary); color: white;
    border-radius: 12px; padding: 32px 36px; margin: 28px 0;
    display: grid; grid-template-columns: 1fr 1fr; gap: 24px;
  }
  .paradox h3 { font-size: 16px; font-weight: 700; opacity: 0.75; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 8px; }
  .paradox-stat { font-size: 36px; font-weight: 800; margin-bottom: 4px; }
  .paradox p { font-size: 14px; opacity: 0.85; }
  .paradox-arrow { grid-column: 1 / -1; text-align: center; font-size: 13px; opacity: 0.8; border-top: 1px solid rgba(255,255,255,0.3); padding-top: 16px; font-style: italic; }

  /* ── Segment matrix ── */
  .seg-matrix { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin: 20px 0; }
  .seg-card { background: white; border-radius: 10px; padding: 20px; box-shadow: 0 2px 8px rgba(55,71,79,0.08); }
  .seg-card .seg-name { font-size: 14px; font-weight: 700; color: var(--dark); margin-bottom: 12px; padding-bottom: 10px; border-bottom: 3px solid var(--pink); }
  .seg-card .seg-stat { display: flex; justify-content: space-between; align-items: center; padding: 6px 0; border-bottom: 1px solid var(--light); font-size: 13px; }
  .seg-card .seg-stat .val { font-weight: 700; }
  .seg-card .seg-stat .val-hi { color: var(--pink); }
  .seg-card .seg-stat .val-md { color: var(--orange); }
  .seg-card .seg-stat .val-lo { color: var(--teal); }

  /* ── Footer ── */
  footer {
    background: var(--dark); color: rgba(255,255,255,0.65);
    padding: 32px 48px; font-size: 13px; margin-top: 80px;
    display: flex; justify-content: space-between; align-items: center;
  }
  footer strong { color: white; }

  /* ── Utils ── */
  h2.section-title { font-size: 26px; font-weight: 700; color: var(--dark); margin-bottom: 8px; }
  p.section-intro { font-size: 15px; color: var(--mid); margin-bottom: 28px; max-width: 820px; line-height: 1.7; }
  .mt24 { margin-top: 24px; }
  .mt32 { margin-top: 32px; }
  .mb16 { margin-bottom: 16px; }
  .pink { color: var(--pink); }
  strong.hi { color: var(--pink); }

  @media print {
    .toc { position: static; }
    .section-divider { margin: 40px 0 28px; }
  }
</style>
</head>
<body>

<!-- ── HERO ── -->
<div class="hero">
  <div class="hero-label">Citation Group · Research Intelligence</div>
  <h1>Workforce Risk & Compliance<br>Survey: Key Findings &amp; Opportunities</h1>
  <p class="hero-sub">A comprehensive summary of Australian business sentiment across HR, payroll, safety and compliance — with diagnostic and campaign opportunities for the marketing team.</p>
  <div class="hero-meta">
    <div class="hero-meta-item"><span class="val">510</span><span class="lbl">Complete responses</span></div>
    <div class="hero-meta-item"><span class="val">141</span><span class="lbl">Survey variables</span></div>
    <div class="hero-meta-item"><span class="val">36</span><span class="lbl">Industries represented</span></div>
    <div class="hero-meta-item"><span class="val">Jan–Feb 2026</span><span class="lbl">Fieldwork period</span></div>
  </div>
</div>

<!-- ── NAV ── -->
<nav class="toc">
  <div class="toc-inner">
    <a href="#findings">Key Findings</a>
    <a href="#paradox">The Confidence Paradox</a>
    <a href="#domains">Four Domains</a>
    <a href="#segments">Segment Profiles</a>
    <a href="#opportunities">Marketing Opportunities</a>
    <a href="#diagnostics">Diagnostic Ideas</a>
    <a href="#campaigns">Campaign Programs</a>
  </div>
</nav>

<div class="content">

<!-- ══════════════════════════════════════════════════════════
     SECTION 1: KEY FINDINGS
══════════════════════════════════════════════════════════ -->
<div id="findings">
  <div class="section-divider" style="background: var(--grad-primary);">
    <span class="num">01</span>
    <h2>Key Findings at a Glance</h2>
  </div>

  <h2 class="section-title">What the data tells us</h2>
  <p class="section-intro">510 Australian business owners, C-Suite executives and senior managers completed this survey. All are in full-time paid employment, all have active workforce management responsibilities. The findings reveal a market where surface-level confidence is high but operational anxiety is deep, specific, and widespread.</p>

  <div class="cards cards-4">
    <div class="card kpi kpi-pink">
      <div class="num">97%</div>
      <div class="desc">Feel broadly confident managing workplace responsibilities</div>
    </div>
    <div class="card kpi kpi-purple">
      <div class="num">78%</div>
      <div class="desc">Say management feels more complex than before</div>
    </div>
    <div class="card kpi kpi-orange">
      <div class="num">73%</div>
      <div class="desc">Believe the right support would significantly reduce their stress</div>
    </div>
    <div class="card kpi kpi-teal">
      <div class="num">42%</div>
      <div class="desc">Have discovered a payroll error or underpayment in their business</div>
    </div>
  </div>

  <div class="mt32">
    <div class="finding">
      <div class="f-num">1</div>
      <div>
        <h3>The "Confidence Paradox" — surface confidence masks deep operational anxiety</h3>
        <p>97% feel broadly confident, yet 78% say management is more complex than before, 69% say it takes too much of their time, and 73% say better support would reduce their stress. These two truths coexist throughout the data — and this tension is Citation's commercial entry point.</p>
        <span class="stat">97% broadly confident</span>
        <span class="stat stat-orange">78% experiencing increased complexity</span>
        <span class="stat stat-purple">73% want support to reduce stress</span>
      </div>
    </div>

    <div class="finding">
      <div class="f-num">2</div>
      <div>
        <h3>Payroll complexity and errors are systemic, not isolated</h3>
        <p>42% have discovered a payroll error or underpayment. 67% say Fair Work Awards or pay rules take more time than they should. 49% find payroll management unnecessarily complex — rising to 54% in mid-sized businesses. This is a widespread, recurring pain point across every cohort.</p>
        <span class="stat">67% Fair Work friction</span>
        <span class="stat stat-orange">42% discovered payroll errors</span>
        <span class="stat stat-purple">49% say payroll is unnecessarily complex</span>
      </div>
    </div>

    <div class="finding">
      <div class="f-num">3</div>
      <div>
        <h3>Psychosocial risk is the fastest-emerging gap in the compliance landscape</h3>
        <p>While physical H&S confidence is high (89%), confidence managing psychosocial risks falls to 77% — and only 55% find people management rewarding and not stressful. 30% are concerned about a psychosocial issue escalating, and this is now a direct regulatory requirement. It sits at the frontier of compliance for most small-to-mid businesses.</p>
        <span class="stat">89% confident on physical H&S</span>
        <span class="stat stat-orange">77% confident on psychosocial — the widest gap</span>
        <span class="stat stat-purple">30% worried about psychosocial escalation</span>
      </div>
    </div>

    <div class="finding">
      <div class="f-num">4</div>
      <div>
        <h3>Skills shortages and data security are the top near-term concerns</h3>
        <p>Skills shortages top the concern list at 38%, followed closely by data breaches (37%), missing a compliance requirement (33%), and workplace safety incidents (34%). These are not hypothetical fears — they are live operational pressures that create clear entry points for structured risk conversations.</p>
        <span class="stat">38% — Skills shortages</span>
        <span class="stat stat-purple">37% — Data breach risk</span>
        <span class="stat stat-orange">34% — Workplace injury risk</span>
      </div>
    </div>

    <div class="finding">
      <div class="f-num">5</div>
      <div>
        <h3>Mid-sized businesses (20–100 staff) carry the highest strain — with the highest appetite for support</h3>
        <p>This cohort scores highest on payroll complexity (54%), time burden, and pay error worry (48%). They are too large for informal owner-managed compliance, too small for dedicated compliance teams. 77% say right support would reduce stress, and 34% want a single integrated HR/payroll/compliance system — the strongest demand of any segment.</p>
        <span class="stat">54% find payroll unnecessarily complex</span>
        <span class="stat stat-orange">77% say right support reduces stress</span>
        <span class="stat stat-purple">34% want integrated system</span>
      </div>
    </div>

    <div class="finding">
      <div class="f-num">6</div>
      <div>
        <h3>System fragmentation is universal — single integrated solutions are the top desire</h3>
        <p>Only 19% manage people, payroll and safety through a single system. 55% use 2–3 systems, 22% use 4 or more. The top service wished for today is a single integrated HR/payroll/compliance system (30%), followed by an online learning platform (29%). Only 12% say they need none of the services listed.</p>
        <span class="stat">81% using 2+ separate systems</span>
        <span class="stat stat-orange">30% want single integrated platform</span>
        <span class="stat stat-teal">88% have at least one unmet service need</span>
      </div>
    </div>

    <div class="finding">
      <div class="f-num">7</div>
      <div>
        <h3>The regulatory treadmill is the defining forward-looking pressure</h3>
        <p>Looking ahead, talent attraction (37%) and evolving compliance (35%) top future challenges. Three of the top five future concerns involve regulatory burden. 78% feel prepared for future changes — but only 57% find law changes manageable, suggesting preparedness confidence may be more aspiration than reality.</p>
        <span class="stat">37% — Attracting &amp; retaining talent</span>
        <span class="stat stat-orange">35% — Evolving compliance requirements</span>
        <span class="stat stat-purple">31% — Keeping up with new laws</span>
      </div>
    </div>
  </div>
</div>


<!-- ══════════════════════════════════════════════════════════
     SECTION 2: CONFIDENCE PARADOX
══════════════════════════════════════════════════════════ -->
<div id="paradox">
  <div class="section-divider" style="background: var(--grad-accent);">
    <span class="num">02</span>
    <h2>The Confidence Paradox — Citation's Commercial Entry Point</h2>
  </div>

  <h2 class="section-title">Confident on the surface. Anxious underneath.</h2>
  <p class="section-intro">The most important strategic insight in the data is the sustained coexistence of high broad confidence and high specific anxiety. This is not cognitive dissonance — it reflects that business leaders have learned to manage complexity through effort and vigilance, but that effort is costly and unsustainable.</p>

  <div class="paradox">
    <div>
      <h3>What they say they feel</h3>
      <div class="paradox-stat">97%</div>
      <p>Feel broadly confident managing workplace responsibilities</p>
    </div>
    <div>
      <h3>What the data actually shows</h3>
      <div class="paradox-stat">78%</div>
      <p>Say it feels more complex than before</p>
    </div>
    <div>
      <h3>And yet...</h3>
      <div class="paradox-stat">87%</div>
      <p>Feel confident their payroll is accurate</p>
    </div>
    <div>
      <h3>While simultaneously...</h3>
      <div class="paradox-stat">43%</div>
      <p>Worry about getting pay or entitlements wrong</p>
    </div>
    <div class="paradox-arrow">The gap between stated confidence and operational anxiety is Citation's commercial white space — the market is not seeking rescue, it is seeking relief.</div>
  </div>

  <div class="cards cards-3 mt24">
    <div class="card card-pink">
      <h3>Only 55% find people management rewarding</h3>
      <p>The weakest confidence score in the entire dataset — below H&S (89%), payroll accuracy (87%), and system consistency (87%). People management fatigue is widespread and under-addressed.</p>
    </div>
    <div class="card card-purple">
      <h3>Only 57% find law changes manageable</h3>
      <p>The most widespread confidence gap — 73% of industries in the 5–19 cohort score at or below 70%. Regulatory change burden is a structural vulnerability for businesses without dedicated compliance resources.</p>
    </div>
    <div class="card card-orange">
      <h3>73% say right support = less stress</h3>
      <p>This is the strongest single signal of unmet demand in the dataset. It frames the proposition clearly: Citation's value is not about capability — it is about stress relief and sustainable compliance.</p>
    </div>
  </div>
</div>


<!-- ══════════════════════════════════════════════════════════
     SECTION 3: FOUR DOMAINS
══════════════════════════════════════════════════════════ -->
<div id="domains">
  <div class="section-divider" style="background: var(--grad-teal);">
    <span class="num">03</span>
    <h2>The Four Compliance Domains — Confidence &amp; Strain Profile</h2>
  </div>

  <h2 class="section-title">Where confidence holds and where it fractures</h2>
  <p class="section-intro">The survey covers four core workforce management domains. Each tells a different story about where businesses are coping and where they are exposed.</p>

  <div class="cards cards-2">

    <div class="card card-pink">
      <h3>🧑‍💼 HR &amp; People Management</h3>
      <div class="bar-chart" style="margin-top:16px;">
        <div class="bar-row"><span class="bar-label">Find it rewarding &amp; not stressful</span><div class="bar-track"><div class="bar-fill bar-pink" style="width:63%">63%</div></div></div>
        <div class="bar-row"><span class="bar-label">Issues escalate more than expected</span><div class="bar-track"><div class="bar-fill bar-orange" style="width:47%">47%</div></div></div>
        <div class="bar-row"><span class="bar-label">Find law changes manageable</span><div class="bar-track"><div class="bar-fill bar-pink" style="width:68%">68%</div></div></div>
        <div class="bar-row"><span class="bar-label">Management MORE complex than before</span><div class="bar-track"><div class="bar-fill bar-dark" style="width:78%">78%</div></div></div>
      </div>
      <p style="font-size:13px;color:var(--mid);margin-top:8px;"><strong class="hi">Key vulnerability:</strong> 47% experience people issues escalating further than expected, and only 63% find people management rewarding. The HR people layer is the most emotionally burdensome domain.</p>
    </div>

    <div class="card card-purple">
      <h3>💰 Payroll &amp; Wage Compliance</h3>
      <div class="bar-chart" style="margin-top:16px;">
        <div class="bar-row"><span class="bar-label">Confident payroll is accurate</span><div class="bar-track"><div class="bar-fill bar-purple" style="width:87%">87%</div></div></div>
        <div class="bar-row"><span class="bar-label">Prepared for wage audits</span><div class="bar-track"><div class="bar-fill bar-purple" style="width:80%">80%</div></div></div>
        <div class="bar-row"><span class="bar-label">Fair Work Awards take too long</span><div class="bar-track"><div class="bar-fill bar-dark" style="width:67%">67%</div></div></div>
        <div class="bar-row"><span class="bar-label">Payroll unnecessarily complex</span><div class="bar-track"><div class="bar-fill bar-orange" style="width:49%">49%</div></div></div>
        <div class="bar-row"><span class="bar-label">Worry about pay errors</span><div class="bar-track"><div class="bar-fill bar-orange" style="width:43%">43%</div></div></div>
      </div>
      <p style="font-size:13px;color:var(--mid);margin-top:8px;"><strong style="color:var(--purple)">Key vulnerability:</strong> Classic confidence paradox — 87% confident but 43% worried. 42% have actually discovered an error. This is the highest-conversion domain for payroll audit and review services.</p>
    </div>

    <div class="card card-teal">
      <h3>🦺 Health, Safety &amp; Wellbeing</h3>
      <div class="bar-chart" style="margin-top:16px;">
        <div class="bar-row"><span class="bar-label">Confident meeting H&amp;S obligations</span><div class="bar-track"><div class="bar-fill bar-teal" style="width:89%">89%</div></div></div>
        <div class="bar-row"><span class="bar-label">Confident managing psychosocial risks</span><div class="bar-track"><div class="bar-fill bar-teal" style="width:77%">77%</div></div></div>
        <div class="bar-row"><span class="bar-label">Safety adds to personal stress</span><div class="bar-track"><div class="bar-fill bar-dark" style="width:61%">61%</div></div></div>
        <div class="bar-row"><span class="bar-label">Serious safety issue is top concern</span><div class="bar-track"><div class="bar-fill bar-orange" style="width:62%">62%</div></div></div>
      </div>
      <p style="font-size:13px;color:var(--mid);margin-top:8px;"><strong style="color:var(--teal)">Key vulnerability:</strong> 12-point gap between physical H&S confidence (89%) and psychosocial confidence (77%). Psychosocial is the rising regulatory frontier — most businesses are underprepared.</p>
    </div>

    <div class="card card-orange">
      <h3>⚙️ Systems, Technology &amp; Future Readiness</h3>
      <div class="bar-chart" style="margin-top:16px;">
        <div class="bar-row"><span class="bar-label">Info accurate across systems</span><div class="bar-track"><div class="bar-fill bar-orange" style="width:87%">87%</div></div></div>
        <div class="bar-row"><span class="bar-label">Feel future-ready</span><div class="bar-track"><div class="bar-fill bar-orange" style="width:82%">82%</div></div></div>
        <div class="bar-row"><span class="bar-label">Using 2+ separate systems</span><div class="bar-track"><div class="bar-fill bar-dark" style="width:81%">81%</div></div></div>
        <div class="bar-row"><span class="bar-label">Currently using AI/automation</span><div class="bar-track"><div class="bar-fill bar-purple" style="width:60%">60%</div></div></div>
      </div>
      <p style="font-size:13px;color:var(--mid);margin-top:8px;"><strong style="color:var(--orange)">Key vulnerability:</strong> 81% using 2+ systems yet 87% claim info is accurate across them — a likely overstatement. System fragmentation is the infrastructure root cause of most compliance risk.</p>
    </div>

  </div>
</div>


<!-- ══════════════════════════════════════════════════════════
     SECTION 4: SEGMENT PROFILES
══════════════════════════════════════════════════════════ -->
<div id="segments">
  <div class="section-divider" style="background: var(--grad-primary);">
    <span class="num">04</span>
    <h2>Segment Profiles — Where Targeting Matters Most</h2>
  </div>

  <h2 class="section-title">Not all anxiety is equal — three distinct audience profiles emerge</h2>
  <p class="section-intro">Segmentation by company size reveals structurally different risk profiles. Each represents a distinct marketing and product proposition.</p>

  <div class="seg-matrix">
    <div class="seg-card">
      <div class="seg-name">5–19 Employees (n=204)<br><span style="font-weight:400;font-size:12px;color:var(--mid)">The owner-managed frontier</span></div>
      <div class="seg-stat"><span>Law changes feel manageable</span><span class="val val-md">57%</span></div>
      <div class="seg-stat"><span>More complex than before</span><span class="val val-hi">79%</span></div>
      <div class="seg-stat"><span>Too much of MY personal time</span><span class="val val-hi">70%</span></div>
      <div class="seg-stat"><span>Attract &amp; retain talent concern</span><span class="val val-hi">46%</span></div>
      <div class="seg-stat"><span>Want right support (stress)</span><span class="val val-md">66%</span></div>
      <div class="seg-stat"><span>Want integrated system</span><span class="val val-md">29%</span></div>
      <p style="font-size:12px;color:var(--mid);margin-top:12px;">Primary pain: time burden and regulatory unreadiness. The owner IS the HR team. Messaging should focus on <strong>reclaiming time</strong> and <strong>removing uncertainty</strong>.</p>
    </div>
    <div class="seg-card" style="border-top: 4px solid var(--pink);">
      <div class="seg-name" style="border-color:var(--pink);">20–100 Employees (n=204)<br><span style="font-weight:400;font-size:12px;color:var(--mid)">⭐ Highest-strain, highest-opportunity</span></div>
      <div class="seg-stat"><span>Payroll unnecessarily complex</span><span class="val val-hi">54%</span></div>
      <div class="seg-stat"><span>Worry about pay errors</span><span class="val val-hi">48%</span></div>
      <div class="seg-stat"><span>Management limits growth</span><span class="val val-hi">67%</span></div>
      <div class="seg-stat"><span>Fair Work takes too long</span><span class="val val-hi">72%</span></div>
      <div class="seg-stat"><span>Want right support (stress)</span><span class="val val-hi">77%</span></div>
      <div class="seg-stat"><span>Want integrated system</span><span class="val val-hi">34%</span></div>
      <p style="font-size:12px;color:var(--mid);margin-top:12px;">Primary pain: structural gap — too complex for ad hoc, too small for dedicated teams. Messaging should focus on <strong>growth enablement</strong> and <strong>payroll protection</strong>.</p>
    </div>
    <div class="seg-card">
      <div class="seg-name">100+ Employees (n=102)<br><span style="font-weight:400;font-size:12px;color:var(--mid)">The compliance-sophisticate</span></div>
      <div class="seg-stat"><span>Law changes feel manageable</span><span class="val val-lo">82%</span></div>
      <div class="seg-stat"><span>Payroll errors discovered</span><span class="val val-hi">47%</span></div>
      <div class="seg-stat"><span>Skills shortages concern</span><span class="val val-hi">33%</span></div>
      <div class="seg-stat"><span>Evolving compliance challenge</span><span class="val val-hi">37%</span></div>
      <div class="seg-stat"><span>Want right support (stress)</span><span class="val val-hi">80%</span></div>
      <div class="seg-stat"><span>Want HR on-demand advice</span><span class="val val-md">28%</span></div>
      <p style="font-size:12px;color:var(--mid);margin-top:12px;">Primary pain: scale complexity and audit exposure. Despite resources, 47% have found errors. Messaging should focus on <strong>audit readiness</strong> and <strong>strategic compliance</strong>.</p>
    </div>
  </div>

  <div class="mt32">
    <h3 class="mb16" style="font-size:18px;font-weight:700;color:var(--dark);">Role-based targeting signals</h3>
    <table class="data-table">
      <thead><tr><th>Role</th><th>Defining anxiety</th><th>Highest concern</th><th>Support appetite</th><th>Best message</th></tr></thead>
      <tbody>
        <tr><td><strong>Owners</strong> (22%)</td><td>Time drain (70%), law unreadiness (60%)</td><td>Attract &amp; retain talent (36%)</td><td class="md">66% — right support reduces stress</td><td>"Get your time back. We carry the compliance load."</td></tr>
        <tr><td><strong>C-Suite</strong> (17%)</td><td>Data breach (41%), safety stress (65%)</td><td class="hi">"Not knowing what I don't know" (29%)</td><td class="hi">81% — right support reduces stress</td><td>"Complete visibility. Confident decisions."</td></tr>
        <tr><td><strong>Senior Managers</strong> (61%)</td><td>Pay error worry (44%), complexity (76%)</td><td>Skills shortages (38%)</td><td class="md">74% — right support reduces stress</td><td>"Reduce the risk. Manage with confidence."</td></tr>
      </tbody>
    </table>
  </div>
</div>


<!-- ══════════════════════════════════════════════════════════
     SECTION 5: MARKETING OPPORTUNITIES
══════════════════════════════════════════════════════════ -->
<div id="opportunities">
  <div class="section-divider" style="background: var(--grad-accent);">
    <span class="num">05</span>
    <h2>Marketing Opportunities — Where to Play</h2>
  </div>

  <h2 class="section-title">Eight high-signal campaign territories</h2>
  <p class="section-intro">Each opportunity below is grounded directly in survey data. The audience signal, message angle, channel thinking and diagnostic hook are all derived from what respondents actually told us.</p>

  <!-- OPP 1 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-pink">💸</div>
      <div class="opp-title">
        <div class="opp-type opp-type-pink">Payroll Compliance · High Priority</div>
        <h3>The Payroll Anxiety Campaign — "You might already have a problem"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> 87% feel confident about payroll accuracy — yet 42% have already discovered an error, and 43% worry about getting pay or entitlements wrong. 67% say Fair Work Awards take more time than they should. This is a category defined by false security.<br><br>
      <strong>The opportunity:</strong> A campaign that doesn't attack confidence but instead reframes it — "Confidence is good. Verification is better." Lead with the underpayment risk narrative (regulatory enforcement, reputational damage, Fair Work compliance). The data shows 80% feel prepared for wage audits, but 54% of mid-sized businesses find payroll unnecessarily complex. That gap is the message.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">20–100 staff (primary)</span>
      <span class="tag tag-audience">100+ staff (secondary)</span>
      <span class="tag tag-channel">LinkedIn · Email · Search</span>
      <span class="tag tag-format">Lead gen · Webinar · Audit CTA</span>
      <span class="tag tag-message">"Confident your payroll is right? Prove it."</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Payroll Risk Self-Assessment</h4>
      <p>A short (5-question) online diagnostic that benchmarks a respondent's payroll exposure — award complexity, manual processes, time since last audit. Output: a personalised risk score and report. Entry point to payroll review or audit support services. 21% of respondents actively want payroll review/audit support today.</p>
    </div>
  </div>

  <!-- OPP 2 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-purple">🧠</div>
      <div class="opp-title">
        <div class="opp-type opp-type-purple">Psychosocial Safety · Emerging Priority</div>
        <h3>The Psychosocial Frontier — "The obligation most businesses aren't ready for"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> Physical H&S confidence is 89%. Psychosocial risk confidence is 77% — a 12-point gap. Only 55% find people management rewarding and not stressful. 30% are concerned about a psychosocial issue escalating. In the 5–19 cohort, Technology (30%), Education (57%), and Manufacturing (50%) show the weakest psychosocial confidence.<br><br>
      <strong>The opportunity:</strong> Psychosocial risk obligations are now legislated across Australian states. Most businesses know they should be doing something — very few have structured responses. A campaign anchored in "the obligation you can't ignore in 2026" with practical guidance as the hook has a clear path to product engagement (EAP, risk assessments, training).
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">All sizes · C-Suite &amp; Owners</span>
      <span class="tag tag-channel">LinkedIn · Industry media · Email</span>
      <span class="tag tag-format">Content series · Checklist · Risk guide</span>
      <span class="tag tag-message">"Psychosocial risk is now a legal obligation. Is your business ready?"</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Psychosocial Risk Readiness Check</h4>
      <p>A structured 8-question diagnostic covering: risk identification processes, incident response, manager capability, and reporting frameworks. Output: a readiness band (Exposed / Developing / Established) with tailored recommendations. High organic search potential given regulatory attention. 24% of all respondents want psychosocial risk guidance today.</p>
    </div>
  </div>

  <!-- OPP 3 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-teal">⏱️</div>
      <div class="opp-title">
        <div class="opp-type opp-type-teal">HR Efficiency · Broad Reach</div>
        <h3>The Time Drain Campaign — "You shouldn't be spending this much time on compliance"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> 69% say workforce responsibilities take up more of their personal time than they'd like. 40% spend 2–5 hours per month understanding HR/safety obligations; 11% spend more than 10 hours monthly. 78% say management is more complex than before. People management is the second-most time-consuming domain after systems/payroll.<br><br>
      <strong>The opportunity:</strong> Position Citation's services as time recovery, not just risk mitigation. The emotional hook — "this is eating your week" — resonates across every size band and role type. Quantify the time cost in a campaign to make the abstract concrete. "The average Australian business owner spends X hours a month on compliance that a support service would handle."
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">Owners (primary) · Senior Managers</span>
      <span class="tag tag-channel">LinkedIn · Paid Social · Podcast ads</span>
      <span class="tag tag-format">Time-cost calculator · Short video · Infographic</span>
      <span class="tag tag-message">"You're spending 6+ hours a month on compliance. We can give that back."</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Compliance Time Cost Calculator</h4>
      <p>A simple tool: "How many hours a month does your team spend on HR, payroll and compliance?" × average salary rate = annual cost in dollars. Compare against a Citation service package. Extremely shareable, low barrier to entry, clear commercial bridge. Output links to on-demand HR advice or integrated system proposition.</p>
    </div>
  </div>

  <!-- OPP 4 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-orange">📈</div>
      <div class="opp-title">
        <div class="opp-type opp-type-orange">Growth Enablement · Strategic Play</div>
        <h3>The Growth Blocker Campaign — "Compliance shouldn't cost you your growth"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> 62% say workforce management limits their ability to focus on growth and core business priorities. This is highest among mid-sized businesses (67%), Engineering (100%), Manufacturing (100%), and Consulting (89%). 73% say the right support would reduce their stress. The link between compliance burden and stalled growth is explicit in the data.<br><br>
      <strong>The opportunity:</strong> A growth-framed campaign targeting mid-market and professional services businesses. Reposition compliance management from "cost and obligation" to "growth infrastructure." Works well for a LinkedIn-led campaign targeting business owners and C-Suite who aspire to scale.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">20–100 staff · Engineering · Consulting · Manufacturing</span>
      <span class="tag tag-channel">LinkedIn · Direct email · Trade press</span>
      <span class="tag tag-format">Case studies · ROI calculator · Event</span>
      <span class="tag tag-message">"Stop letting compliance get in the way of your next growth phase."</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Compliance Maturity Benchmark</h4>
      <p>A 10-question assessment mapping a business across the four compliance domains (HR, payroll, safety, systems). Output: a maturity band with industry benchmarks drawn directly from this survey data ("businesses like yours score X on payroll readiness"). Commercial bridge to integrated service packages. Strongly motivated by the 35% of businesses who are 'partially systemised' or lower.</p>
    </div>
  </div>

  <!-- OPP 5 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-pink">🔗</div>
      <div class="opp-title">
        <div class="opp-type opp-type-pink">Integration · Platform Play</div>
        <h3>The Fragmentation Campaign — "Your data is spread across 3 systems. So is your risk."</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> 81% of businesses use 2 or more separate systems for people, payroll and safety management. 30% want a single integrated HR/payroll/compliance system — the top service desired across the full sample. System fragmentation is the infrastructure root cause behind most of the compliance anxieties in this survey.<br><br>
      <strong>The opportunity:</strong> A platform/integration campaign that leads with the visible symptom (fragmentation, manual reconciliation, inconsistent data) and positions integration as the structural fix. Data from the survey provides third-party validation: "81% of Australian businesses are managing people, payroll and safety across multiple disconnected systems."
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">20–100 staff (primary) · C-Suite &amp; Ops leaders</span>
      <span class="tag tag-channel">LinkedIn · Search (high intent) · Email</span>
      <span class="tag tag-format">Demo · ROI calculator · Comparison guide</span>
      <span class="tag tag-message">"One system. All your people, pay and safety data. Finally."</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Systems Audit Questionnaire</h4>
      <p>A 6-question audit mapping which systems a business uses for HR records, payroll, WHS, learning and compliance tracking. Output: a fragmentation score + a visual "systems map" showing where their data siloes are and what that costs them in risk exposure. Natural CTA to a platform demo or systems consultation.</p>
    </div>
  </div>

  <!-- OPP 6 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-purple">⚖️</div>
      <div class="opp-title">
        <div class="opp-type opp-type-purple">Industrial Relations · Sector Campaign</div>
        <h3>The IR Complexity Campaign — "Fair Work shouldn't be this hard for small business"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> 61% of all respondents operate in environments where IR obligations are relevant. Of those, 29% find them challenging or very challenging. 67% agree Fair Work Awards take more time than they should — rising to 72% in the 20–100 staff band. Industries with the highest Fair Work burden: Shipping/Logistics (100%), Manufacturing (81%), Disability Services (80%), Accounting (79%), Engineering (79%).<br><br>
      <strong>The opportunity:</strong> A targeted campaign for award-dense industries where Fair Work complexity is the primary compliance cost. Sector-specific versions work well here — a Manufacturing or Retail version of the campaign will outperform a generic message because the award context is highly specific.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">Manufacturing · Retail · Disability · Transport · Hospitality</span>
      <span class="tag tag-channel">Industry associations · Trade media · LinkedIn</span>
      <span class="tag tag-format">Award guide · Compliance calendar · Webinar</span>
      <span class="tag tag-message">"Running a [Retail/Manufacturing] business? You have 4 Modern Awards to navigate."</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Award Complexity Checker</h4>
      <p>Industry + employee type inputs → outputs which Modern Awards apply, key classification risks, and recent changes. Pairs naturally with foundU's payroll ruleset capability. Could be co-branded or lead-shared between Citation and foundU. High organic search value for "Modern Award [industry]" queries.</p>
    </div>
  </div>

  <!-- OPP 7 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-teal">🤖</div>
      <div class="opp-title">
        <div class="opp-type opp-type-teal">AI &amp; Future Readiness · Forward Play</div>
        <h3>The Responsible AI Campaign — "60% of businesses are using AI. How many have a policy?"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> 60% of respondents are already using AI or automation. AI adoption is a top-3 future challenge for 28% of businesses. Yet confidence that AI is being adopted safely and appropriately lags adoption — suggesting governance is outpaced by implementation. 40% of future challenge respondents flag AI as a concern; C-Suite score this highest.<br><br>
      <strong>The opportunity:</strong> A thought-leadership-led campaign positioning Citation as the trusted guide for responsible AI adoption in a workforce context — covering data privacy, employment law implications, psychosocial risks of AI workloads, and policy frameworks. High resonance with C-Suite and tech-forward businesses.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">C-Suite · Technology · Finance · Consulting</span>
      <span class="tag tag-channel">LinkedIn · Podcast · Conference</span>
      <span class="tag tag-format">Whitepaper · Policy template · Webinar</span>
      <span class="tag tag-message">"Your team is already using AI. Do you have an AI Workplace Policy?"</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: AI Workplace Readiness Audit</h4>
      <p>A 7-question tool covering: current AI tool usage, data privacy policies, employment impact assessment, psychosocial risk of AI workloads, and policy documentation. Output: a readiness gap report with three recommended actions. High-authority content play — limited competition in this space from Australian HR compliance providers.</p>
    </div>
  </div>

  <!-- OPP 8 -->
  <div class="opp">
    <div class="opp-header">
      <div class="opp-icon opp-icon-orange">🎯</div>
      <div class="opp-title">
        <div class="opp-type opp-type-orange">Talent &amp; Culture · Acquisition Play</div>
        <h3>The Talent Anxiety Campaign — "You can't attract great people into a compliance mess"</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>The data signal:</strong> Attracting and retaining talent is the #1 future challenge at 37%, and it is highest in the 5–19 employee cohort (46%). 18% want manager/leadership training; 27% want employee wellbeing/EAP support; 29% want an online learning platform. These three desires cluster around the same problem: building a workplace people want to stay in.<br><br>
      <strong>The opportunity:</strong> A campaign that connects compliance maturity to employer brand — "the businesses that attract the best people have the best HR foundations." Positions Citation's people management, learning, and EAP products as talent infrastructure rather than compliance overhead. Particularly powerful for the 5–19 cohort where owner-operators are personally driving recruitment.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">5–19 staff (primary) · Owners &amp; Senior Managers</span>
      <span class="tag tag-channel">LinkedIn · Instagram · Referral</span>
      <span class="tag tag-format">Guide · Checklist · Workshop</span>
      <span class="tag tag-message">"Your best people are watching how you manage your workforce."</span>
    </div>
    <hr class="opp-divider">
    <div class="diag-idea">
      <h4>🔬 Diagnostic Opportunity: Employer Attractiveness Health Check</h4>
      <p>A short tool measuring: onboarding quality, manager capability, wellbeing provision, flexibility policies, and learning opportunities. Output: an employer attractiveness score with benchmarks. Strong social sharing potential ("We scored 74/100 as an employer"). Bridges to iHasco, EAP, and HR advisory products.</p>
    </div>
  </div>

</div>


<!-- ══════════════════════════════════════════════════════════
     SECTION 6: DIAGNOSTIC PORTFOLIO
══════════════════════════════════════════════════════════ -->
<div id="diagnostics">
  <div class="section-divider" style="background: var(--grad-teal);">
    <span class="num">06</span>
    <h2>Diagnostic Portfolio — Building a Risk Intelligence Engine</h2>
  </div>

  <h2 class="section-title">From one-off tools to a connected diagnostic ecosystem</h2>
  <p class="section-intro">Each individual diagnostic creates lead generation value. Together, they can form a connected "Workforce Risk Intelligence" platform that positions Citation as the definitive benchmark source for Australian business compliance — and feeds a rich first-party data asset.</p>

  <div class="cards cards-2 mt24">
    <div class="card card-pink">
      <h3>Short-form diagnostics (top of funnel)</h3>
      <p style="margin:8px 0 12px;">High volume, low friction. 3–5 questions. Immediate output. Social-shareable result. Designed for paid and organic traffic.</p>
      <ul style="padding-left:18px;">
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Compliance Time Cost Calculator</li>
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Payroll Risk Score (5 questions)</li>
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Award Complexity Checker</li>
        <li style="font-size:13px;color:var(--mid);">Employer Attractiveness Score</li>
      </ul>
    </div>
    <div class="card card-purple">
      <h3>Mid-form diagnostics (mid funnel)</h3>
      <p style="margin:8px 0 12px;">8–12 questions. Personalised report output. Email gate for results. Designed for lead capture and sales qualification.</p>
      <ul style="padding-left:18px;">
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Psychosocial Risk Readiness Check</li>
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Systems Fragmentation Audit</li>
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">AI Workplace Readiness Audit</li>
        <li style="font-size:13px;color:var(--mid);">Compliance Maturity Benchmark</li>
      </ul>
    </div>
    <div class="card card-teal">
      <h3>Deep diagnostic (bottom of funnel)</h3>
      <p style="margin:8px 0 12px;">20–30 questions across all four domains. Produces a full "Workforce Risk Report" — personalised, benchmarked, actionable. Gated behind a consultation booking.</p>
      <ul style="padding-left:18px;">
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Full Workforce Risk Assessment</li>
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Industry-benchmarked results (powered by this survey)</li>
        <li style="font-size:13px;color:var(--mid);">Recommended product pathways by risk band</li>
      </ul>
    </div>
    <div class="card card-orange">
      <h3>Annual benchmark report (PR &amp; authority)</h3>
      <p style="margin:8px 0 12px;">Publish this research publicly as "The Citation Workforce Risk Index" — an annual state-of-the-nation on Australian business compliance sentiment. PR, media, industry associations, LinkedIn.</p>
      <ul style="padding-left:18px;">
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Establishes Citation as the authoritative research source</li>
        <li style="font-size:13px;color:var(--mid);margin-bottom:6px;">Fuels 12 months of content campaigns</li>
        <li style="font-size:13px;color:var(--mid);">Year-on-year tracking creates ongoing media angles</li>
      </ul>
    </div>
  </div>
</div>


<!-- ══════════════════════════════════════════════════════════
     SECTION 7: CAMPAIGN PROGRAMS
══════════════════════════════════════════════════════════ -->
<div id="campaigns">
  <div class="section-divider" style="background: var(--grad-primary);">
    <span class="num">07</span>
    <h2>Campaign Programs — Connecting the Dots</h2>
  </div>

  <h2 class="section-title">Three recommended campaign programs for FY26</h2>
  <p class="section-intro">Rather than running eight separate campaigns, the opportunities above naturally cluster into three integrated campaign programs, each with a clear primary audience, a content engine, a diagnostic entry point, and a commercial outcome.</p>

  <div class="opp" style="border-left: 6px solid var(--pink);">
    <div class="opp-header">
      <div class="opp-icon opp-icon-pink" style="font-size:28px;">🛡️</div>
      <div class="opp-title">
        <div class="opp-type opp-type-pink">Program 1 · Flagship</div>
        <h3>The "Protected" Program — Compliance confidence for the mid-market</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>Primary audience:</strong> 20–100 employee businesses, owners and C-Suite, across Retail, Manufacturing, Consulting, Engineering, and Finance.<br><br>
      <strong>Central message:</strong> "The businesses that grow fastest aren't the ones working harder on compliance — they're the ones who've built the right foundations." Position Citation as the infrastructure layer that lets mid-market businesses compete.<br><br>
      <strong>Content engine:</strong> Monthly "Workforce Risk" content — payroll accuracy, Fair Work updates, psychosocial obligations, AI policy. Powered by survey data as ongoing reference benchmarks.<br><br>
      <strong>Diagnostic hook:</strong> Compliance Maturity Benchmark → Full Workforce Risk Assessment → Consultation booking.<br><br>
      <strong>Commercial outcome:</strong> Integrated HR/payroll/compliance service packages. Estimated addressable: 204 survey respondents in this band = indicative of a large mid-market segment.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">20–100 staff</span>
      <span class="tag tag-channel">LinkedIn · Email · Search</span>
      <span class="tag tag-format">Research report · Webinar series · Diagnostic</span>
      <span class="tag tag-message">Foundation for growth, not just compliance</span>
    </div>
  </div>

  <div class="opp" style="border-left: 6px solid var(--purple);">
    <div class="opp-header">
      <div class="opp-icon opp-icon-purple" style="font-size:28px;">⚡</div>
      <div class="opp-title">
        <div class="opp-type opp-type-purple">Program 2 · Awareness &amp; Lead Gen</div>
        <h3>The "Reclaim" Program — Time recovery for the owner-operator</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>Primary audience:</strong> 5–19 employee businesses, owners and senior managers, particularly in award-dense industries (Retail, Hospitality, Education, Accounting, Infra & Construction).<br><br>
      <strong>Central message:</strong> "You're spending 40+ hours a year on compliance tasks that shouldn't be on your plate. Citation handles it — so you don't have to." Position on time recovery and personal stress reduction (66% say right support reduces stress).<br><br>
      <strong>Content engine:</strong> "5-minute compliance" content format — quick clarity on Fair Work changes, award updates, safety checklist. Mobile-first. High frequency, low friction.<br><br>
      <strong>Diagnostic hook:</strong> Compliance Time Cost Calculator → Award Complexity Checker → On-demand HR advice or payroll review CTA.<br><br>
      <strong>Commercial outcome:</strong> On-demand HR support, outsourced payroll, compliance subscription products.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">5–19 staff · Owners</span>
      <span class="tag tag-channel">LinkedIn · Email · Google Search · Meta</span>
      <span class="tag tag-format">Calculator · Short content · Award guides</span>
      <span class="tag tag-message">Reclaim your time. We carry the compliance.</span>
    </div>
  </div>

  <div class="opp" style="border-left: 6px solid var(--teal);">
    <div class="opp-header">
      <div class="opp-icon opp-icon-teal" style="font-size:28px;">🔭</div>
      <div class="opp-title">
        <div class="opp-type opp-type-teal">Program 3 · Thought Leadership</div>
        <h3>The "Frontier" Program — Emerging risk authority for the C-Suite</h3>
      </div>
    </div>
    <div class="opp-body">
      <strong>Primary audience:</strong> C-Suite and senior managers in 100+ employee businesses, particularly Technology, Finance, Consulting, and Real Estate.<br><br>
      <strong>Central message:</strong> "The workforce compliance landscape is changing faster than most businesses realise. Psychosocial risk. AI policy. Right to disconnect. Data privacy. Citation helps you stay ahead of what's coming — not just catch up to what's here."<br><br>
      <strong>Content engine:</strong> Quarterly "Frontier Risk" executive briefings — deep dives on emerging compliance areas with practical frameworks. PR-driven, conference-backed, LinkedIn-distributed.<br><br>
      <strong>Diagnostic hook:</strong> AI Workplace Readiness Audit → Psychosocial Risk Readiness Check → Strategic advisory engagement.<br><br>
      <strong>Commercial outcome:</strong> Strategic HR advisory retainers, ISO certification support, enterprise compliance partnerships.
    </div>
    <div class="tag-row">
      <span class="tag tag-audience">100+ staff · C-Suite</span>
      <span class="tag tag-channel">LinkedIn · Conference · PR · Executive email</span>
      <span class="tag tag-format">Executive briefings · Whitepaper · Roundtables</span>
      <span class="tag tag-message">Stay ahead of the compliance frontier.</span>
    </div>
  </div>

  <!-- Prioritisation matrix -->
  <div class="mt32">
    <h2 class="section-title">Prioritisation — Where to start</h2>
    <p class="section-intro">Ranked by strength of data signal, commercial proximity, and execution ease.</p>
    <table class="data-table">
      <thead><tr><th>Opportunity</th><th>Data signal strength</th><th>Audience size</th><th>Commercial proximity</th><th>Recommended priority</th></tr></thead>
      <tbody>
        <tr><td><strong>Payroll Anxiety Campaign</strong></td><td class="hi">Very strong (42% errors, 67% Fair Work)</td><td class="hi">All segments</td><td class="hi">High — direct product match</td><td class="hi">★★★★★ Start here</td></tr>
        <tr><td><strong>Time Drain Campaign</strong></td><td class="hi">Very strong (69% affected)</td><td class="hi">All segments</td><td class="md">Medium — broad awareness play</td><td class="hi">★★★★★ Start here</td></tr>
        <tr><td><strong>Psychosocial Frontier</strong></td><td class="md">Strong (77% vs 89% H&S gap)</td><td class="md">All sizes</td><td class="hi">High — regulatory urgency</td><td class="hi">★★★★☆ Near-term</td></tr>
        <tr><td><strong>Growth Blocker Campaign</strong></td><td class="md">Strong (62% affected)</td><td class="md">20–100 staff</td><td class="hi">High — brand positioning</td><td class="hi">★★★★☆ Near-term</td></tr>
        <tr><td><strong>Fragmentation / Integration</strong></td><td class="md">Strong (81% on 2+ systems)</td><td class="md">Mid-market</td><td class="md">Medium — platform play</td><td class="md">★★★☆☆ Mid-term</td></tr>
        <tr><td><strong>IR / Fair Work sector campaigns</strong></td><td class="md">Strong in specific industries</td><td class="md">Industry-specific</td><td class="hi">High — low competition</td><td class="md">★★★☆☆ Mid-term</td></tr>
        <tr><td><strong>AI &amp; Future Readiness</strong></td><td>Moderate but growing</td><td class="md">C-Suite / large</td><td class="md">Medium — longer sales cycle</td><td class="md">★★★☆☆ Mid-term</td></tr>
        <tr><td><strong>Talent &amp; Employer Brand</strong></td><td>Moderate (37% top concern)</td><td>5–19 staff</td><td class="md">Medium — iHasco tie-in</td><td>★★☆☆☆ Longer play</td></tr>
      </tbody>
    </table>
  </div>

</div>

</div><!-- /content -->

<footer>
  <div><strong>Citation Group</strong> · Workforce Risk &amp; Compliance Survey Analysis · February 2026</div>
  <div>n=510 complete responses · Fieldwork January–February 2026 · Confidential</div>
</footer>

</body>
</html>
