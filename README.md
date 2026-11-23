<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Amna Ghafoor | Computer Science Graduate</title>
<meta name="description" content="Computer Science graduate with SQL, Python and data experience. Portfolio and CV.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=Manrope:wght@400;500;700&display=swap" rel="stylesheet">
<style>
:root{
  --maroon:#2a0008; --maroon-2:#3d0a14; --pink:#ecc5c0; --cream:#fdfbe0; --sage:#dcdbb5;
  --serif:"Instrument Serif",Georgia,"Times New Roman",serif;
  --sans:"Manrope",system-ui,-apple-system,"Segoe UI",Arial,sans-serif;
}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth}
body{background:var(--maroon);color:var(--cream);font-family:var(--sans);line-height:1.65;font-size:17px}
a{color:inherit}
:focus-visible{outline:3px solid var(--pink);outline-offset:3px}
.wrap{max-width:1080px;margin:0 auto;padding:0 24px}
section{padding:88px 0;position:relative}
h1,h2,h3{font-family:var(--serif);font-weight:400;line-height:1}
h2{font-size:clamp(44px,7vw,76px);margin-bottom:36px}
h2 em{color:var(--pink)}
.pill{display:inline-block;background:var(--pink);color:var(--maroon);padding:6px 18px;border-radius:999px;font-size:14px;font-weight:700}
.dot{position:absolute;border-radius:50%;background:var(--sage);opacity:.9;pointer-events:none}

nav{position:sticky;top:0;z-index:5;background:rgba(42,0,8,.92);backdrop-filter:blur(6px)}
nav .wrap{display:flex;gap:22px;align-items:center;justify-content:space-between;padding-top:14px;padding-bottom:14px}
nav ul{display:flex;gap:20px;list-style:none;padding:0;flex-wrap:wrap}
nav a{text-decoration:none;font-size:14px;font-weight:500}
nav a:hover{color:var(--pink)}
.brand{font-family:var(--serif);font-size:24px}

/* hero */
.hero{padding-top:72px;overflow:hidden}
.hero-grid{display:grid;grid-template-columns:1.5fr 1fr;gap:48px;align-items:center}
.hero h1{font-size:clamp(64px,11vw,138px);color:var(--pink)}
.hero h1 span{display:block;font-style:italic;color:var(--cream)}
.hero p.lead{max-width:540px;margin:28px 0;font-size:19px}
.btns{display:flex;gap:12px;flex-wrap:wrap}
.btn{display:inline-block;padding:13px 26px;border-radius:999px;text-decoration:none;font-weight:700;font-size:15px;border:2px solid var(--cream)}
.btn.main{background:var(--cream);color:var(--maroon)}
.btn.main:hover{background:var(--pink);border-color:var(--pink)}
.btn.alt:hover{background:var(--cream);color:var(--maroon)}
.badge{width:min(100%,340px);aspect-ratio:1;border-radius:50%;background:var(--pink);color:var(--maroon);display:grid;place-items:center;justify-self:center;position:relative}
.badge b{font-family:var(--serif);font-size:clamp(90px,14vw,150px);font-weight:400;font-style:italic}
.badge::after{content:"";position:absolute;width:26%;aspect-ratio:1;border-radius:50%;background:var(--maroon);right:2%;bottom:4%}

/* light sections */
.light{background:var(--cream);color:var(--maroon)}
.light h2 em{color:#a3414f}
.sage{background:var(--sage);color:var(--maroon)}
.sage h2 em{color:#7a2a36}

/* role fit */
.fit{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:20px}
.fit article{background:var(--maroon);color:var(--cream);padding:28px;border-radius:22px}
.fit article:nth-child(2){background:var(--pink);color:var(--maroon)}
.fit article:nth-child(3){background:var(--maroon-2)}
.fit article:nth-child(4){background:var(--pink);color:var(--maroon)}
.fit h3{font-size:30px;margin-bottom:12px}
.fit p{font-size:15.5px}

/* about */
.about{display:grid;grid-template-columns:1fr 1fr;gap:48px}
.about p+p{margin-top:16px}
.facts{list-style:none;padding:0;border-left:4px solid var(--maroon);padding-left:24px;display:grid;gap:14px}
.facts strong{display:block;font-family:var(--serif);font-weight:400;font-size:26px;line-height:1.1}

/* experience */
.job{display:grid;grid-template-columns:200px 1fr;gap:28px;padding:30px 0;border-top:1px solid rgba(253,251,224,.25)}
.job:last-child{border-bottom:1px solid rgba(253,251,224,.25)}
.job .when{color:var(--pink);font-size:15px;font-weight:500}
.job h3{font-size:34px;margin-bottom:4px}
.job .org{font-weight:700;margin-bottom:12px}
.job ul{padding-left:20px}
.job li{margin-bottom:6px}

/* projects */
.projects{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:22px}
.proj{background:var(--cream);border-radius:22px;padding:28px;display:flex;flex-direction:column;gap:12px}
.proj:nth-child(even){background:var(--pink)}
.proj h3{font-size:30px}
.proj p{font-size:15.5px;flex:1}
.proj .tags{font-size:13.5px;font-weight:700}
.proj a{font-weight:700;font-size:15px}

/* skills */
.skills{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:36px}
.skills h3{font-size:30px;margin-bottom:12px}
.skills ul{list-style:none;padding:0;display:flex;flex-wrap:wrap;gap:8px}
.skills li{border:2px solid var(--maroon);border-radius:999px;padding:4px 14px;font-size:14.5px;font-weight:500}

/* contact */
.contact{text-align:center;overflow:hidden}
.contact h2{font-size:clamp(56px,10vw,120px);margin-bottom:20px}
.contact h2 span{font-style:italic;color:var(--pink);display:block}
.contact p{max-width:520px;margin:0 auto 28px}
.contact .btns{justify-content:center}
footer{padding:22px 0;text-align:center;font-size:13.5px;background:var(--maroon-2);color:var(--sage)}

@media (max-width:760px){
  .hero-grid,.about,.job{grid-template-columns:1fr}
  .badge{width:220px}
  nav ul{gap:14px}
  .brand{display:none}
  section{padding:64px 0}
}
@media (prefers-reduced-motion:reduce){html{scroll-behavior:auto}}
</style>
</head>
<body>

<nav aria-label="Main">
  <div class="wrap">
    <span class="brand">Amna Ghafoor</span>
    <ul>
      <li><a href="#fit">Role fit</a></li>
      <li><a href="#experience">Experience</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </div>
</nav>

<header class="hero">
  <div class="dot" style="width:46px;height:46px;top:40px;right:12%"></div>
  <div class="dot" style="width:22px;height:22px;top:150px;right:4%"></div>
  <div class="dot" style="width:70px;height:70px;bottom:30px;left:-20px"></div>
  <div class="wrap hero-grid">
    <div>
      <span class="pill">Computer Science Graduate</span>
      <h1 style="margin-top:22px">Amna <span>Ghafoor</span></h1>
      <p class="lead">I work with SQL, Python and data to find out what is happening and why. I built a startup database that cut data access time by 35%, and I am looking for my first full-time tech role.</p>
      <div class="btns">
        <a class="btn main" href="mailto:contact.amnaghafoor@gmail.com?subject=Application%20-%20CindraForge">Email me</a>
        <a class="btn alt" href="#projects">See my projects</a>
      </div>
    </div>
    <div class="badge" aria-hidden="true"><b>AG</b></div>
  </div>
</header>

<section id="fit" class="light">
  <div class="wrap">
    <h2>What I bring to <em>your team</em></h2>
    <div class="fit">
      <article>
        <h3>Programming basics</h3>
        <p>BSc Computer Science (2021–2025). I write Python, SQL and C++, and completed a 40-day Python for Data Science course.</p>
      </article>
      <article>
        <h3>SQL and databases</h3>
        <p>I built and managed a startup database at NICF that reduced data access time by 35%.</p>
      </article>
      <article>
        <h3>Analysis and troubleshooting</h3>
        <p>I clean messy data, track trends and flag what looks wrong. Data quality rose 20% after I improved collection and cleaning.</p>
      </article>
      <article>
        <h3>Ready to learn</h3>
        <p>I picked up Power BI, agentic AI and Generative AI through bootcamps and courses, and I am eager to learn log monitoring on the job.</p>
      </article>
    </div>
  </div>
</section>

<section id="about">
  <div class="dot" style="width:54px;height:54px;top:60px;right:8%"></div>
  <div class="wrap about">
    <div>
      <h2>About <em>me</em></h2>
      <p>I am a Computer Science graduate from Government College University, Faisalabad. My internships took me from startup data work to equity research, where I spent my days turning raw numbers into reports people could act on.</p>
      <p>I like work where careful checking matters: a query that returns the right rows, a dashboard that matches the source, a problem traced back to its cause.</p>
    </div>
    <ul class="facts">
      <li><strong>Faisalabad, Pakistan</strong>Open to on-site work</li>
      <li><strong>BSc Computer Science</strong>GCUF, 2021–2025</li>
      <li><strong>She-Venture Fellow</strong>NIC Faisalabad, founder of FlexiBuild</li>
    </ul>
  </div>
</section>

<section id="experience" class="sage" style="background:var(--maroon-2);color:var(--cream)">
  <div class="wrap">
    <h2>Experience</h2>
    <div class="job">
      <div class="when">Oct 2025 – Nov 2025<br>On site</div>
      <div>
        <h3>Management Trainee Officer</h3>
        <p class="org">AKD Securities Ltd.</p>
        <ul>
          <li>Analyzed stock price, volume and trend data across 6 PSX sectors and 176 companies.</li>
          <li>Built internal Excel dashboards and reports for the research team.</li>
          <li>Prepared industry reports from financial and market data.</li>
        </ul>
      </div>
    </div>
    <div class="job">
      <div class="when">Apr 2025 – Present</div>
      <div>
        <h3>Founder, FlexiBuild</h3>
        <p class="org">She-Venture Fellowship, NIC Faisalabad</p>
        <ul>
          <li>Lead product direction for a construction-tech startup using research and data.</li>
          <li>Break technical and market problems into practical, buildable steps.</li>
        </ul>
      </div>
    </div>
    <div class="job">
      <div class="when">Aug 2023 – Oct 2023<br>On site</div>
      <div>
        <h3>Data Science Intern</h3>
        <p class="org">National Incubation Center Faisalabad</p>
        <ul>
          <li>Built and managed a startup database, cutting data access time by 35%.</li>
          <li>Improved data collection and cleaning, raising data quality by 20%.</li>
          <li>Researched 27 startups; one startup grew customer acquisition by 12% and cut costs by 5% using my insights.</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="projects" class="sage">
  <div class="wrap">
    <h2>Selected <em>projects</em></h2>
    <div class="projects">
      <article class="proj">
        <h3>Electric Vehicle Dashboard</h3>
        <p>An interactive Power BI dashboard that shows EV market data and trends in one view.</p>
        <span class="tags">Power BI, data visualization</span>
        <a href="https://amna-ghafoor.github.io/AmnaGhafoor">View in my portfolio</a>
      </article>
      <article class="proj">
        <h3>Pakistan Cement Market Report</h3>
        <p>Sector analysis and reporting on the Pakistani cement industry.</p>
        <span class="tags">Data analysis, reporting</span>
        <a href="https://amna-ghafoor.github.io/AmnaGhafoor">View in my portfolio</a>
      </article>
      <article class="proj">
        <h3>Education in Punjab</h3>
        <p>A data-driven report on education statistics and trends across Punjab.</p>
        <span class="tags">Data analysis, research</span>
        <a href="https://amna-ghafoor.github.io/AmnaGhafoor">View in my portfolio</a>
      </article>
      <article class="proj">
        <h3>AI Home Construction Platform</h3>
        <p>An AI-driven platform that supports construction decisions, built for FlexiBuild.</p>
        <span class="tags">AI, product thinking</span>
        <a href="https://amna-ghafoor.github.io/AmnaGhafoor">View in my portfolio</a>
      </article>
      <article class="proj">
        <h3>Mock Interview Chat Bot</h3>
        <p>An AI tool that lets people practice interview questions and get instant replies.</p>
        <span class="tags">Python, AI</span>
        <a href="https://amna-ghafoor.github.io/AmnaGhafoor">View in my portfolio</a>
      </article>
    </div>
  </div>
</section>

<section id="skills" class="light">
  <div class="wrap">
    <h2>Skills and <em>training</em></h2>
    <div class="skills">
      <div>
        <h3>Programming and data</h3>
        <ul><li>Python</li><li>SQL</li><li>C++</li><li>Data cleaning</li><li>Data wrangling</li></ul>
      </div>
      <div>
        <h3>Analysis tools</h3>
        <ul><li>Power BI</li><li>Excel</li><li>Tableau</li><li>KPI tracking</li><li>Trend analysis</li></ul>
      </div>
      <div>
        <h3>Ways of working</h3>
        <ul><li>Problem solving</li><li>Troubleshooting</li><li>Communication</li><li>Teamwork</li><li>Quick learner</li></ul>
      </div>
      <div>
        <h3>Certifications</h3>
        <ul><li>Agentic AI Bootcamp, atomcamp</li><li>Power BI Workshop, atomcamp</li><li>Data Analysis for Governance</li><li>Intro to Generative AI and LLMs, Google</li><li>40 Days of Python, Codanics</li></ul>
      </div>
    </div>
  </div>
</section>

<section id="contact" class="contact">
  <div class="dot" style="width:60px;height:60px;top:50px;left:10%"></div>
  <div class="dot" style="width:28px;height:28px;bottom:80px;right:12%"></div>
  <div class="wrap">
    <h2>Let’s <span>talk.</span></h2>
    <p>I would love to start my tech career at CindraForge. My CV is attached to my application email and I am happy to share more on request.</p>
    <div class="btns">
      <a class="btn main" href="mailto:contact.amnaghafoor@gmail.com">contact.amnaghafoor@gmail.com</a>
      <a class="btn alt" href="https://linkedin.com/in/amnaghafoor/">LinkedIn</a>
      <a class="btn alt" href="tel:+923427775560">+92 342 7775560</a>
    </div>
  </div>
</section>

<footer>© 2026 Amna Ghafoor · Faisalabad, Pakistan</footer>

</body>
</html>
