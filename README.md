<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Chamod Dhananjaya – Software Engineering Undergraduate CV</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@500;600;700&family=Source+Sans+3:wght@400;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --acc:#1f4e8c; --navy:#14284b; --soft:#e6eef9; --softtext:#1b4b82;
    --ink:#1c2633; --muted:#5d6b7b; --rule:#d9e0e8; --bg:#e6eaef;
    --head:'Outfit','Segoe UI',Arial,sans-serif; --body:'Source Sans 3',Calibri,Arial,sans-serif;
  }
  [data-theme="charcoal"]{--acc:#4a5360; --navy:#26292e; --soft:#eceef1; --softtext:#2f343a}
  [data-theme="forest"]{--acc:#2f7a5b; --navy:#17382d; --soft:#e2f2ea; --softtext:#1d5740}
  [data-theme="burgundy"]{--acc:#9a2f4a; --navy:#4a1523; --soft:#f8e7ec; --softtext:#7a2238}

  *{box-sizing:border-box;-webkit-print-color-adjust:exact;print-color-adjust:exact}
  body{margin:0;background:var(--bg);font-family:var(--body);color:var(--ink);font-size:10pt;line-height:1.45}

  .bar{max-width:210mm;margin:16px auto 0;padding:0 8px;display:flex;flex-wrap:wrap;justify-content:space-between;align-items:center;gap:10px 14px;font-size:13px;color:var(--muted)}
  .themes{display:flex;align-items:center;gap:8px}
  .themes button{width:26px;height:26px;border-radius:50%;border:2px solid #fff;box-shadow:0 0 0 1px #aab4c0;cursor:pointer;padding:0}
  .themes button[aria-pressed="true"]{box-shadow:0 0 0 3px var(--acc)}
  .themes button:focus-visible,.pdf:focus-visible{outline:3px solid #8fb8de;outline-offset:2px}
  .pdf{font:inherit;font-weight:600;background:var(--navy);color:#fff;border:0;border-radius:6px;padding:8px 14px;cursor:pointer}
  [contenteditable]:focus{outline:2px dashed #8fb8de;outline-offset:2px}

  .page{width:210mm;min-height:297mm;margin:12px auto 32px;background:#fff;padding:14mm 16mm 12mm;box-shadow:0 2px 14px rgba(15,34,56,.2)}

  /* Header with Profile Photo */
  header{
    padding-bottom:11px;
    border-bottom:3px solid var(--acc);
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:16px;
  }
  .header-info{flex:1}
  .avatar{
    width:86px;
    height:86px;
    border-radius:50%;
    object-fit:cover;
    border:3px solid var(--acc);
    box-shadow:0 2px 8px rgba(0,0,0,.12);
    flex-shrink:0;
    background:var(--soft);
  }

  h1{font-family:var(--head);font-weight:700;font-size:25pt;line-height:1.1;margin:0;color:var(--navy);letter-spacing:-.01em}
  .role{margin:3px 0 8px;font-family:var(--head);font-weight:500;font-size:12pt;color:var(--acc)}
  .contact{list-style:none;margin:0;padding:0;display:flex;flex-wrap:wrap;gap:2px 16px;font-size:9.5pt}
  .contact li{margin:0}
  .contact b{color:var(--muted);font-weight:600}
  .contact a{color:var(--ink);text-decoration:none}
  .contact a:hover{text-decoration:underline;color:var(--acc)}

  section{padding-top:11px}
  h2{font-family:var(--head);font-weight:600;font-size:11.5pt;margin:0 0 6px;color:var(--navy);padding-left:8px;border-left:4px solid var(--acc);line-height:1.2}
  p{margin:0}
  ul{margin:3px 0 0;padding-left:16px}
  li{margin-bottom:2px}
  .entry{margin-bottom:9px;break-inside:avoid}
  .entry:last-child{margin-bottom:0}
  .head{display:flex;justify-content:space-between;gap:12px;align-items:baseline}
  .head strong{font-family:var(--head);font-weight:600;font-size:10.8pt;color:var(--navy)}
  .date{color:var(--muted);font-size:9.3pt;white-space:nowrap}
  .sub{color:var(--acc);font-weight:600;margin:0 0 2px;font-size:9.8pt}
  .tech{margin-top:3px;font-size:9.3pt;color:var(--muted)}
  .tech b{color:var(--softtext)}

  .skills{display:grid;grid-template-columns:36mm 1fr;gap:3px 10px;margin:0}
  .skills dt{font-weight:700;color:var(--navy)}
  .skills dd{margin:0}
  .small{font-size:9.5pt;color:var(--muted)}

  @media (max-width:760px){
    .page{width:auto;margin:8px;padding:18px}
    header{flex-direction:column-reverse;align-items:flex-start}
    .avatar{width:76px;height:76px}
    .head{flex-direction:column;gap:0}
    .skills{grid-template-columns:1fr;gap:0}
    .skills dd{margin-bottom:5px}
  }
  @media print{
    @page{size:A4;margin:0}
    body{background:#fff}
    .bar{display:none}
    .page{margin:0;box-shadow:none;width:210mm;min-height:297mm}
    [contenteditable]:focus{outline:0}
  }
</style>
</head>
<body>

<div class="bar">
  <div class="themes" role="group" aria-label="Colour theme">
    <span>Colour:</span>
    <button type="button" data-t="navy" aria-label="Corporate Navy" title="Corporate Navy" style="background:#14284b" aria-pressed="true"></button>
    <button type="button" data-t="charcoal" aria-label="Executive Charcoal" title="Executive Charcoal" style="background:#26292e" aria-pressed="false"></button>
    <button type="button" data-t="forest" aria-label="Forest Green" title="Forest Green" style="background:#17382d" aria-pressed="false"></button>
    <button type="button" data-t="burgundy" aria-label="Deep Burgundy" title="Deep Burgundy" style="background:#4a1523" aria-pressed="false"></button>
  </div>
  <span>Click text to edit.</span>
  <button class="pdf" type="button" onclick="window.print()">Save as PDF</button>
</div>

<main class="page" contenteditable="true" spellcheck="false">

  <header>
    <div class="header-info">
      <h1>Chamod Dhananjaya</h1>
      <p class="role">Software Engineering Undergraduate</p>
      <ul class="contact">
        <li><b>Phone</b> 076 961 1178</li>
        <li><b>Email</b> <a href="mailto:chamoddhananjaya76@gmail.com">chamoddhananjaya76@gmail.com</a></li>
        <li><b>Location</b> Hirikuluwa, Muddaragama</li>
        <li><b>GitHub</b> <a href="https://github.com/chamoddhananjaya810" target="_blank" rel="noopener">github.com/chamoddhananjaya810</a></li>
        <li><b>Portfolio</b> <a href="https://chamod-dhananjaya.vercel.app" target="_blank" rel="noopener">chamod-dhananjaya.vercel.app</a></li>
      </ul>
    </div>
    <img class="avatar" src="https://github.com/chamoddhananjaya810.png" alt="Chamod Dhananjaya" onerror="this.style.display='none'">
  </header>

  <section>
    <h2>Profile</h2>
    <p>Software Engineering undergraduate reading for a BSc (Hons) at Birmingham City University through Java Institute, with a UK-awarded Diploma and HND in Software Engineering. Has built full-stack web applications and cross-platform mobile apps using Laravel, React, Flutter and Firebase. Strong in backend architecture, database management and enterprise systems integration, with working knowledge of modern DevOps practices (Docker &amp; Kubernetes).</p>
  </section>

  <section>
    <h2>Technical skills</h2>
    <dl class="skills">
      <dt>Backend &amp; languages</dt><dd>Java, Jakarta EE, Java Servlets, PHP, Laravel, Spring Boot, Hibernate, Python, PostgreSQL, MySQL, Firebase, MongoDB, SQLite, Microservices, RESTful APIs</dd>
      <dt>Frontend &amp; mobile</dt><dd>HTML5, CSS3, JavaScript, TypeScript, React, React Native, Angular, Flutter, Dart, Tailwind CSS, Bootstrap, XML, Android</dd>
      <dt>Architecture &amp; DevOps</dt><dd>MVC architecture, Git / GitHub, Docker, Kubernetes, Payara, Ubuntu</dd>
      <dt>Testing &amp; tools</dt><dd>Postman (API testing), Unit testing, IntelliJ IDEA, Android Studio</dd>
      <dt>Currently learning</dt><dd>Containerized microservices, DevOps pipelines &amp; OOD patterns</dd>
    </dl>
  </section>

  <section>
    <h2>Projects</h2>

    <div class="entry">
      <div class="head"><strong>Aswanu – Agricultural marketplace (inventory and order tracking)</strong></div>
      <ul>
        <li>Built a marketplace that connects local farmers and buyers directly, without middlemen.</li>
        <li>Developed the buyer mobile app with Android and Firebase, and the admin/seller web panel with React and Firebase.</li>
        <li>Added real-time order tracking, dynamic pricing, and Google Maps API integration for distance and shipping cost calculation.</li>
      </ul>
      <p class="tech"><b>Tech:</b> Android, React, Firebase, Google Maps API</p>
    </div>

    <div class="entry">
      <div class="head"><strong>SmartRetail – POS, repair and financial comparison system</strong></div>
      <ul>
        <li>Developed a cross-platform point-of-sale and repair management system with a Laravel backend and Flutter app.</li>
        <li>Managed store inventory, sales, and repair workflows where items are logged, assigned to technicians and tracked to completion.</li>
        <li>Built dashboards for inventory, sales and stock management, plus monthly and yearly income-versus-expense comparisons.</li>
      </ul>
      <p class="tech"><b>Tech:</b> Laravel, Flutter, MySQL, REST API</p>
    </div>

    <div class="entry">
      <div class="head"><strong>Smart Railway – Train ticket fraud prevention system</strong></div>
      <ul>
        <li>Built a software solution to address train ticket fraud, a real problem faced by the railway department.</li>
        <li>Developed the data layer with Hibernate (ORM) and Java Servlets for reliable ticket and booking data management.</li>
      </ul>
      <p class="tech"><b>Tech:</b> Java, Servlets, Hibernate, MySQL</p>
    </div>
  </section>

  <section>
    <h2>Research</h2>
    <div class="entry">
      <div class="head"><strong>Object-Oriented Design Patterns</strong><span class="date">Ongoing</span></div>
      <ul>
        <li>Currently researching and studying object-oriented design (OOD) patterns and how they improve the structure and maintainability of software systems.</li>
      </ul>
    </div>
  </section>

  <section>
    <h2>Education</h2>
    <div class="entry">
      <div class="head"><strong>BSc (Hons) in Software Engineering</strong><span class="date">2026 – 2027 (ongoing)</span></div>
      <p class="sub">Birmingham City University, via Java Institute</p>
    </div>
    <div class="entry">
      <div class="head"><strong>Higher National Diploma (HND) in Software Engineering</strong><span class="date">2025</span></div>
      <p class="sub">UK-awarded qualification, via Java Institute</p>
    </div>
    <div class="entry">
      <div class="head"><strong>G.C.E. Advanced Level</strong><span class="date">2021</span></div>
      <p class="small">Buddhist Civilization (B), Media (C), ICT (S)</p>
    </div>
    <div class="entry">
      <div class="head"><strong>G.C.E. Ordinary Level</strong><span class="date">2018</span></div>
      <p class="small">Buddhism (B), History (B), Mathematics (C), English (C), ICT (C), Science (C), Sinhala (C), Drama (C), Geography (S)</p>
    </div>
  </section>

  <section>
    <h2>Soft skills</h2>
    <p>Problem solving · Backend architecture and logic · System design · System management · Inventory management · Time management · Adaptability to new technology</p>
  </section>

</main>

<script>
  var btns = document.querySelectorAll('.themes button');
  btns.forEach(function(b){
    b.addEventListener('click', function(){
      var t = b.getAttribute('data-t');
      if (t === 'navy') document.documentElement.removeAttribute('data-theme');
      else document.documentElement.setAttribute('data-theme', t);
      btns.forEach(function(x){ x.setAttribute('aria-pressed', x === b ? 'true' : 'false'); });
    });
  });
</script>
</body>
</html>
