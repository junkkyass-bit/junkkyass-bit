<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0"/>
<title>NERV // junkkyass-bit — Profile</title>
<link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&family=Noto+Sans+JP:wght@300;400;700&display=swap" rel="stylesheet"/>
<style>
*{box-sizing:border-box;margin:0;padding:0;}
:root{
  --black:#0a0a0f;
  --darkblue:#0d1b2a;
  --blue:#1a3a5c;
  --cyan:#00b4d8;
  --red:#c1121f;
  --orange:#e07a00;
  --white:#e8e8e8;
  --dim:#7a8a9a;
  --green:#00ff88;
}
html,body{background:var(--black);color:var(--white);font-family:'Share Tech Mono',monospace;min-height:100vh;}
body{padding:1.5rem 1rem 3rem;}

/* layout */
.wrap{max-width:860px;margin:0 auto;}
.scanline-wrap{border:1px solid var(--blue);border-radius:2px;overflow:hidden;margin-bottom:1.2rem;}
.header-term{background:var(--darkblue);border-bottom:1px solid var(--cyan);padding:.35rem .8rem;display:flex;align-items:center;justify-content:space-between;}
.term-title{font-size:.65rem;color:var(--cyan);letter-spacing:.15em;text-transform:uppercase;}
.term-dots{display:flex;gap:5px;}
.dot{width:8px;height:8px;border-radius:50%;}
.dot-r{background:var(--red);}
.dot-o{background:var(--orange);}
.dot-g{background:#3a3;}
.content-pad{padding:1.2rem 1rem;}

/* hero */
.hero{text-align:center;padding:2rem 1rem 1.5rem;border-bottom:1px solid var(--blue);}
.nerv-logo{font-size:.65rem;color:var(--dim);letter-spacing:.3em;margin-bottom:.5rem;}
.nerv-logo span{color:var(--red);}
.big-name{font-size:2.6rem;font-weight:700;color:var(--white);letter-spacing:-.02em;line-height:1;font-family:'Noto Sans JP',sans-serif;}
.big-name em{color:var(--cyan);font-style:normal;}
.jp-sub{font-size:.8rem;color:var(--dim);letter-spacing:.2em;margin:.4rem 0 .2rem;font-family:'Noto Sans JP',sans-serif;}
.pattern-line{font-size:.65rem;color:var(--red);letter-spacing:.08em;margin-top:.3rem;}
.cursor{display:inline-block;width:10px;height:1em;background:var(--cyan);vertical-align:middle;animation:blink 1s step-end infinite;}
@keyframes blink{0%,100%{opacity:1;}50%{opacity:0;}}

/* alert bars */
.alert-bar{background:var(--red);color:#fff;font-size:.65rem;letter-spacing:.2em;padding:.3rem .8rem;text-align:center;text-transform:uppercase;}
.active-bar{background:#003a1a;color:var(--green);font-size:.65rem;letter-spacing:.2em;padding:.3rem .8rem;text-align:center;border:1px solid #005a2a;margin-bottom:1.2rem;}

/* section headers */
.sec-header{font-size:.6rem;color:var(--cyan);letter-spacing:.25em;text-transform:uppercase;border-bottom:1px solid var(--blue);padding-bottom:.3rem;margin-bottom:.8rem;}
.sec-header span{color:var(--dim);}

/* about grid */
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:.8rem;margin-bottom:1.2rem;}
.about-block{border:1px solid var(--blue);border-radius:2px;padding:.8rem;}
.about-label{font-size:.58rem;color:var(--cyan);letter-spacing:.2em;text-transform:uppercase;margin-bottom:.4rem;}
.about-val{font-size:.78rem;color:var(--white);line-height:1.6;}
.about-val .acc{color:var(--orange);}
.about-val .live{color:var(--green);}

/* code block */
.code-window{border:1px solid var(--blue);border-radius:2px;overflow:hidden;margin-bottom:1.2rem;}
.code-body{background:#060d14;padding:.9rem 1rem;font-size:.75rem;line-height:1.8;color:var(--dim);overflow-x:auto;white-space:pre;}
.kw{color:#569cd6;}
.str{color:#ce9178;}
.key{color:var(--cyan);}
.val{color:var(--orange);}
.cm{color:#4a5a6a;}
.arr2{color:#9cdcfe;}

/* skills */
.skill-row{display:grid;grid-template-columns:repeat(auto-fill,minmax(130px,1fr));gap:.5rem;margin-bottom:.6rem;}
.skill-chip{border:1px solid var(--blue);border-radius:2px;padding:.4rem .6rem;font-size:.65rem;letter-spacing:.08em;display:flex;align-items:center;gap:.4rem;}
.chip-fe{border-color:#1a4a7a;color:#7ab8f5;}
.chip-be{border-color:#1a4a3a;color:#7af5b8;}
.chip-db{border-color:#4a1a2a;color:#f57ab8;}
.chip-tool{border-color:#3a3a1a;color:#f5e07a;}
.chip-infra{border-color:#3a1a4a;color:#c07af5;}
.chip-dot{width:6px;height:6px;border-radius:50%;flex-shrink:0;}
.dfe{background:#378ADD;}
.dbe{background:#1D9E75;}
.ddb{background:#D4537E;}
.dtool{background:#BA7517;}
.dinfra{background:#7F77DD;}

/* stats */
.stat-row{display:grid;grid-template-columns:repeat(4,1fr);gap:.6rem;margin-bottom:1.2rem;}
.stat-box{border:1px solid var(--blue);border-radius:2px;padding:.7rem;text-align:center;}
.stat-n{font-size:1.5rem;font-weight:700;line-height:1;}
.stat-l{font-size:.55rem;color:var(--dim);letter-spacing:.15em;text-transform:uppercase;margin-top:.3rem;}
.stat-bar{height:3px;background:#1a2a3a;border-radius:2px;margin-top:.4rem;overflow:hidden;}
.stat-fill{height:100%;border-radius:2px;}

/* progress */
.prog-item{margin-bottom:.6rem;}
.prog-top{display:flex;justify-content:space-between;font-size:.62rem;margin-bottom:.2rem;}
.prog-name{color:var(--white);letter-spacing:.05em;}
.prog-pct{color:var(--cyan);}
.prog-track{height:4px;background:#1a2a3a;border-radius:2px;overflow:hidden;}
.prog-bar{height:100%;border-radius:2px;}

/* projects */
.projects{display:grid;grid-template-columns:1fr 1fr;gap:.8rem;margin-bottom:1.2rem;}
.proj-card{border:1px solid var(--blue);border-radius:2px;padding:.8rem;position:relative;overflow:hidden;}
.proj-card::before{content:'';position:absolute;top:0;left:0;width:3px;height:100%;}
.proj-num{font-size:.55rem;color:var(--dim);letter-spacing:.2em;margin-bottom:.3rem;}
.proj-title{font-size:.82rem;color:var(--white);margin-bottom:.3rem;font-weight:700;}
.proj-stack{font-size:.6rem;color:var(--orange);margin-bottom:.4rem;letter-spacing:.05em;}
.proj-desc{font-size:.62rem;color:var(--dim);line-height:1.5;margin-bottom:.4rem;}
.proj-status{font-size:.58rem;padding:2px 7px;border-radius:2px;display:inline-block;}
.s-active{background:#0a2a1a;color:#00ff88;border:1px solid #004d1a;}
.s-plan{background:#1a1a0a;color:#ffcc00;border:1px solid #4d4400;}

/* pulse dot */
.pulse{display:inline-block;width:6px;height:6px;border-radius:50%;background:var(--green);margin-right:4px;vertical-align:middle;animation:pulse 1.5s ease-in-out infinite;}
@keyframes pulse{0%,100%{opacity:1;}50%{opacity:.2;}}

/* quote */
.quote-terminal{border:1px solid var(--blue);border-radius:2px;padding:1rem;margin-bottom:1.2rem;background:#060d14;}
.prompt{color:var(--cyan);font-size:.7rem;margin-bottom:.3rem;}
.q-text{font-size:.75rem;color:var(--dim);line-height:1.9;}
.q-author{font-size:.62rem;color:var(--red);margin-top:.5rem;}

/* connect */
.connect-row{display:flex;flex-wrap:wrap;gap:.5rem;margin-bottom:1.2rem;}
.conn-btn{font-family:'Share Tech Mono',monospace;font-size:.65rem;padding:6px 14px;border:1px solid var(--blue);border-radius:2px;background:transparent;color:var(--cyan);cursor:pointer;letter-spacing:.1em;text-decoration:none;transition:background .15s,color .15s;}
.conn-btn:hover{background:var(--blue);color:var(--white);}
.footer-strip{border-top:1px solid var(--blue);padding-top:.8rem;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:.4rem;}
.footer-l{font-size:.58rem;color:var(--dim);letter-spacing:.1em;}
.footer-r{font-size:.58rem;color:var(--red);}

/* readme output */
.readme-out{background:#060d14;border:1px solid var(--blue);border-radius:2px;padding:1rem;font-family:'Share Tech Mono',monospace;font-size:.68rem;line-height:1.8;color:#5a7a8a;white-space:pre-wrap;word-break:break-word;max-height:420px;overflow-y:auto;margin-top:.8rem;}
.copy-btn{font-family:'Share Tech Mono',monospace;font-size:.7rem;padding:9px 20px;border:1px solid var(--cyan);border-radius:2px;background:transparent;color:var(--cyan);cursor:pointer;letter-spacing:.1em;margin-top:1rem;transition:background .15s,color .15s;}
.copy-btn:hover{background:var(--cyan);color:var(--black);}

@media(max-width:580px){
  .about-grid,.projects{grid-template-columns:1fr;}
  .stat-row{grid-template-columns:repeat(2,1fr);}
  .big-name{font-size:1.8rem;}
}
</style>
</head>
<body>
<div class="wrap">

  <!-- HERO -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">NERV // <span style="color:var(--white)">MAGI SYSTEM</span> — PROFILE_INIT</span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="hero">
      <div class="nerv-logo">神経 · <span>NERV</span> · TECHNICAL DIVISION · UNIT-07</div>
      <div class="big-name">Zakaria <em>Moumsik</em></div>
      <div class="jp-sub">ムムシク・ザカリア</div>
      <div class="jp-sub" style="color:var(--dim);font-size:.7rem;">動的ウェブ開発者 · モロッコ支部</div>
      <div class="pattern-line">
        <span class="pulse"></span>
        PATTERN: BLUE — DYNAMIC WEB DEVELOPER — ACTIVELY DEPLOYING — SYNC: 99.8%
        <span class="cursor"></span>
      </div>
    </div>
  </div>

  <div class="alert-bar">!! MAGI CONSENSUS: UNIT ONLINE — BUILDING DYNAMIC, DATA-DRIVEN WEB APPLICATIONS !!</div>
  <div class="active-bar"><span class="pulse"></span> STATUS: ACTIVELY SHIPPING CODE — junkkyass-bit — MOROCCO BRANCH ONLINE</div>

  <!-- PROFILE -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">SYS // <span style="color:var(--white)">OPERATOR PROFILE</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="sec-header">// <span>00</span> — identification</div>
      <div class="about-grid">
        <div class="about-block">
          <div class="about-label">Designation</div>
          <div class="about-val">Zakaria Moumsik<br><span class="acc">junkkyass-bit</span></div>
        </div>
        <div class="about-block">
          <div class="about-label">Station</div>
          <div class="about-val">Morocco 🇲🇦<br><span class="acc">Fullstack Division</span></div>
        </div>
        <div class="about-block">
          <div class="about-label">Classification</div>
          <div class="about-val"><span class="live">ACTIVE DEVELOPER</span><br><span class="acc">Dynamic Web Applications</span></div>
        </div>
        <div class="about-block">
          <div class="about-label">Specialization</div>
          <div class="about-val">PHP + MySQL backends<br><span class="acc">AJAX-powered frontends</span></div>
        </div>
      </div>

      <div class="sec-header">// <span>01</span> — neural profile</div>
      <div class="code-window">
        <div class="header-term" style="padding:.25rem .8rem;">
          <span class="term-title" style="color:var(--dim);">pilot_profile.js</span>
        </div>
        <div class="code-body"><span class="kw">const</span> <span class="arr2">zakaria</span> = {
  <span class="key">name</span>:     <span class="str">"Zakaria Moumsik"</span>,
  <span class="key">github</span>:   <span class="str">"junkkyass-bit"</span>,
  <span class="key">status</span>:   <span class="str">"ACTIVELY BUILDING"</span>,  <span class="cm">// not training. doing.</span>
  <span class="key">sync</span>:     <span class="val">99.8</span>,
  <span class="key">core</span>:     <span class="str">"Dynamic, data-driven web applications"</span>,
  <span class="key">stack</span>: {
    <span class="key">frontend</span>: [<span class="str">"HTML5"</span>, <span class="str">"CSS3"</span>, <span class="str">"JS"</span>, <span class="str">"jQuery"</span>, <span class="str">"AJAX"</span>, <span class="str">"React"</span>, <span class="str">"Next.js"</span>, <span class="str">"Three.js"</span>, <span class="str">"Tailwind"</span>],
    <span class="key">backend</span>:  [<span class="str">"Node.js"</span>, <span class="str">"PHP"</span>, <span class="str">"Python"</span>],
    <span class="key">database</span>: [<span class="str">"MySQL"</span>],
    <span class="key">infra</span>:    [<span class="str">"Linux"</span>, <span class="str">"Git"</span>, <span class="str">"GitHub"</span>, <span class="str">"npm"</span>],
  },
  <span class="key">currentlyBuilding</span>: [
    <span class="str">"Full-stack dynamic apps (PHP + MySQL + AJAX)"</span>,
    <span class="str">"3D web experiences with Three.js"</span>,
    <span class="str">"REST APIs with Node.js"</span>,
  ],
  <span class="key">mission</span>: <span class="str">"Ship dynamic websites. Every day."</span>,
};</div>
      </div>
    </div>
  </div>

  <!-- TECH STACK -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">MAGI // <span style="color:var(--white)">WEAPONS CATALOG</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="sec-header">// <span>02</span> — frontend arsenal</div>
      <div class="skill-row">
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>HTML5</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>CSS3</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>JavaScript</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>jQuery</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>AJAX / JSON</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>React</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>Next.js</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>Three.js</div>
        <div class="skill-chip chip-fe"><span class="chip-dot dfe"></span>Tailwind CSS</div>
      </div>
      <div class="sec-header">// <span>03</span> — backend core</div>
      <div class="skill-row">
        <div class="skill-chip chip-be"><span class="chip-dot dbe"></span>Node.js</div>
        <div class="skill-chip chip-be"><span class="chip-dot dbe"></span>PHP</div>
        <div class="skill-chip chip-be"><span class="chip-dot dbe"></span>Python</div>
        <div class="skill-chip chip-db"><span class="chip-dot ddb"></span>MySQL</div>
      </div>
      <div class="sec-header">// <span>04</span> — support systems</div>
      <div class="skill-row">
        <div class="skill-chip chip-infra"><span class="chip-dot dinfra"></span>Linux</div>
        <div class="skill-chip chip-tool"><span class="chip-dot dtool"></span>Git</div>
        <div class="skill-chip chip-tool"><span class="chip-dot dtool"></span>GitHub</div>
        <div class="skill-chip chip-tool"><span class="chip-dot dtool"></span>npm</div>
        <div class="skill-chip chip-tool"><span class="chip-dot dtool"></span>Photoshop</div>
      </div>
    </div>
  </div>

  <!-- ACTIVE OPERATIONS -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">NERV // <span style="color:var(--white)">ACTIVE OPERATIONS</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="sec-header">// <span>05</span> — currently deploying</div>
      <div class="projects">
        <div class="proj-card" style="border-left-color:var(--cyan);">
          <div class="proj-num"><span class="pulse"></span>OP-001 · ACTIVE</div>
          <div class="proj-title">Dynamic CRUD App</div>
          <div class="proj-stack">PHP + MySQL + AJAX + jQuery</div>
          <div class="proj-desc">Full pipeline — form to database to live DOM update. No page reload. Real users, real data.</div>
          <span class="proj-status s-active">SHIPPING</span>
        </div>
        <div class="proj-card" style="border-left-color:var(--orange);">
          <div class="proj-num"><span class="pulse"></span>OP-002 · ACTIVE</div>
          <div class="proj-title">REST API Service</div>
          <div class="proj-stack">Node.js + MySQL + JSON</div>
          <div class="proj-desc">Clean endpoints, structured JSON responses, connected to a live MySQL database.</div>
          <span class="proj-status s-active">SHIPPING</span>
        </div>
        <div class="proj-card" style="border-left-color:#c17af5;">
          <div class="proj-num">OP-003 · STAGING</div>
          <div class="proj-title">3D Portfolio Site</div>
          <div class="proj-stack">Three.js + Next.js + WebGL</div>
          <div class="proj-desc">Immersive 3D interface. Because a static portfolio page is not enough.</div>
          <span class="proj-status s-plan">IN PROGRESS</span>
        </div>
        <div class="proj-card" style="border-left-color:#f57ab8;">
          <div class="proj-num">OP-004 · STAGING</div>
          <div class="proj-title">React Dashboard</div>
          <div class="proj-stack">React + AJAX + PHP backend</div>
          <div class="proj-desc">Component-driven UI pulling live data from a PHP + MySQL API layer.</div>
          <span class="proj-status s-plan">IN PROGRESS</span>
        </div>
      </div>
    </div>
  </div>

  <!-- SYNC RATES -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">MAGI // <span style="color:var(--white)">SYNC ANALYSIS</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="sec-header">// <span>06</span> — skill synchronization</div>
      <div class="stat-row">
        <div class="stat-box">
          <div class="stat-n" style="color:var(--cyan);">16+</div>
          <div class="stat-l">Technologies</div>
          <div class="stat-bar"><div class="stat-fill" style="width:80%;background:var(--cyan);"></div></div>
        </div>
        <div class="stat-box">
          <div class="stat-n" style="color:var(--green);">2</div>
          <div class="stat-l">Stack Layers</div>
          <div class="stat-bar"><div class="stat-fill" style="width:100%;background:var(--green);"></div></div>
        </div>
        <div class="stat-box">
          <div class="stat-n" style="color:#c17af5;">99.8%</div>
          <div class="stat-l">Sync Rate</div>
          <div class="stat-bar"><div class="stat-fill" style="width:99%;background:#c17af5;"></div></div>
        </div>
        <div class="stat-box">
          <div class="stat-n" style="color:var(--orange);">▲</div>
          <div class="stat-l">Rising Pilot</div>
          <div class="stat-bar"><div class="stat-fill" style="width:65%;background:var(--orange);"></div></div>
        </div>
      </div>
      <div class="prog-item">
        <div class="prog-top"><span class="prog-name">PHP + MySQL (dynamic backends)</span><span class="prog-pct">82%</span></div>
        <div class="prog-track"><div class="prog-bar" style="width:82%;background:var(--green);"></div></div>
      </div>
      <div class="prog-item">
        <div class="prog-top"><span class="prog-name">AJAX / jQuery (live interfaces)</span><span class="prog-pct">80%</span></div>
        <div class="prog-track"><div class="prog-bar" style="width:80%;background:var(--cyan);"></div></div>
      </div>
      <div class="prog-item">
        <div class="prog-top"><span class="prog-name">React / Next.js</span><span class="prog-pct">75%</span></div>
        <div class="prog-track"><div class="prog-bar" style="width:75%;background:#7ab8f5;"></div></div>
      </div>
      <div class="prog-item">
        <div class="prog-top"><span class="prog-name">Node.js REST APIs</span><span class="prog-pct">70%</span></div>
        <div class="prog-track"><div class="prog-bar" style="width:70%;background:var(--orange);"></div></div>
      </div>
      <div class="prog-item">
        <div class="prog-top"><span class="prog-name">Three.js / WebGL</span><span class="prog-pct">55%</span></div>
        <div class="prog-track"><div class="prog-bar" style="width:55%;background:#c17af5;"></div></div>
      </div>
    </div>
  </div>

  <!-- QUOTE -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">MAGI // <span style="color:var(--white)">PILOT TRANSMISSION</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="quote-terminal">
        <div class="prompt">PILOT_07@NERV:~$</div>
        <div class="q-text">
          "I don't build static pages.<br>
          I build systems that breathe — forms that submit without reloading,<br>
          databases that talk back, interfaces that update in real time.<br>
          Dynamic is not a feature. It's the standard."
        </div>
        <div class="q-author">— ZAKARIA MOUMSIK // junkkyass-bit // SYNC: 99.8%</div>
      </div>
    </div>
  </div>

  <!-- CONNECT -->
  <div class="scanline-wrap">
    <div class="header-term">
      <span class="term-title">NERV // <span style="color:var(--white)">COMMS ARRAY</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="sec-header">// <span>07</span> — establish contact</div>
      <div class="connect-row">
        <a class="conn-btn" href="mailto:YOUR_EMAIL">[EMAIL]</a>
        <a class="conn-btn" href="https://linkedin.com/in/YOUR_PROFILE" target="_blank">[LINKEDIN]</a>
        <a class="conn-btn" href="https://twitter.com/YOUR_HANDLE" target="_blank">[TWITTER]</a>
        <a class="conn-btn" href="#" target="_blank">[PORTFOLIO]</a>
        <a class="conn-btn" href="https://github.com/junkkyass-bit" target="_blank">[GITHUB]</a>
      </div>
      <div class="footer-strip">
        <div class="footer-l">NERV TECHNICAL DIVISION · junkkyass-bit · MOROCCO BRANCH</div>
        <div class="footer-r">GOD'S IN HIS HEAVEN — ALL'S RIGHT WITH THE WORLD</div>
      </div>
    </div>
  </div>

  <!-- README COPY -->
  <div class="scanline-wrap" style="margin-top:1.2rem;">
    <div class="header-term">
      <span class="term-title">OUTPUT // <span style="color:var(--white)">README.MD</span></span>
      <div class="term-dots"><div class="dot dot-r"></div><div class="dot dot-o"></div><div class="dot dot-g"></div></div>
    </div>
    <div class="content-pad">
      <div class="sec-header">// paste this into your github profile repo</div>
      <div class="readme-out" id="readme-out"></div>
      <button class="copy-btn" id="copy-btn" onclick="copyIt()">[COPY README.MD]</button>
    </div>
  </div>

</div>

<script>
const readme = `<!-- NERV PROFILE — junkkyass-bit -->
<div align="center">

\`\`\`
███╗   ██╗███████╗██████╗ ██╗   ██╗
████╗  ██║██╔════╝██╔══██╗██║   ██║
██╔██╗ ██║█████╗  ██████╔╝██║   ██║
██║╚██╗██║██╔══╝  ██╔══██╗╚██╗ ██╔╝
██║ ╚████║███████╗██║  ██║ ╚████╔╝
╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝  ╚═══╝
\`\`\`

<img src="https://readme-typing-svg.herokuapp.com/?font=Share+Tech+Mono&size=20&center=true&vCenter=true&width=650&height=60&duration=4000&color=00B4D8&lines=PATTERN:+BLUE+%E2%80%94+CONFIRMED;DYNAMIC+WEB+DEVELOPER+%2F%2F+ACTIVELY+SHIPPING;PHP+%2B+MySQL+%2B+AJAX+%2B+React+%2B+Node.js;%E3%83%95%E3%83%AB%E3%82%B9%E3%82%BF%E3%83%83%E3%82%AF%E9%96%8B%E7%99%BA%E8%80%85+%C2%B7+%E5%8B%95%E7%9A%84%E3%82%A6%E3%82%A7%E3%83%96;GOD'S+IN+HIS+HEAVEN+%E2%80%94+ALL'S+RIGHT+WITH+THE+WORLD" />

<img src="https://komarev.com/ghpvc/?username=junkkyass-bit&label=PROFILE+VIEWS&color=c1121f&style=flat" />
<img src="https://img.shields.io/github/followers/junkkyass-bit?label=FOLLOWERS&style=flat&color=00b4d8" />
<img src="https://img.shields.io/badge/STATUS-ACTIVELY%20BUILDING-00ff88?style=flat" />

</div>

---

\`\`\`javascript
const zakaria = {
  name:     "Zakaria Moumsik",
  github:   "junkkyass-bit",
  status:   "ACTIVELY BUILDING",  // not training. doing.
  sync:     99.8,
  core:     "Dynamic, data-driven web applications",
  stack: {
    frontend: ["HTML5","CSS3","JS","jQuery","AJAX","React","Next.js","Three.js","Tailwind"],
    backend:  ["Node.js", "PHP", "Python"],
    database: ["MySQL"],
    infra:    ["Linux", "Git", "GitHub", "npm"],
  },
  currentlyBuilding: [
    "Full-stack dynamic apps (PHP + MySQL + AJAX)",
    "3D web experiences with Three.js",
    "REST APIs with Node.js",
  ],
  mission: "Ship dynamic websites. Every day.",
};
\`\`\`

---

## ⚙️ Tech Stack

### Frontend
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

### Backend & Database
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)

### Infrastructure
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)
![NPM](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)

---

## 🔴 Active Operations

| CODE | MISSION | STACK | STATUS |
|------|---------|-------|--------|
| OP-001 | Dynamic CRUD App | PHP + MySQL + AJAX + jQuery | 🟢 SHIPPING |
| OP-002 | REST API Service | Node.js + MySQL + JSON | 🟢 SHIPPING |
| OP-003 | 3D Portfolio Site | Three.js + Next.js | 🔵 IN PROGRESS |
| OP-004 | React Dashboard | React + AJAX + PHP | 🔵 IN PROGRESS |

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=junkkyass-bit&show_icons=true&theme=midnight-purple&hide_border=true&count_private=true&title_color=00b4d8&icon_color=c1121f&text_color=e8e8e8&bg_color=0a0a0f" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=junkkyass-bit&theme=dark&hide_border=true&background=0a0a0f&ring=00b4d8&fire=c1121f&currStreakLabel=00b4d8" width="48%" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=junkkyass-bit&layout=compact&theme=midnight-purple&hide_border=true&bg_color=0a0a0f&title_color=00b4d8&text_color=e8e8e8" width="40%" />
</p>

---

## 📡 Pilot Transmission

> *"I don't build static pages.*
> *I build systems that breathe — forms that submit without reloading,*
> *databases that talk back, interfaces that update in real time.*
> *Dynamic is not a feature. It's the standard."*
>
> **— ZAKARIA MOUMSIK // junkkyass-bit // SYNC: 99.8%**

---

## 🔗 Connect

<p align="left">
  <a href="mailto:YOUR_EMAIL"><img src="https://img.shields.io/badge/EMAIL-c1121f?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/YOUR_PROFILE"><img src="https://img.shields.io/badge/LINKEDIN-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://twitter.com/YOUR_HANDLE"><img src="https://img.shields.io/badge/TWITTER-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white"/></a>
</p>

---

<div align="center">
  <sub>NERV TECHNICAL DIVISION · junkkyass-bit · MOROCCO BRANCH</sub><br/>
  <sub><i>GOD'S IN HIS HEAVEN — ALL'S RIGHT WITH THE WORLD</i></sub>
</div>`;

document.getElementById('readme-out').textContent = readme;

function copyIt(){
  navigator.clipboard.writeText(readme).then(()=>{
    const btn = document.getElementById('copy-btn');
    btn.textContent = '[COPIED — PASTE INTO README.MD]';
    setTimeout(()=>{ btn.textContent = '[COPY README.MD]'; }, 2500);
  }).catch(()=>{
    const ta = document.createElement('textarea');
    ta.value = readme;
    document.body.appendChild(ta);
    ta.select();
    document.execCommand('copy');
    document.body.removeChild(ta);
    const btn = document.getElementById('copy-btn');
    btn.textContent = '[COPIED!]';
    setTimeout(()=>{ btn.textContent = '[COPY README.MD]'; }, 2500);
  });
}
</script>
</body>
</html>
