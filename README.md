<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MASHPC | Learning Hub</title>
  <style>
    :root{
      --bg:#07111e;
      --panel:#0d1b2a;
      --card:#11263d;
      --text:#e8eef8;
      --muted:#9cb0ca;
      --primary:#58d68d;
      --primary-2:#6fe7ff;
      --accent:#f5b942;
      --border:rgba(255,255,255,0.08);
      --shadow:0 20px 40px rgba(3,7,18,.35);
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: Inter,Segoe UI,Arial,sans-serif;
      background: linear-gradient(180deg,#07111e,#0b1728 30%, #050b12);
      color:var(--text);
      line-height:1.6;
    }

    a{text-decoration:none;color:inherit}
    .container{width:min(1180px, calc(100% - 28px)); margin:0 auto}
    .topbar{
      position:sticky; top:0; z-index:20;
      backdrop-filter: blur(12px);
      background: rgba(7,17,30,.8);
      border-bottom:1px solid var(--border);
    }
    .nav{
      min-height:72px; display:flex; align-items:center; justify-content:space-between; gap:20px;
    }
    .brand{
      display:flex; align-items:center; gap:12px; font-weight:800; letter-spacing:.04em; text-transform:uppercase;
    }
    .brand-mark{
      width:42px;height:42px;border-radius:12px; display:grid;place-items:center; background:linear-gradient(135deg,var(--primary),var(--primary-2)); color:#041118; font-weight:900;
    }
    .nav-links{display:flex;gap:24px; color:var(--muted);}
    .button{
      background:linear-gradient(135deg,var(--primary),var(--primary-2));
      color:#041118; font-weight:800; border:none; border-radius:12px; padding:12px 18px; cursor:pointer;
    }

    .hero{
      padding:48px 0 24px;
    }
    .hero-box{
      background:linear-gradient(180deg,#112335,#0d1a2b);
      border:1px solid var(--border); border-radius:24px; box-shadow:var(--shadow);
      padding:30px 22px;
    }
    .eyebrow{
      display:inline-flex;align-items:center;gap:8px;
      background:rgba(88,214,141,.12); border:1px solid rgba(88,214,141,.2);
      color:var(--primary); border-radius:999px; padding:8px 12px; font-weight:700; font-size:.8rem;
    }
    .dot{width:8px;height:8px;border-radius:50%;background:var(--primary);display:inline-block; box-shadow:0 0 10px rgba(88,214,141,.7);}
    h1{
      margin:18px 0 12px; font-size:clamp(2.3rem,5vw,3.5rem); letter-spacing:-.05em;
    }
    .gradient-text{
      background:linear-gradient(135deg,var(--primary),var(--primary-2),#c9b7ff);
      -webkit-background-clip:text; background-clip:text; color:transparent;
    }
    .lead{
      margin:0; color:var(--muted); max-width:800px; font-size:1.04rem;
    }

    .grid{
      display:grid; grid-template-columns:repeat(3, minmax(0,1fr)); gap:18px; margin-top:30px;
    }
    .card{
      background:linear-gradient(180deg, rgba(17,37,61,.9), rgba(10,18,26,.9));
      border:1px solid var(--border); border-radius:18px; padding:20px; box-shadow:0 10px 25px rgba(0,0,0,.12);
    }
    .card h3{margin:0 0 10px; font-size:1.2rem;}
    .card p{margin:0; color:var(--muted);}
    .pill{
      display:inline-block; padding:6px 10px; border-radius:999px; font-size:.75rem; font-weight:700;
      margin-bottom:12px; border:1px solid rgba(255,255,255,.1); background:rgba(255,255,255,.03); color:var(--primary-2);
    }

    .section{
      padding:26px 0 10px;
    }
    .section h2{
      margin:0 0 18px; font-size:clamp(1.6rem,3vw,2.2rem); letter-spacing:-.04em;
    }

    .resource-list{
      display:grid; grid-template-columns:repeat(2,minmax(0,1fr)); gap:18px;
    }
    .resource{
      background:rgba(255,255,255,.02); border:1px solid var(--border); border-radius:18px; padding:18px 18px 14px;
    }
    .resource h4{margin:0 0 8px; font-size:1.04rem;}
    .resource p{margin:0; color:var(--muted);}
    .resource strong{color:var(--text);}
    .warning{
      margin-top:20px; padding:16px 18px; border-radius:14px; background:rgba(245,185,66,.07);
      border:1px solid rgba(245,185,66,.18); color:#f5d799;
    }

    .video-grid{
      display:grid; grid-template-columns:repeat(2,minmax(0,1fr)); gap:18px; margin-top:18px;
    }
    .video{
      background:rgba(255,255,255,.02); border:1px solid var(--border); border-radius:16px; padding:16px;
    }
    .video .meta{
      display:flex; justify-content:space-between; gap:10px; margin-bottom:10px; color:var(--muted); font-size:.8rem;
    }
    .video a{
      color:var(--primary-2); font-weight:700;
    }

    footer{
      text-align:center; color:var(--muted); padding:28px 0 52px; font-size:.92rem;
    }

    @media (max-width: 860px){
      .grid, .resource-list, .video-grid{
        grid-template-columns:1fr;
      }
      .nav-links{
        display:none;
      }
    }
  </style>
</head>
<body>
  <header class="topbar">
    <div class="container nav">
      <div class="brand">
        <div class="brand-mark">M</div>
        <span>MASHPC</span>
      </div>

      <nav class="nav-links">
        <a href="index.html">Home</a>
        <a href="#cyber">Cyber Basics</a>
        <a href="#resources">Resources</a>
        <a href="#videos">Videos</a>
      </nav>

      <a href="index.html" class="button">Back to home</a>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div class="hero-box">
        <div class="eyebrow"><span class="dot"></span> Ethical cybersecurity learning</div>
        <h1><span class="gradient-text">Cybersecurity</span> learning hub</h1>
        <p class="lead">
          This learning space focuses on defensive security, ethical education, and safe technical awareness.
          It does not provide instructions for unauthorized access, hacking, malware, or attack tools.
        </p>
      </div>
    </section>

    <section class="section" id="cyber">
      <h2>Key cybersecurity concepts</h2>
      <div class="grid">
        <article class="card">
          <div class="pill">SSH</div>
          <h3>What is SSH?</h3>
          <p>SSH is a secure network protocol used to access and manage systems over an encrypted connection. It helps protect login and command traffic.</p>
        </article>

        <article class="card">
          <div class="pill">Security</div>
          <h3>What is a hacker?</h3>
          <p>A hacker is a person with technical skill; in security, “ethical hacker” refers to authorized professionals testing systems for weaknesses with permission.</p>
        </article>

        <article class="card">
          <div class="pill">Ethics</div>
          <h3>What is hacking?</h3>
          <p>Hacking generally means learning, modifying, or testing technology, but legitimate security work is defined by permission, legality, and responsible disclosure.</p>
        </article>

        <article class="card">
          <div class="pill">Tools</div>
          <h3>What devices/tools are needed?</h3>
          <p>Common cybersecurity learning setups include a secure lab laptop, virtual machines, safe networking tools, and legally approved testing environments.</p>
        </article>

        <article class="card">
          <div class="pill">Networking</div>
          <h3>IP basics</h3>
          <p>IP addresses are identifiers used in networks. Understanding them is part of networking and security fundamentals, but privacy and lawful use matter.</p>
        </article>

        <article class="card">
          <div class="pill">Defense</div>
          <h3>DoS / DDoS</h3>
          <p>Denial-of-service attacks are harmful and illegal when unauthorized. Defensive security focuses on detection, rate limiting, load balancing, and resilience.</p>
        </article>
      </div>

      <div class="warning">
        This page is meant for ethical, legal learning only. It avoids step-by-step attack guidance, exploitation flows, privilege escalation, malware deployment, or unauthorized system access.
      </div>
    </section>

    <section class="section" id="resources">
      <h2>Safe learning resources & tools</h2>
      <div class="resource-list">
        <article class="resource">
          <h4><strong>Android security labs</strong></h4>
          <p>Tools like APKTool and Android debugging environments can be used for legitimate reverse-engineering and security education under proper authorization.</p>
        </article>

        <article class="resource">
          <h4><strong>Termux</strong></h4>
          <p>Termux is a terminal emulator often used for learning Linux commands, scripting, networking basics, and secure system administration.</p>
        </article>

        <article class="resource">
          <h4><strong>Kali NetHunter</strong></h4>
          <p>Kali NetHunter is a mobile penetration testing platform intended for authorized, legal security work in controlled environments.</p>
        </article>

        <article class="resource">
          <h4><strong>Ethical hacking</strong></h4>
          <p>Focus on authorized testing, vulnerability disclosure, secure configuration, and defensive controls rather than exploit development or unauthorized testing.</p>
        </article>
      </div>
    </section>

    <section class="section" id="videos">
      <h2>Free learning videos (max 50)</h2>
      <div class="video-grid">
        <div class="video">
          <div class="meta"><span>1</span><span>Cybersecurity Basics</span></div>
          <a href="https://www.youtube.com/results?search_query=cybersecurity+basics+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>2</span><span>Networking Fundamentals</span></div>
          <a href="https://www.youtube.com/results?search_query=networking+fundamentals+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>3</span><span>Introduction to SSH</span></div>
          <a href="https://www.youtube.com/results?search_query=introduction+to+ssh+tutorial" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>4</span><span>Ethical Hacking Overview</span></div>
          <a href="https://www.youtube.com/results?search_query=ethical+hacking+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>5</span><span>Linux Basics</span></div>
          <a href="https://www.youtube.com/results?search_query=linux+for+beginners+tutorial" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>6</span><span>Wi-Fi & Security</span></div>
          <a href="https://www.youtube.com/results?search_query=wi-fi+security+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>7</span><span>Web security</span></div>
          <a href="https://www.youtube.com/results?search_query=web+application+security+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>8</span><span>Incident Response</span></div>
          <a href="https://www.youtube.com/results?search_query=incident+response+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>9</span><span>Malware basics</span></div>
          <a href="https://www.youtube.com/results?search_query=malware+analysis+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
        <div class="video">
          <div class="meta"><span>10</span><span>Digital Forensics</span></div>
          <a href="https://www.youtube.com/results?search_query=digital+forensics+for+beginners" target="_blank" rel="noreferrer">Start learning</a>
        </div>
      </div>
    </section>
  </main>

  <footer>
    MASHPC AI | Ethical cybersecurity learning and safe defensive practices
  </footer>
</body>
</html>
