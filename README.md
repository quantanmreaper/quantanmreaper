<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bhavin Mepani — Engineering Leverage</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
<style>
  /* General Reset & Typography */
  body {
    margin: 0;
    font-family: 'Inter', sans-serif;
    background: #f5f5f5;
    color: #111;
    line-height: 1.6;
    overflow-x: hidden;
  }

  a {
    color: #4f46e5;
    text-decoration: none;
    transition: all 0.3s ease;
  }
  a:hover {
    text-decoration: underline;
    color: #6366f1;
  }

  /* Container */
  .container {
    max-width: 900px;
    margin: 0 auto;
    padding: 2rem 1rem;
  }

  /* Header */
  .header {
    text-align: center;
    margin-bottom: 2rem;
    position: relative;
  }

  /* Animated SVG Logo */
  .header svg circle {
    stroke-dasharray: 302;
    stroke-dashoffset: 302;
    animation: draw 2s forwards ease-out;
  }

  .header svg path {
    transform-origin: 50% 50%;
    transform-box: fill-box;
    animation: pulse 3s infinite alternate;
  }

  @keyframes draw {
    to { stroke-dashoffset: 0; }
  }

  @keyframes pulse {
    from { opacity: 0.2; transform: scale(1); }
    to { opacity: 0.5; transform: scale(1.05); }
  }

  .header h1 {
    margin: 0;
    font-size: 2.5rem;
    font-weight: 700;
    letter-spacing: 1px;
    opacity: 0;
    animation: fadeIn 1s forwards 2s;
  }

  .header h3 {
    margin: 0.25rem 0 0 0;
    font-weight: 400;
    color: #555;
    letter-spacing: 1.5px;
    opacity: 0;
    animation: fadeIn 1s forwards 2.5s;
  }

  @keyframes fadeIn {
    to { opacity: 1; }
  }

  hr {
    border: none;
    height: 2px;
    background: linear-gradient(to right, #4f46e5, #6366f1);
    margin: 2rem 0;
    border-radius: 1px;
    opacity: 0;
    transform: translateX(-50px);
    animation: slideIn 1s forwards 3s;
  }

  @keyframes slideIn {
    to { opacity: 1; transform: translateX(0); }
  }

  /* Sections */
  section {
    margin-bottom: 2rem;
    opacity: 0;
    transform: translateY(20px);
    transition: all 0.6s ease-out;
  }

  section.visible {
    opacity: 1;
    transform: translateY(0);
  }

  section h2 {
    font-size: 1.6rem;
    margin-bottom: 0.5rem;
    color: #222;
    position: relative;
    transition: color 0.3s;
  }

  section h2::after {
    content: '';
    display: block;
    width: 40px;
    height: 2px;
    background: #4f46e5;
    margin-top: 4px;
    border-radius: 1px;
    transition: width 0.3s;
  }

  section:hover h2::after {
    width: 60px;
  }

  section:hover h2 {
    color: #4f46e5;
  }

  p, ul {
    margin: 0.5rem 0 0 0;
    font-size: 1rem;
    color: #333;
  }

  ul {
    padding-left: 1.2rem;
  }

  ul li {
    margin-bottom: 0.5rem;
  }

  .highlight {
    color: #4f46e5;
    font-weight: 600;
  }

  /* Footer / Call to Action */
  .footer {
    text-align: center;
    margin-top: 3rem;
    font-size: 1rem;
    color: #555;
    opacity: 0;
    transform: translateY(20px);
    transition: all 0.6s ease-out;
  }

  .footer.visible {
    opacity: 1;
    transform: translateY(0);
  }

  .footer a {
    font-weight: 600;
  }

  /* Subtle decorative background */
  body::before {
    content: '';
    position: fixed;
    width: 100%;
    height: 100%;
    background: radial-gradient(circle at top left, rgba(79,70,229,0.05), transparent 70%);
    z-index: -1;
  }
</style>
</head>
<body>

<div class="container">

  <!-- Header with animated SVG -->
  <div class="header">
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
      <circle cx="50" cy="50" r="48" stroke="#4f46e5" stroke-width="4" fill="none" />
      <path d="M25 50 L50 25 L75 50 L50 75 Z" fill="#4f46e5" opacity="0.2"/>
    </svg>
    <h1>Bhavin Mepani</h1>
    <h3>Engineering Leverage</h3>
  </div>

  <hr/>

  <!-- SYSTEMS. NOT FEATURES -->
  <section>
    <h2>SYSTEMS. NOT FEATURES.</h2>
    <p>I build <span class="highlight">systems that compound</span>.</p>
    <p>Laravel is my structural backbone.<br>Python is my intelligence layer.</p>
    <p>I operate where backend architecture meets emerging AI.</p>
    <p>Not experimenting.<br>Specializing.</p>
  </section>

  <!-- COMPETITIVE SIGNAL -->
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

  <!-- CURRENT DIRECTION -->
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

  <!-- CORE STACK -->
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

  <!-- OPERATING PRINCIPLES -->
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

  <!-- LONG TERM -->
  <section>
    <h2>LONG TERM</h2>
    <ul>
      <li>Full-Stack Systems → Intelligent Infrastructure → AI-Driven Platforms</li>
    </ul>
    <p>I am not building projects.<br>I am building capability.</p>
  </section>

  <!-- Footer -->
  <div class="footer">
    If you value precision over noise —<br>let’s build.<br><br>
    <a href="https://linkedin.com/in/Bhavin Mepani" target="_blank">LinkedIn</a>
  </div>

</div>

<script>
  // Scroll reveal animation
  const sections = document.querySelectorAll('section');
  const footer = document.querySelector('.footer');

  const revealOnScroll = () => {
    const triggerBottom = window.innerHeight * 0.85;

    sections.forEach(section => {
      const top = section.getBoundingClientRect().top;
      if (top < triggerBottom) {
        section.classList.add('visible');
      }
    });

    if (footer.getBoundingClientRect().top < triggerBottom) {
      footer.classList.add('visible');
    }
  };

  window.addEventListener('scroll', revealOnScroll);
  window.addEventListener('load', revealOnScroll);
</script>

</body>
</html>
