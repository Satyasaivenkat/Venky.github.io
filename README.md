# Venky.github.io
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Pampana Satya Sai Venkat — Interactive Portfolio</title>
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#7c3aed; --muted:#9aa4b2; --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.03);
      --max-width:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,Arial;background:linear-gradient(180deg,#071028 0%, #0f1724 60%);color:#e6eef6}
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max-width);margin:0 auto;padding:40px 20px}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 380px;gap:32px;align-items:center;padding:40px;background:linear-gradient(90deg, rgba(124,58,237,0.06), transparent);border-radius:16px;box-shadow:0 6px 30px rgba(2,6,23,0.6)}
    .hero .intro h1{font-size:28px;margin:0 0 8px 0;letter-spacing:-0.5px}
    .hero .intro p{margin:0;color:var(--muted)}
    .hero .meta{display:flex;flex-direction:column;gap:12px;align-items:flex-end}
    .card{background:linear-gradient(180deg,var(--glass), var(--glass-2));padding:18px;border-radius:12px;backdrop-filter:blur(6px)}

    .contact-row{display:flex;gap:12px;flex-wrap:wrap}
    .pill{display:inline-flex;align-items:center;gap:8px;padding:8px 12px;border-radius:999px;background:rgba(255,255,255,0.03);font-size:14px;color:var(--muted)}

    /* Sections */
    section{margin-top:32px}
    .section-title{display:flex;align-items:center;gap:12px;margin-bottom:18px}
    .section-title h2{margin:0;font-size:18px}
    .timeline{position:relative;padding-left:24px}
    .timeline:before{content:'';position:absolute;left:8px;top:0;bottom:0;width:2px;background:linear-gradient(#7c3aed,#1e3a8a)}
    .timeline-item{position:relative;padding:20px 18px;margin-bottom:18px;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);border-radius:12px}
    .timeline-item .meta{font-size:13px;color:var(--muted)}

    .skills{display:flex;gap:12px;flex-wrap:wrap}
    .skill{padding:10px 14px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));font-weight:600}

    .projects-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:16px}
    .project{padding:18px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);transition:transform .35s ease, box-shadow .35s ease}
    .project:hover{transform:translateY(-6px);box-shadow:0 12px 40px rgba(2,6,23,0.6)}

    .contact-card{display:flex;flex-direction:column;gap:12px}
    .btn{display:inline-block;padding:10px 16px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#1e90ff);color:white;font-weight:700}

    footer{margin-top:40px;text-align:center;color:var(--muted);font-size:13px}

    /* responsive */
    @media(max-width:900px){
      .hero{grid-template-columns:1fr;}
      .projects-grid{grid-template-columns:1fr}
    }

    /* micro animations */
    .glow{box-shadow:0 10px 30px rgba(124,58,237,0.12)}
    .tag{font-size:12px;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.02);color:var(--muted)}

  </style>
</head>
<body>
  <div class="wrap">
    <header class="hero" id="hero">
      <div class="intro">
        <div class="card">
          <h1>Pampana Satya Sai Venkat</h1>
          <p class="muted">QA Engineer · Automation (Selenium + Java) · Manual Testing · JIRA</p>
          <div style="height:14px"></div>
          <p>I ensure high-quality web experiences by combining structured test design, Selenium automation, and collaborative defect management. Passionate about building reliable, responsive applications — currently focused on Solpeine, a photographer’s portfolio and booking platform.</p>
          <div style="height:12px"></div>
          <div class="contact-row">
            <span class="pill">📞 +91 99086 77538</span>
            <a class="pill" href="mailto:satyasaivenkat26@gmail.com">✉️ satyasaivenkat26@gmail.com</a>
            <a class="pill" href="https://www.linkedin.com/in/satya-sai-venkat-46b006194" target="_blank">🔗 LinkedIn</a>
          </div>
        </div>
      </div>

      <aside class="meta">
        <div class="card" style="width:100%">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div>
              <div class="tag">Location</div>
              <div style="font-weight:700;margin-top:6px">Rajahmundry, India</div>
            </div>
            <div style="text-align:right">
              <div class="tag">Experience</div>
              <div style="font-weight:700;margin-top:6px">1+ yrs (Internships & Projects)</div>
            </div>
          </div>
          <div style="height:12px"></div>
          <div style="display:flex;gap:8px;justify-content:space-between;align-items:center">
            <div style="flex:1">
              <div class="tag">Primary</div>
              <div style="font-weight:700;margin-top:6px">Selenium + Java</div>
            </div>
            <div style="flex:1;text-align:right">
              <div class="tag">Tool</div>
              <div style="font-weight:700;margin-top:6px">JIRA</div>
            </div>
          </div>
        </div>
        <div class="card" style="width:100%;text-align:center">
          <div style="font-size:13px;color:var(--muted)">Open to roles:</div>
          <div style="font-weight:800;margin-top:8px">QA Engineer · Automation Tester · Software Test Engineer</div>
          <div style="height:12px"></div>
          <a class="btn" href="#contact">Contact Me</a>
        </div>
      </aside>
    </header>

    <!-- Narrative Timeline -->
    <section id="timeline">
      <div class="section-title"><h2>Career Timeline</h2><div style="flex:1"></div></div>
      <div class="timeline">
        <div class="timeline-item" data-when="2025">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div>
              <strong>Zummit Infolabs — QA Engineer</strong>
              <div class="meta">March 2025 – Present</div>
            </div>
            <div class="tag">Solpeine</div>
          </div>
          <p style="margin-top:10px;color:var(--muted)">Led QA for Solpeine: wrote test cases from SRS, executed manual and automated tests, managed a 2-member QA team, and tracked defects in JIRA. Built Selenium + Java automation to streamline regression.</p>
        </div>

        <div class="timeline-item" data-when="2023">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div>
              <strong>HQL Edutech — Software Tester Intern</strong>
              <div class="meta">Oct 2023 – Apr 2024</div>
            </div>
            <div class="tag">E-commerce Testing</div>
          </div>
          <p style="margin-top:10px;color:var(--muted)">Executed UI and integration testing on e-commerce web app; authored automation scripts using Selenium WebDriver and documented defects with reproduction steps.</p>
        </div>
      </div>
    </section>

    <!-- Skills -->
    <section id="skills">
      <div class="section-title"><h2>Core Skills</h2><div style="flex:1"></div></div>
      <div class="skills">
        <div class="skill">Selenium WebDriver</div>
        <div class="skill">Java</div>
        <div class="skill">TestNG</div>
        <div class="skill">Manual Testing</div>
        <div class="skill">Test Case Design</div>
        <div class="skill">Regression Testing</div>
        <div class="skill">JIRA</div>
        <div class="skill">Agile / SDLC</div>
        <div class="skill">HTML / CSS / JavaScript</div>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects">
      <div class="section-title"><h2>Selected Projects</h2><div style="flex:1"></div></div>
      <div class="projects-grid">
        <article class="project">
          <h3>Solpeine — Photographer’s Website</h3>
          <p class="meta">Role: QA Engineer · Selenium Automation · Team Lead</p>
          <p style="color:var(--muted);margin-top:8px">A portfolio + booking platform for photographers. Tested gallery, booking flow, payment gateway, and admin panels. Automated critical flows using Selenium WebDriver and Java; reduced manual regression workload significantly.</p>
          <div style="height:10px"></div>
          <div style="display:flex;gap:8px;flex-wrap:wrap">
            <span class="pill">Test Cases</span><span class="pill">Automation</span><span class="pill">API Testing</span>
          </div>
        </article>

        <article class="project">
          <h3>E-commerce Web App — HQL Edutech</h3>
          <p class="meta">Role: Software Tester Intern</p>
          <p style="color:var(--muted);margin-top:8px">Focused on UI/functional testing and automation. Logged detailed defects and verified fixes across releases, contributing to improved stability.</p>
          <div style="height:10px"></div>
          <div style="display:flex;gap:8px;flex-wrap:wrap">
            <span class="pill">UI Testing</span><span class="pill">Selenium</span><span class="pill">Bug Reporting</span>
          </div>
        </article>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact">
      <div class="section-title"><h2>Get in Touch</h2><div style="flex:1"></div></div>
      <div class="card contact-card">
        <div style="display:flex;gap:16px;flex-wrap:wrap">
          <div style="flex:1;min-width:220px">
            <strong>Email</strong>
            <div class="meta">satyasaivenkat26@gmail.com</div>
            <div style="height:8px"></div>
            <strong>Phone</strong>
            <div class="meta">+91 99086 77538</div>
            <div style="height:8px"></div>
            <strong>LinkedIn</strong>
            <div class="meta"><a href="https://www.linkedin.com/in/satya-sai-venkat-46b006194" target="_blank">linkedin.com/in/satya-sai-venkat-46b006194</a></div>
          </div>
          <form style="flex:1;min-width:260px" id="contactForm">
            <label style="display:block;font-weight:600;margin-bottom:6px">Message</label>
            <textarea id="message" rows="4" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit"></textarea>
            <div style="height:10px"></div>
            <button class="btn" type="button" id="sendBtn">Send Message</button>
            <div id="formNote" style="color:var(--muted);margin-top:8px;font-size:13px"></div>
          </form>
        </div>
      </div>
    </section>

    <footer>
      Crafted with care · Interactive one-page portfolio · Designed for recruiters and hiring managers
    </footer>
  </div>

  <!-- GSAP & JS -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
  <script>
    // Basic entrance animations
    gsap.registerPlugin(ScrollTrigger);

    gsap.from('#hero .intro .card', {opacity:0,y:30,duration:0.9,delay:0.2, ease:'power3.out'});
    gsap.from('#hero .meta .card', {opacity:0,x:30,duration:0.9,delay:0.4, ease:'power3.out'});

    // timeline items
    gsap.utils.toArray('.timeline-item').forEach((el, i) => {
      gsap.from(el, {
        opacity:0, y:30, duration:0.8, delay:0.1*i,
        scrollTrigger:{trigger:el, start:'top 80%'}
      });
    });

    // projects
    gsap.utils.toArray('.project').forEach(el=>{
      gsap.from(el,{opacity:0, y:20, duration:0.8, scrollTrigger:{trigger:el, start:'top 85%'}})
    })

    // skills micro hover
    document.querySelectorAll('.skill').forEach((s)=>{
      s.addEventListener('mouseenter',()=>gsap.to(s,{scale:1.06, duration:0.25, ease:'power2.out'}));
      s.addEventListener('mouseleave',()=>gsap.to(s,{scale:1, duration:0.25, ease:'power2.out'}));
    })

    // contact form (non-server) — friendly UI
    document.getElementById('sendBtn').addEventListener('click', ()=>{
      const msg = document.getElementById('message').value.trim();
      const note = document.getElementById('formNote');
      if(!msg){ note.textContent = 'Please type a message before sending.'; return; }
      note.textContent = 'Message ready to send — copy it and email to satyasaivenkat26@gmail.com';
      gsap.fromTo(note,{opacity:0},{opacity:1,duration:0.6});
    });

    // small floating glow on scroll
    gsap.to('.hero', {boxShadow:'0 30px 120px rgba(124,58,237,0.06)', scrollTrigger:{trigger:'.hero', start:'top center', end:'bottom top', scrub:1}})

    // accessibility: reduce motion respect
    if(window.matchMedia('(prefers-reduced-motion: reduce)').matches){ gsap.globalTimeline.pause(); }
  </script>
</body>
</html>
