[index.html](https://github.com/user-attachments/files/31165000/index.html)
# Portfolio<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kazem (Farhad) Kondori — Warehouse &amp; Distribution Operations Leader</title>
<style>
  :root{
    --ink:#1B1F23;
    --panel:#23282D;
    --panel-2:#2B3137;
    --paper:#F3F1EA;
    --paper-dim:#E7E3D8;
    --amber:#E8A33D;
    --amber-dim:#C98A2E;
    --teal:#3E8E7E;
    --steel:#8A94A0;
    --steel-dark:#5B646E;
    --line: rgba(243,241,234,0.14);
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--ink);
    color:var(--paper);
    font-family:'Helvetica Neue', Arial, sans-serif;
    -webkit-font-smoothing:antialiased;
    line-height:1.55;
  }
  .mono{ font-family:'Courier New', 'Consolas', monospace; }
  .display{ font-family:'Arial Narrow', 'Helvetica Neue Condensed', Impact, sans-serif; text-transform:uppercase; letter-spacing:.03em; }

  a{ color:var(--amber); text-decoration:none; }
  a:hover{ text-decoration:underline; }

  .wrap{ max-width:920px; margin:0 auto; padding:0 32px; }

  /* ===== HEADER / MANIFEST STRIP ===== */
  header{
    background:
      repeating-linear-gradient(135deg, rgba(232,163,61,0.10) 0px, rgba(232,163,61,0.10) 14px, transparent 14px, transparent 28px),
      var(--panel);
    border-bottom:3px solid var(--amber);
    padding:38px 0 30px;
  }
  .manifest-id{
    font-size:11px;
    letter-spacing:.14em;
    color:var(--steel);
    display:flex;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:8px;
    margin-bottom:22px;
    padding-bottom:14px;
    border-bottom:1px dashed var(--line);
  }
  .manifest-id span b{ color:var(--amber); font-weight:600; }

  .name-block h1{
    font-size:44px;
    font-weight:600;
    letter-spacing:.01em;
    margin:0 0 6px;
    color:var(--paper);
  }
  .role-line{
    font-size:15px;
    letter-spacing:.06em;
    color:var(--amber);
    font-weight:500;
    text-transform:uppercase;
    margin-bottom:18px;
  }
  .contact-row{
    display:flex;
    flex-wrap:wrap;
    gap:18px;
    font-size:13px;
    color:var(--steel);
  }
  .contact-row a{ color:var(--paper); }
  .contact-row .sep{ color:var(--steel-dark); }

  /* ===== RATING PLATE STATS ===== */
  .plate-section{ padding:40px 0 10px; }
  .plate-grid{
    display:flex;
    flex-wrap:wrap;
    gap:14px;
  }
  .plate{
    flex:1 1 150px;
    position:relative;
    background:linear-gradient(160deg, var(--panel-2), var(--panel));
    border:1px solid var(--line);
    border-radius:6px;
    padding:18px 16px 16px;
  }
  .plate::before, .plate::after{
    content:"";
    position:absolute;
    width:6px; height:6px;
    border-radius:50%;
    background:var(--steel-dark);
    box-shadow: inset 0 1px 1px rgba(0,0,0,.5), 0 0 0 1px rgba(243,241,234,0.06);
    top:8px;
  }
  .plate::before{ left:8px; }
  .plate::after{ right:8px; }
  .plate .rivet-b{ position:absolute; width:6px; height:6px; border-radius:50%; background:var(--steel-dark); bottom:8px; box-shadow: inset 0 1px 1px rgba(0,0,0,.5); }
  .plate .rivet-bl{ left:8px; }
  .plate .rivet-br{ right:8px; }
  .plate-label{
    font-size:10px;
    letter-spacing:.12em;
    color:var(--steel);
    margin-bottom:8px;
  }
  .plate-value{
    font-family:'Arial Narrow', 'Helvetica Neue Condensed', Impact, sans-serif; letter-spacing:.02em;
    font-size:30px;
    font-weight:600;
    color:var(--amber);
    line-height:1;
  }
  .plate-sub{
    font-size:11px;
    color:var(--steel);
    margin-top:6px;
  }

  /* ===== ZONE SECTIONS ===== */
  .zone{ padding:46px 0; border-top:1px solid var(--line); }
  .zone-head{
    display:flex;
    align-items:baseline;
    gap:14px;
    margin-bottom:22px;
  }
  .zone-num{
    font-family:'Arial Narrow', 'Helvetica Neue Condensed', Impact, sans-serif; letter-spacing:.02em;
    font-size:13px;
    color:var(--ink);
    background:var(--amber);
    padding:4px 10px;
    border-radius:3px;
    letter-spacing:.06em;
    font-weight:600;
  }
  .zone-title{
    font-family:'Arial Narrow', 'Helvetica Neue Condensed', Impact, sans-serif; letter-spacing:.02em;
    font-size:22px;
    letter-spacing:.03em;
    color:var(--paper);
  }

  .summary-text{
    font-size:15.5px;
    color:#DAD7CC;
    max-width:760px;
  }

  /* skill chips */
  .chip-row{ display:flex; flex-wrap:wrap; gap:8px; margin-top:6px; }
  .chip{
    font-family:'Courier New', 'Consolas', monospace;
    font-size:11.5px;
    color:var(--paper);
    background:var(--panel-2);
    border:1px solid var(--line);
    border-left:3px solid var(--teal);
    padding:6px 10px;
    border-radius:3px;
    letter-spacing:.02em;
  }

  /* experience log */
  .log-entry{
    display:flex;
    gap:20px;
    padding:20px 0;
    border-top:1px solid var(--line);
  }
  .log-entry:first-child{ border-top:none; padding-top:0; }
  .log-dock{
    flex:0 0 74px;
    text-align:center;
  }
  .dock-badge{
    font-family:'Arial Narrow', 'Helvetica Neue Condensed', Impact, sans-serif; letter-spacing:.02em;
    font-size:11px;
    color:var(--steel);
    letter-spacing:.08em;
  }
  .dock-badge b{
    display:block;
    font-size:26px;
    color:var(--amber);
    line-height:1.1;
  }
  .log-body{ flex:1; min-width:0; }
  .log-title-row{
    display:flex;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:6px;
    margin-bottom:2px;
  }
  .log-title{
    font-size:16.5px;
    font-weight:600;
    color:var(--paper);
  }
  .log-date{
    font-family:'Courier New', 'Consolas', monospace;
    font-size:12px;
    color:var(--amber-dim);
    white-space:nowrap;
  }
  .log-org{
    font-size:12.5px;
    color:var(--steel);
    font-style:italic;
    margin-bottom:10px;
  }
  .log-body ul{
    margin:0;
    padding-left:18px;
    color:#CFCCC1;
    font-size:14px;
  }
  .log-body li{ margin-bottom:6px; }
  .log-body li::marker{ color:var(--teal); }

  /* certifications */
  .cert-grid{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
  }
  .cert-tag{
    font-family:'Courier New', 'Consolas', monospace;
    font-size:12px;
    color:var(--ink);
    background:var(--paper-dim);
    padding:7px 12px;
    border-radius:3px;
    font-weight:500;
  }

  /* footer */
  footer{
    background:var(--panel);
    border-top:3px solid var(--amber);
    padding:34px 0 30px;
    text-align:center;
  }
  footer .fline{
    font-family:'Arial Narrow', 'Helvetica Neue Condensed', Impact, sans-serif; letter-spacing:.02em;
    font-size:18px;
    color:var(--paper);
    margin-bottom:10px;
    letter-spacing:.02em;
  }
  footer .fcontacts{
    font-size:13px;
    color:var(--steel);
  }
  footer .fcontacts a{ color:var(--amber); }
  footer .fnote{
    margin-top:16px;
    font-size:11px;
    color:var(--steel-dark);
    letter-spacing:.04em;
  }

  @media (max-width:640px){
    .wrap{ padding:0 20px; }
    .name-block h1{ font-size:32px; }
    .plate-grid{ gap:10px; }
    .plate{ flex:1 1 120px; }
    .log-entry{ gap:12px; }
    .log-dock{ flex:0 0 50px; }
    .dock-badge b{ font-size:20px; }
  }

  @media print{
    body{ background:var(--ink) !important; -webkit-print-color-adjust:exact; print-color-adjust:exact; }
  }
</style>
</head>
<body>

<header>
  <div class="wrap">
    <div class="manifest-id mono">
      <span>PORTFOLIO REF: <b>KFK-2026-WM</b></span>
      <span>ISSUED: <b>AUG 2026</b></span>
      <span>STATUS: <b>ACTIVELY SEEKING</b></span>
    </div>
    <div class="name-block">
      <h1>Kazem (Farhad) Kondori</h1>
      <div class="role-line">Warehouse, Facilities &amp; Distribution Operations Leader</div>
      <div class="contact-row mono">
        <span>North York, ON</span>
        <span class="sep">/</span>
        <a href="tel:+16477709017">647-770-9017</a>
        <span class="sep">/</span>
        <a href="mailto:farhad.kondori@gmail.com">farhad.kondori@gmail.com</a>
        <span class="sep">/</span>
        <a href="https://linkedin.com/in/kazem-kondori-053225245" target="_blank" rel="noopener">linkedin.com/in/kazem-kondori-053225245</a>
      </div>
    </div>
  </div>
</header>

<section class="plate-section">
  <div class="wrap">
    <div class="plate-grid">
      <div class="plate">
        <span class="rivet-b rivet-bl"></span><span class="rivet-b rivet-br"></span>
        <div class="plate-label mono">INVENTORY ACCURACY</div>
        <div class="plate-value">98%</div>
        <div class="plate-sub">sustained via disciplined cycle counts</div>
      </div>
      <div class="plate">
        <span class="rivet-b rivet-bl"></span><span class="rivet-b rivet-br"></span>
        <div class="plate-label mono">EFFICIENCY GAIN</div>
        <div class="plate-value">30%</div>
        <div class="plate-sub">from layout &amp; workflow redesign</div>
      </div>
      <div class="plate">
        <span class="rivet-b rivet-bl"></span><span class="rivet-b rivet-br"></span>
        <div class="plate-label mono">TEAM LED</div>
        <div class="plate-value">25+</div>
        <div class="plate-sub">full-time &amp; seasonal, two shifts</div>
      </div>
      <div class="plate">
        <span class="rivet-b rivet-bl"></span><span class="rivet-b rivet-br"></span>
        <div class="plate-label mono">DUAL SCOPE</div>
        <div class="plate-value" style="font-size:22px;">Warehouse<br>+ Facilities</div>
        <div class="plate-sub">HVAC, electrical, cold rooms, generators</div>
      </div>
      <div class="plate">
        <span class="rivet-b rivet-bl"></span><span class="rivet-b rivet-br"></span>
        <div class="plate-label mono">RECOGNITION</div>
        <div class="plate-value" style="font-size:20px;">CHFA<br>Award '24</div>
        <div class="plate-sub">Best Brand — highest customer satisfaction</div>
      </div>
    </div>
  </div>
</section>

<section class="zone">
  <div class="wrap">
    <div class="zone-head">
      <span class="zone-num">ZONE 1</span>
      <span class="zone-title display">Operations Summary</span>
    </div>
    <p class="summary-text">
      Warehouse, Facilities, and Distribution Leader with 10+ years across logistics, fulfillment, inventory
      control, and building operations, including 6+ years in dual-scope supervisory and management roles
      directing two-shift, multi-facility teams of up to 25+ staff. Held full facility management responsibility
      alongside warehouse operations — building infrastructure (HVAC, electrical, plumbing, cold rooms, generators),
      contractor sourcing and cost control, equipment maintenance records, and carrier/dispatch coordination.
      Direct QA sampling experience coordinating with Quality Assurance and external labs. Proven record of
      building a culture of safety, accountability, and continuous improvement — translating hands-on floor
      leadership into measurable results in inventory accuracy, throughput, and cost control. Fluent in SAP ERP,
      WMS platforms, EDI transactions, and KPI-driven decision-making, with direct experience shaping in-house
      system requirements. Currently active as an independent warehouse operations consultant.
    </p>
    <div class="chip-row">
      <span class="chip">SAP ERP</span>
      <span class="chip">ADVANCEPRO</span>
      <span class="chip">DATA NINJA WMS</span>
      <span class="chip">EDI 856 ASN</span>
      <span class="chip">CYCLE COUNTING</span>
      <span class="chip">KPI REPORTING</span>
      <span class="chip">FACILITIES & INFRASTRUCTURE</span>
      <span class="chip">CONTRACTOR & VENDOR MGMT</span>
      <span class="chip">QA SAMPLING & LAB COORDINATION</span>
      <span class="chip">LEAN / CONTINUOUS IMPROVEMENT</span>
      <span class="chip">OHSA / WHMIS</span>
    </div>
  </div>
</section>

<section class="zone">
  <div class="wrap">
    <div class="zone-head">
      <span class="zone-num">ZONE 2</span>
      <span class="zone-title display">Experience Log</span>
    </div>

    <div class="log-entry">
      <div class="log-dock">
        <span class="dock-badge">DOOR<b>05</b></span>
      </div>
      <div class="log-body">
        <div class="log-title-row">
          <span class="log-title">Independent Consultant — Warehouse Operations &amp; Supply Chain</span>
          <span class="log-date">FEB 2025 — PRESENT</span>
        </div>
        <div class="log-org">Saturn Maple Inc. · Ontario · Part-Time / Advisory</div>
        <ul>
          <li>Redesigned a compact, narrow warehouse layout to maximize machinery placement and racking capacity.</li>
          <li>Sourced cost-competitive equipment and packaging suppliers, and advised on health &amp; safety protocols where none previously existed.</li>
          <li>Ongoing technical advisory on equipment decisions — e.g. recommending a used electric reach truck over a propane forklift for a low-ventilation space.</li>
        </ul>
      </div>
    </div>

    <div class="log-entry">
      <div class="log-dock">
        <span class="dock-badge">DOOR<b>04</b></span>
      </div>
      <div class="log-body">
        <div class="log-title-row">
          <span class="log-title">Assistant Warehouse Manager / Facility Manager</span>
          <span class="log-date">MAR 2018 — NOV 2024</span>
        </div>
        <div class="log-org">CanPrev Natural Health Products · Scarborough, ON</div>
        <ul>
          <li>Held dual responsibility for warehouse operations and full facility management across two buildings (80,000 + 45,000 sq ft), leading a team of 25+ full-time and seasonal staff supporting 900+ SKUs and ~500 orders/day.</li>
          <li>Managed all building infrastructure — HVAC, plumbing, electrical, lighting, cold rooms, and generators — sourcing contractors through competitive quoting to control cost while maintaining service quality.</li>
          <li>Coordinated pickup/delivery scheduling with carrier and trucking dispatch; personally drove rental trucks across the GTA for pickups and deliveries. Maintained inspection and maintenance records for forklifts, reach trucks, and pallet jacks.</li>
          <li>Worked directly with Quality Assurance, pulling QC samples from received goods and coordinating lab testing and documentation.</li>
          <li>Maintained ~98% inventory accuracy through disciplined SAP ERP/WMS transactions and root-cause investigation of discrepancies.</li>
          <li>Contributed functional requirements to CanPrev's in-house WMS build ("Kinetics"), focused on automating and speeding up receiving.</li>
          <li>Redesigned warehouse layout and standardized procedures — a 30% efficiency improvement.</li>
          <li>Recruited, trained, and coached two shift supervisors and their associates, handling performance management and disciplinary matters; fulfillment speed helped drive CanPrev's CHFA Best Brand Award (Sep 2024) for highest customer satisfaction.</li>
        </ul>
      </div>
    </div>

    <div class="log-entry">
      <div class="log-dock">
        <span class="dock-badge">DOOR<b>03</b></span>
      </div>
      <div class="log-body">
        <div class="log-title-row">
          <span class="log-title">Warehouse Supervisor</span>
          <span class="log-date">MAY 2016 — FEB 2018</span>
        </div>
        <div class="log-org">CanPrev Natural Health Products · Scarborough, ON</div>
        <ul>
          <li>Supervised a team of 10 across receiving, picking, replenishment, and shipping.</li>
          <li>Supported inventory accuracy through cycle counts and ERP transaction auditing; trained staff on procedures and safety.</li>
        </ul>
      </div>
    </div>

    <div class="log-entry">
      <div class="log-dock">
        <span class="dock-badge">DOOR<b>02</b></span>
      </div>
      <div class="log-body">
        <div class="log-title-row">
          <span class="log-title">Warehouse &amp; Inventory Coordinator</span>
          <span class="log-date">JAN 2012 — SEP 2015</span>
        </div>
        <div class="log-org">Net Gostaran Pouya Inc. · Tehran, Iran</div>
        <ul>
          <li>Managed inventory records, stock movement, and documentation; coordinated receiving/shipping and maintained an organized warehouse layout.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section class="zone">
  <div class="wrap">
    <div class="zone-head">
      <span class="zone-num">ZONE 3</span>
      <span class="zone-title display">Education &amp; Certifications</span>
    </div>
    <div class="cert-grid">
      <span class="cert-tag">B.A. — Statistics</span>
      <span class="cert-tag">MCSE</span>
      <span class="cert-tag">Supply Chain Mgmt Certificate — Rutgers University</span>
      <span class="cert-tag">Forklift Certification</span>
      <span class="cert-tag">ISO 9001</span>
      <span class="cert-tag">GMP</span>
      <span class="cert-tag">Lean Fundamentals</span>
      <span class="cert-tag">WHMIS</span>
    </div>
  </div>
</section>

<footer>
  <div class="wrap">
    <div class="fline display">Let's talk operations.</div>
    <div class="fcontacts mono">
      <a href="mailto:farhad.kondori@gmail.com">farhad.kondori@gmail.com</a>
      &nbsp;·&nbsp; 647-770-9017
      &nbsp;·&nbsp;
      <a href="https://linkedin.com/in/kazem-kondori-053225245" target="_blank" rel="noopener">LinkedIn</a>
    </div>
    <div class="fnote mono">ALL METRICS VERIFIED · CANPREV NATURAL HEALTH PRODUCTS &amp; SATURN MAPLE INC.</div>
  </div>
</footer>

</body>
</html>
