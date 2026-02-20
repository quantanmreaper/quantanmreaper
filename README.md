<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bhavin Mepani — Engineering Leverage</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
<style>
  /* Reset & Base */
  * { box-sizing: border-box; margin:0; padding:0; }
  body {
    font-family: 'Inter', sans-serif;
    background: #0f0f15;
    color: #eee;
    overflow-x: hidden;
  }
  a { color: #7f5af0; text-decoration: none; transition: 0.3s; }
  a:hover { color: #b692f6; }

  /* Parallax background layers */
  .bg-layer {
    position: fixed;
    width: 150%;
    height: 150%;
    top: -25%;
    left: -25%;
    pointer-events: none;
    background-repeat: no-repeat;
    background-position: center;
    z-index: -2;
  }
  .bg-layer.layer1 { background: radial-gradient(circle at 20% 30%, rgba(127,90,255,0.05), transparent 70%); }
  .bg-layer.layer2 { background: radial-gradient(circle at 80% 70%, rgba(127,90,255,0.07), transparent 70%); }

  /* Container */
  .container { max-width: 900px; margin:0 auto; padding:4rem 1rem; position: relative; z-index: 1; }

  /* Header */
  .header { text-align: center; margin-bottom: 3rem; }
  .header svg { width: 120px; height: 120px; margin-bottom: 1rem; }
  .header svg circle {
    stroke-dasharray: 302;
    stroke-dashoffset: 302;
    stroke:#7f5af0;
    stroke-width:4;
    fill:none;
    animation: draw 2s forwards ease-out;
  }
  .header svg path {
    transform-origin: 50% 50%;
    transform-box: fill-box;
    fill:#7f5af0;
    opacity:0.2;
    animation: pulse 3s infinite alternate;
  }
  @keyframes draw { to { stroke-dashoffset:0; } }
  @keyframes pulse { 0% { opacity:0.2; transform:scale(1);} 100%{opacity:0.5; transform:scale(1.05);} }

  .header h1, .header h3 { opacity:0; animation: fadeIn 1s forwards; }
  .header h1 { animation-delay:2s; font-size:2.8rem; font-weight:700; letter-spacing:1px; color:#fff; }
  .header h3 { animation-delay:2.5s; font-weight:400; color:#aaa; letter-spacing:1.5px; margin-top:0.25rem; }
  @keyframes fadeIn { to { opacity:1; } }

  hr {
    border:none; height:2px; border-radius:1px;
    background: linear-gradient(to right, #7f5af0, #b692f6);
    margin:2rem 0; opacity:0; transform:translateX(-50px);
    animation: slideIn 1s forwards 3s;
  }
  @keyframes slideIn { to { opacity:1; transform:translateX(0); } }

  /* Section cards */
  section {
    background: rgba(255,255,255,0.03);
    backdrop-filter: blur(12px);
    border-radius:16px;
    padding:2rem;
    margin-bottom:2.5rem;
    box-shadow:0 10px 30px rgba(127,90,255,0.1);
    transform:translateY(30px);
    opacity:0;
    transition: all 0.8s cubic-bezier(0.25,1,0.5,1);
    cursor:default;
  }
  section.visible { transform:translateY(0); opacity:1; }
  section:hover { transform:translateY(-5px) scale(1.02); box-shadow:0 15px 40px rgba(127,90,255,0.25); }

  section h2 {
    font-size:1.8rem; margin-bottom:0.75rem; color:#fff; position:relative; transition:0.3s;
  }
  section h2::after {
    content:''; display:block; width:40px; height:2px; background:#7f5af0; margin-top:6px; border-radius:2px; transition:width 0.3s;
  }
  section:hover h2::after { width:60px; }
  section:hover h2 { color:#b692f6; }

  p, ul { font-size:1rem; color:#ddd; margin:0.5rem 0 0 0; }
  ul { padding-left:1.2rem; }
  ul li { margin-bottom:0.5rem; }
  .highlight { color:#7f5af0; font-weight:600; }

  /* Footer */
  .footer { text-align:center; margin-top:3rem; font-size:1rem; color:#aaa; opacity:0; transform:translateY(20px); transition:0.6s ease-out; }
  .footer.visible { opacity:1; transform:translateY(0); }
  .footer a { font-weight:600; color:#7f5af0; }
</style>
</head>
<body>

<div class="bg-layer layer1"></div>
<div class="bg-layer layer2"></div>

<div class="container">

  <div class="header">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <circle cx="50" cy="50" r="48"/>
      <path d="M25 50 L50 25 L75 50 L50 75 Z"/>
    </svg>
    <h1>Bhavin Mepani</h1>
    <h3>Engineering Leverage</h3>
  </div>

  <hr/>

  <section>
    <h2>SYSTEMS. NOT FEATURES.</h2>
    <p>I build <span class="highlight">systems that compound</span>.</p>
    <p>Laravel is my structural backbone.<br>Python is my intelligence layer.</p>
    <p>I operate where backend architecture meets emerging AI.</p>
    <p>Not experimenting.<br>Specializing.</p>
  </section>

  <section>
    <h2>COMPETITIVE SIGNAL</h2>
    <p>Top-3 finish in every hackathon entered.</p>
    <p>But the medal is not the metric.</p>
    <p>Leadership under compression is.</p>
    <ul>
      <li>I bring structure into chaos.</li>
      <li>I turn time pressure into execution clarity.</li>
      <li>I ship.</li>
    </ul>
  </section>

  <section>
    <h2>CURRENT DIRECTION</h2>
    <ul>
      <li>Building a production-grade full-stack system at my internship.</li>
      <li>Designing scalable Laravel architecture.</li>
      <li>Engineering clean admin intelligence with Filament.</li>
      <li>Creating reactive interfaces with Livewire.</li>
    </ul>
    <p>Parallel focus:</p>
    <ul>
      <li>Deep specialization in Python, AI & Machine Learning.</li>
      <li>From using models → to architecting intelligent systems.</li>
    </ul>
  </section>

  <section>
    <h2>CORE STACK</h2>
    <ul>
      <li>Laravel</li>
      <li>Filament</li>
      <li>Livewire</li>
      <li>Python</li>
      <li>FastAPI</li>
    </ul>
    <p>No clutter.<br>No trend-chasing.<br>Just tools that scale.</p>
  </section>

  <section>
    <h2>OPERATING PRINCIPLES</h2>
    <ul>
      <li>Consistency compounds.</li>
      <li>Discipline scales.</li>
      <li>Systems outperform effort.</li>
      <li>Intelligence reduces friction.</li>
    </ul>
    <p>Lazy — in repetition.<br>Relentless — in execution.<br>Deterministic by design.</p>
  </section>

  <section>
    <h2>LONG TERM</h2>
    <ul>
      <li>Full-Stack Systems → Intelligent Infrastructure → AI-Driven Platforms</li>
    </ul>
    <p>I am not building projects.<br>I am building capability.</p>
  </section>

  <div class="footer">
    If you value precision over noise —<br>let’s build.<br><br>
    <a href="https://linkedin.com/in/Bhavin Mepani" target="_blank">LinkedIn</a>
  </div>

</div>

<script>
  // Scroll reveal
  const sections = document.querySelectorAll('section');
  const footer = document.querySelector('.footer');
  function reveal() {
    const trigger = window.innerHeight * 0.85;
    sections.forEach(sec => {
      if(sec.getBoundingClientRect().top < trigger){ sec.classList.add('visible'); }
    });
    if(footer.getBoundingClientRect().top < trigger){ footer.classList.add('visible'); }
  }
  window.addEventListener('scroll', reveal);
  window.addEventListener('load', reveal);

  // Parallax background
  window.addEventListener('mousemove', e=>{
    document.querySelector('.layer1').style.transform=`translate(${e.clientX*0.02}px, ${e.clientY*0.02}px)`;
    document.querySelector('.layer2').style.transform=`translate(${e.clientX*0.04}px, ${e.clientY*0.04}px)`;
  });
</script>

</body>
</html>
