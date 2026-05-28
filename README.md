# gayatrigandhi.github.io
Career Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Meet Gayatri</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@2.44.0/tabler-icons.min.css">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --blue: #1B4FD8;
  --blue-light: #EEF2FF;
  --gold: #C9973A;
  --text: #111827;
  --text-secondary: #6B7280;
  --text-tertiary: #9CA3AF;
  --surface: #F9FAFB;
  --bg: #ffffff;
  --border: rgba(0,0,0,0.08);
  --radius-md: 8px;
  --radius-lg: 12px;
}

body {
  font-family: 'DM Sans', sans-serif;
  background: #F3F4F6;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem 1rem;
  color: var(--text);
}

.card {
  background: #fff;
  border-radius: 20px;
  box-shadow: 0 4px 40px rgba(0,0,0,0.08), 0 1px 4px rgba(0,0,0,0.04);
  width: 100%;
  max-width: 780px;
  padding: 2.5rem;
}

.nav {
  display: flex;
  gap: 6px;
  margin-bottom: 2.5rem;
  flex-wrap: wrap;
}

.nav-btn {
  background: none;
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 6px 14px;
  font-size: 11px;
  font-family: 'DM Sans', sans-serif;
  color: var(--text-secondary);
  cursor: pointer;
  transition: all 0.2s;
  letter-spacing: 0.05em;
  text-transform: uppercase;
}
.nav-btn.active {
  background: var(--blue);
  border-color: var(--blue);
  color: #fff;
}
.nav-btn:hover:not(.active) {
  border-color: #9CA3AF;
  color: var(--text);
}

.slide { display: none; animation: fadeIn 0.35s ease; }
.slide.visible { display: block; }
@keyframes fadeIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: translateY(0); } }

.eyebrow {
  font-size: 11px;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--gold);
  font-weight: 500;
  margin-bottom: 0.5rem;
}

.display-name {
  font-family: 'Playfair Display', serif;
  font-size: 48px;
  font-weight: 700;
  line-height: 1.1;
  color: var(--text);
  margin-bottom: 0.75rem;
}

.tagline {
  font-size: 17px;
  color: var(--text-secondary);
  font-weight: 300;
  line-height: 1.6;
  max-width: 420px;
  margin-bottom: 2rem;
}

.intro-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin-top: 2rem;
}

.intro-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius-lg);
  padding: 1.25rem;
}
.intro-card .label {
  font-size: 11px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--text-tertiary);
  margin-bottom: 8px;
}
.intro-card .value {
  font-size: 14px;
  font-weight: 500;
  color: var(--text);
  line-height: 1.5;
}

.accent-bar {
  width: 40px;
  height: 3px;
  background: var(--blue);
  border-radius: 2px;
  margin-bottom: 1.5rem;
}

.section-title {
  font-family: 'Playfair Display', serif;
  font-size: 30px;
  font-weight: 700;
  color: var(--text);
  margin-bottom: 0.5rem;
}

.timeline {
  position: relative;
  padding-left: 28px;
  margin-top: 2rem;
}
.timeline::before {
  content: '';
  position: absolute;
  left: 7px;
  top: 8px;
  bottom: 8px;
  width: 1px;
  background: var(--border);
}
.tl-item {
  position: relative;
  margin-bottom: 1.5rem;
  animation: slideIn 0.4s ease both;
}
.tl-item::before {
  content: '';
  position: absolute;
  left: -25px;
  top: 6px;
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--blue);
  border: 2px solid #fff;
  outline: 1px solid var(--blue);
}
.tl-item.current::before {
  background: var(--gold);
  outline-color: var(--gold);
  width: 10px;
  height: 10px;
  left: -26px;
  top: 5px;
}
.tl-year { font-size: 11px; color: var(--text-tertiary); letter-spacing: 0.08em; margin-bottom: 2px; }
.tl-company { font-weight: 500; font-size: 16px; color: var(--text); }
.tl-role { font-size: 13px; color: var(--text-secondary); margin-top: 2px; }
@keyframes slideIn { from { opacity: 0; transform: translateX(-8px); } to { opacity: 1; transform: translateX(0); } }

.philo-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin-top: 2rem;
}
.philo-card {
  border: 1px solid var(--border);
  border-radius: var(--radius-lg);
  padding: 1.25rem;
  background: #fff;
}
.philo-card .philo-head {
  font-size: 13px;
  font-weight: 500;
  color: var(--blue);
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 8px;
}
.philo-card .philo-head i { font-size: 18px; }
.philo-card ul { list-style: none; font-size: 13px; color: var(--text-secondary); line-height: 2; }
.philo-card ul li::before { content: '—  '; color: var(--gold); }

.stakeholder-row {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin-top: 2rem;
}
.sh-card {
  background: var(--surface);
  border: 1px solid var(--border);
  border-radius: var(--radius-lg);
  padding: 1rem 1.25rem;
  display: flex;
  align-items: center;
  gap: 12px;
  font-size: 14px;
  font-weight: 500;
}
.sh-icon {
  width: 36px;
  height: 36px;
  border-radius: 8px;
  background: var(--blue-light);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  color: var(--blue);
  font-size: 18px;
}

.toolkit-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 8px;
  margin-top: 2rem;
}
.tool-pill {
  border: 1px solid var(--border);
  border-radius: var(--radius-md);
  padding: 10px 12px;
  font-size: 12px;
  text-align: center;
  color: var(--text-secondary);
  background: var(--surface);
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
}
.tool-pill i { font-size: 15px; color: var(--blue); }

.passions-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 12px;
  margin-top: 2rem;
}
.passion-card {
  border: 1px solid var(--border);
  border-radius: var(--radius-lg);
  padding: 1.25rem 1.5rem;
  background: #fff;
  display: flex;
  align-items: center;
  gap: 16px;
}
.passion-icon {
  width: 44px;
  height: 44px;
  border-radius: 10px;
  background: var(--blue-light);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 22px;
  color: var(--blue);
  flex-shrink: 0;
}
.passion-title { font-weight: 500; font-size: 15px; }
.passion-sub { font-size: 12px; color: var(--text-secondary); margin-top: 3px; }

.case-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  font-size: 11px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--blue);
  background: var(--blue-light);
  border-radius: 20px;
  padding: 4px 12px;
  margin-bottom: 0.75rem;
}

.case-trio {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 12px;
  margin: 1.5rem 0;
}
.trio-card {
  border-radius: var(--radius-lg);
  padding: 1.25rem;
  border: 1px solid var(--border);
  background: #fff;
}
.trio-card .tc-label {
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--text-tertiary);
  margin-bottom: 8px;
}
.trio-card .tc-content { font-size: 14px; color: var(--text-secondary); line-height: 1.6; }
.trio-card.highlight { background: var(--blue); border-color: var(--blue); }
.trio-card.highlight .tc-label { color: rgba(255,255,255,0.6); }
.trio-card.highlight .tc-content { color: #fff; }

.stat-row {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin: 1.5rem 0;
}
.stat-box {
  background: var(--surface);
  border-radius: var(--radius-md);
  padding: 1rem;
  text-align: center;
}
.stat-box .sv { font-size: 26px; font-weight: 500; color: var(--blue); font-family: 'Playfair Display', serif; }
.stat-box .sl { font-size: 12px; color: var(--text-secondary); margin-top: 4px; }

.result-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 12px;
  margin-top: 1.5rem;
}
.result-card {
  border: 1px solid var(--border);
  border-radius: var(--radius-lg);
  padding: 1.25rem;
  background: #fff;
}
.result-card .rc-cat {
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--gold);
  font-weight: 500;
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 6px;
}
.result-card ul { list-style: none; font-size: 12.5px; color: var(--text-secondary); line-height: 1.9; }
.result-card ul li::before { content: '↗  '; color: var(--blue); font-size: 11px; }

.steps-flow {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1px;
  background: var(--border);
  border-radius: var(--radius-lg);
  overflow: hidden;
  margin-top: 2rem;
}
.step-cell { background: #fff; padding: 1.25rem; }
.step-cell .step-num {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  color: #E5E7EB;
  margin-bottom: 8px;
  font-weight: 700;
}
.step-cell .step-title { font-size: 13px; font-weight: 500; margin-bottom: 6px; }
.step-cell .step-desc { font-size: 12px; color: var(--text-secondary); line-height: 1.6; }

.divider { height: 1px; background: var(--border); margin: 1.5rem 0; }

.pager {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 2.5rem;
  padding-top: 1.5rem;
  border-top: 1px solid var(--border);
}
.pg-btn {
  background: none;
  border: 1px solid var(--border);
  border-radius: 20px;
  padding: 7px 18px;
  font-size: 13px;
  cursor: pointer;
  font-family: 'DM Sans', sans-serif;
  color: var(--text-secondary);
  transition: all 0.2s;
}
.pg-btn:hover { border-color: #9CA3AF; color: var(--text); }
.pg-dots { display: flex; gap: 6px; }
.dot { width: 6px; height: 6px; border-radius: 50%; background: #E5E7EB; transition: background 0.2s; }
.dot.on { background: var(--blue); }

@media (max-width: 600px) {
  .card { padding: 1.5rem; }
  .intro-grid, .philo-grid, .case-trio, .result-grid, .stat-row { grid-template-columns: 1fr; }
  .stakeholder-row { grid-template-columns: 1fr 1fr; }
  .toolkit-grid { grid-template-columns: repeat(2, 1fr); }
  .passions-grid { grid-template-columns: 1fr; }
  .steps-flow { grid-template-columns: 1fr 1fr; }
  .display-name { font-size: 34px; }
  .nav-btn { font-size: 10px; padding: 5px 10px; }
}
</style>
</head>
<body>

<div class="card">
  <nav class="nav" role="tablist">
    <button class="nav-btn active" onclick="go(0)">Intro</button>
    <button class="nav-btn" onclick="go(1)">Career</button>
    <button class="nav-btn" onclick="go(2)">Philosophy</button>
    <button class="nav-btn" onclick="go(3)">Toolkit</button>
    <button class="nav-btn" onclick="go(4)">Passions</button>
    <button class="nav-btn" onclick="go(5)">Case: Mailchimp</button>
    <button class="nav-btn" onclick="go(6)">Case: POS</button>
  </nav>

  <!-- Slide 0: Intro -->
  <div class="slide visible" id="s0">
    <div class="eyebrow">Meet</div>
    <div class="display-name">Gayatri</div>
    <div style="font-size:13px;color:var(--text-tertiary);margin-bottom:0.5rem;font-style:italic">(Guy-tree)</div>
    <p class="tagline">Building research systems that shape product strategy through mixed-methods research, behavioral insight, and systems thinking.</p>
    <div class="accent-bar"></div>
    <div class="intro-grid">
      <div class="intro-card">
        <div class="label">Experience</div>
        <div class="value">15+ years</div>
      </div>
      <div class="intro-card">
        <div class="label">Approach</div>
        <div class="value">Mixed-methods &amp; behavioral insight</div>
      </div>
      <div class="intro-card">
        <div class="label">Focus</div>
        <div class="value">Product strategy &amp; systems thinking</div>
      </div>
    </div>
    <div class="pager">
      <span></span>
      <div class="pg-dots" id="dots0"></div>
      <button class="pg-btn" onclick="go(1)">Career →</button>
    </div>
  </div>

  <!-- Slide 1: Career -->
  <div class="slide" id="s1">
    <div class="eyebrow">My career journey</div>
    <div class="section-title">From Bajaj to EQ Bank</div>
    <p style="color:var(--text-secondary);font-size:14px;margin-top:0.5rem">A trajectory through fintech, martech, and consumer banking — always anchored in research.</p>
    <div class="timeline">
      <div class="tl-item" style="animation-delay:0.05s">
        <div class="tl-year">2010</div>
        <div class="tl-company">Bajaj Auto</div>
        <div class="tl-role">Post-MBA entry into market research</div>
      </div>
      <div class="tl-item" style="animation-delay:0.1s">
        <div class="tl-year">2011</div>
        <div class="tl-company">ICICI Bank</div>
        <div class="tl-role">Consumer banking research</div>
      </div>
      <div class="tl-item" style="animation-delay:0.15s">
        <div class="tl-year">2016</div>
        <div class="tl-company">CIBC</div>
        <div class="tl-role">Digital banking &amp; product insight</div>
      </div>
      <div class="tl-item" style="animation-delay:0.2s">
        <div class="tl-year">2021</div>
        <div class="tl-company">Square</div>
        <div class="tl-role">POS &amp; fintech UX research</div>
      </div>
      <div class="tl-item" style="animation-delay:0.25s">
        <div class="tl-year">2022</div>
        <div class="tl-company">Intuit Mailchimp</div>
        <div class="tl-role">Partner program &amp; service provider research</div>
      </div>
      <div class="tl-item current" style="animation-delay:0.3s">
        <div class="tl-year">2024 — Present</div>
        <div class="tl-company">EQ Bank</div>
        <div class="tl-role">Digital-first consumer banking research</div>
      </div>
    </div>
    <div class="pager">
      <button class="pg-btn" onclick="go(0)">← Intro</button>
      <div class="pg-dots" id="dots1"></div>
      <button class="pg-btn" onclick="go(2)">Philosophy →</button>
    </div>
  </div>

  <!-- Slide 2: Philosophy -->
  <div class="slide" id="s2">
    <div class="eyebrow">Research philosophy</div>
    <div class="section-title">How I work</div>
    <div class="philo-grid">
      <div class="philo-card">
        <div class="philo-head"><i class="ti ti-zoom-question"></i> Clarity in ambiguity</div>
        <ul>
          <li>Decision-ready clarity</li>
          <li>Surface assumptions</li>
          <li>Shared mental models</li>
        </ul>
      </div>
      <div class="philo-card">
        <div class="philo-head"><i class="ti ti-topology-star-ring"></i> Systems for scale</div>
        <ul>
          <li>Reusable frameworks</li>
          <li>Insight systems</li>
          <li>Decision models</li>
        </ul>
      </div>
      <div class="philo-card">
        <div class="philo-head"><i class="ti ti-users"></i> Partnership for impact</div>
        <ul>
          <li>Early embedding</li>
          <li>User-grounded influence</li>
          <li>Translate complexity</li>
        </ul>
      </div>
    </div>
    <div class="divider"></div>
    <div class="stakeholder-row">
      <div class="sh-card"><div class="sh-icon"><i class="ti ti-speakerphone"></i></div>Integrated Marketing</div>
      <div class="sh-card"><div class="sh-icon"><i class="ti ti-map"></i></div>Product</div>
      <div class="sh-card"><div class="sh-icon"><i class="ti ti-brush"></i></div>Design</div>
      <div class="sh-card"><div class="sh-icon"><i class="ti ti-puzzle"></i></div>Strategy</div>
      <div class="sh-card"><div class="sh-icon"><i class="ti ti-headset"></i></div>Customer Success</div>
      <div class="sh-card"><div class="sh-icon"><i class="ti ti-chart-bar"></i></div>Data Science</div>
    </div>
    <div class="pager">
      <button class="pg-btn" onclick="go(1)">← Career</button>
      <div class="pg-dots" id="dots2"></div>
      <button class="pg-btn" onclick="go(3)">Toolkit →</button>
    </div>
  </div>

  <!-- Slide 3: Toolkit -->
  <div class="slide" id="s3">
    <div class="eyebrow">Methodology</div>
    <div class="section-title">The toolkit</div>
    <div class="toolkit-grid">
      <div class="tool-pill"><i class="ti ti-user"></i>In-depth interviews</div>
      <div class="tool-pill"><i class="ti ti-target"></i>Concept testing</div>
      <div class="tool-pill"><i class="ti ti-speakerphone"></i>Creative testing</div>
      <div class="tool-pill"><i class="ti ti-map-2"></i>Journey maps</div>
      <div class="tool-pill"><i class="ti ti-users"></i>Focus groups</div>
      <div class="tool-pill"><i class="ti ti-device-desktop"></i>Usability testing</div>
      <div class="tool-pill"><i class="ti ti-clipboard-list"></i>Online surveys</div>
      <div class="tool-pill"><i class="ti ti-arrows-split-2"></i>A/B testing</div>
      <div class="tool-pill"><i class="ti ti-id"></i>User personas</div>
      <div class="tool-pill"><i class="ti ti-device-laptop"></i>Digital communities</div>
      <div class="tool-pill"><i class="ti ti-layout-list"></i>Segmentations</div>
      <div class="tool-pill"><i class="ti ti-puzzle"></i>Co-creation workshops</div>
    </div>
    <div class="pager">
      <button class="pg-btn" onclick="go(2)">← Philosophy</button>
      <div class="pg-dots" id="dots3"></div>
      <button class="pg-btn" onclick="go(4)">Passions →</button>
    </div>
  </div>

  <!-- Slide 4: Passions -->
  <div class="slide" id="s4">
    <div class="eyebrow">My passions</div>
    <div class="section-title">Beyond the research brief</div>
    <div class="passions-grid">
      <div class="passion-card">
        <div class="passion-icon"><i class="ti ti-building-skyscraper"></i></div>
        <div>
          <div class="passion-title">Toronto — home base</div>
          <div class="passion-sub">Deeply rooted in the city's energy &amp; culture</div>
        </div>
      </div>
      <div class="passion-card">
        <div class="passion-icon"><i class="ti ti-needle-thread"></i></div>
        <div>
          <div class="passion-title">Crochet &amp; handcraft</div>
          <div class="passion-sub">Patience, pattern recognition — researcher skills at play</div>
        </div>
      </div>
      <div class="passion-card">
        <div class="passion-icon"><i class="ti ti-trees"></i></div>
        <div>
          <div class="passion-title">Nature &amp; the outdoors</div>
          <div class="passion-sub">Camping, forests, and recharging off-screen</div>
        </div>
      </div>
      <div class="passion-card">
        <div class="passion-icon"><i class="ti ti-heart"></i></div>
        <div>
          <div class="passion-title">Women's health advocacy</div>
          <div class="passion-sub">CIBC Run for the Cure — cancer research fundraising</div>
        </div>
      </div>
    </div>
    <div class="pager">
      <button class="pg-btn" onclick="go(3)">← Toolkit</button>
      <div class="pg-dots" id="dots4"></div>
      <button class="pg-btn" onclick="go(5)">Case Study 1 →</button>
    </div>
  </div>

  <!-- Slide 5: Case Study 1 -->
  <div class="slide" id="s5">
    <div class="case-badge"><i class="ti ti-users" style="font-size:13px"></i> Mixed methods research</div>
    <div class="section-title">Service Partner Category Exploration</div>
    <p style="font-size:14px;color:var(--text-secondary);margin:0.5rem 0 1.5rem;line-height:1.7">How can Mailchimp &amp; Co improve its partner program to drive adoption and achieve service partner-led growth, similar to its competitors?</p>
    <div class="case-trio">
      <div class="trio-card">
        <div class="tc-label">The question</div>
        <div class="tc-content">Improve partner program to drive adoption and achieve SP-led growth</div>
      </div>
      <div class="trio-card">
        <div class="tc-label">The solution</div>
        <div class="tc-content">Thorough mixed-methods research to understand the Service Provider category and identify high-value targets</div>
      </div>
      <div class="trio-card highlight">
        <div class="tc-label">The impact</div>
        <div class="tc-content">Significant increase in MC&amp;Co participants, influx of HV SMBs, improved acquisition targeting</div>
      </div>
    </div>
    <div class="divider"></div>
    <div style="font-size:12px;color:var(--text-tertiary);text-transform:uppercase;letter-spacing:0.1em;margin-bottom:12px">Competitor benchmark</div>
    <div class="stat-row">
      <div class="stat-box"><div class="sv">45%</div><div class="sl">Revenue from HubSpot Partner Solutions Program</div></div>
      <div class="stat-box"><div class="sv">33%</div><div class="sl">Customer referrals via partner channel</div></div>
      <div class="stat-box"><div class="sv">$1B</div><div class="sl">Generated annually through the partner ecosystem</div></div>
    </div>
    <div class="divider"></div>
    <div style="font-size:13px;font-weight:500;margin-bottom:12px">Key results</div>
    <div class="result-grid">
      <div class="result-card">
        <div class="rc-cat"><i class="ti ti-box" style="font-size:14px"></i> Product</div>
        <ul>
          <li>Scaled from 50k to 80k members</li>
          <li>Updated agency target lists for FFS</li>
          <li>BI typing tool became look-alike model</li>
        </ul>
      </div>
      <div class="result-card">
        <div class="rc-cat"><i class="ti ti-speakerphone" style="font-size:14px"></i> Marketing</div>
        <ul>
          <li>More personalized partner programs</li>
          <li>Higher open rates &amp; click-throughs</li>
          <li>GTM campaigns better targeted</li>
        </ul>
      </div>
      <div class="result-card">
        <div class="rc-cat"><i class="ti ti-building" style="font-size:14px"></i> Org</div>
        <ul>
          <li>Segment predictor in sign-up flow</li>
          <li>Higher stakeholder engagement</li>
          <li>Invited to consult on FY25 strategy</li>
        </ul>
      </div>
    </div>
    <div class="pager">
      <button class="pg-btn" onclick="go(4)">← Passions</button>
      <div class="pg-dots" id="dots5"></div>
      <button class="pg-btn" onclick="go(6)">Case Study 2 →</button>
    </div>
  </div>

  <!-- Slide 6: Case Study 2 -->
  <div class="slide" id="s6">
    <div class="case-badge"><i class="ti ti-device-desktop" style="font-size:13px"></i> Qualitative + usability research</div>
    <div class="section-title">POS Bundling Solutions</div>
    <p style="font-size:14px;color:var(--text-secondary);margin:0.5rem 0 1.5rem;line-height:1.7">Offering bundling for EU markets required a major redesign — a web-based flow that could take up to 34 engineering weeks, expanding checkout from 6 to 15 steps.</p>
    <div class="steps-flow">
      <div class="step-cell">
        <div class="step-num">01</div>
        <div class="step-title">Tiger team setup</div>
        <div class="step-desc">Cross-functional squad aligned on goals, constraints, and decision criteria</div>
      </div>
      <div class="step-cell">
        <div class="step-num">02</div>
        <div class="step-title">Rapid design loop</div>
        <div class="step-desc">Daily stand-ups, design variants reviewed, feasibility unblocked</div>
      </div>
      <div class="step-cell">
        <div class="step-num">03</div>
        <div class="step-title">Research prep</div>
        <div class="step-desc">Hypothesis-driven guide built, refined with tiger team input</div>
      </div>
      <div class="step-cell">
        <div class="step-num">04</div>
        <div class="step-title">Interviews &amp; walkthroughs</div>
        <div class="step-desc">12 moderated UT sessions via Figma screenshare, UK/IRE participants</div>
      </div>
      <div class="step-cell">
        <div class="step-num">05</div>
        <div class="step-title">Insight co-creation</div>
        <div class="step-desc">FigJam theme mapping + brainstorming session to co-interpret findings</div>
      </div>
      <div class="step-cell">
        <div class="step-num">06</div>
        <div class="step-title">Final path alignment</div>
        <div class="step-desc">Insights + design + feasibility → optimized path with cross-functional buy-in</div>
      </div>
    </div>
    <div class="divider"></div>
    <div class="result-grid">
      <div class="result-card">
        <div class="rc-cat"><i class="ti ti-bolt" style="font-size:14px"></i> Efficiency</div>
        <ul>
          <li>Future playbook for balancing UX with dev effort</li>
        </ul>
      </div>
      <div class="result-card">
        <div class="rc-cat"><i class="ti ti-coin" style="font-size:14px"></i> Resources</div>
        <ul>
          <li>Team avoided a flow leading to poor UX and low conversions</li>
        </ul>
      </div>
      <div class="result-card">
        <div class="rc-cat"><i class="ti ti-file-description" style="font-size:14px"></i> Documentation</div>
        <ul>
          <li>Historical record created for future similar scenarios</li>
        </ul>
      </div>
    </div>
    <div class="pager">
      <button class="pg-btn" onclick="go(5)">← Case Study 1</button>
      <div class="pg-dots" id="dots6"></div>
      <button class="pg-btn" onclick="go(0)">↩ Start over</button>
    </div>
  </div>

</div>

<script>
const total = 7;
let cur = 0;

function go(n) {
  document.querySelectorAll('.slide').forEach((s, i) => {
    s.classList.toggle('visible', i === n);
  });
  document.querySelectorAll('.nav-btn').forEach((b, i) => {
    b.classList.toggle('active', i === n);
  });
  for (let i = 0; i < total; i++) {
    const el = document.getElementById('dots' + i);
    if (el) {
      el.innerHTML = Array.from({length: total}, (_, j) =>
        `<div class="dot${j === n ? ' on' : ''}"></div>`
      ).join('');
    }
  }
  cur = n;
  window.scrollTo({ top: 0, behavior: 'smooth' });
}

go(0);
</script>
</body>
</html>
