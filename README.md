<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mahabub Hasan | IT Project Manager</title>

  <!-- Fonts & Icons -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <link href="https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css" rel="stylesheet">

  <style>
    *{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif}
    html{scroll-behavior:smooth}
    body{background:#0f172a;color:#e5e7eb}

    /* NAV */
    header.nav{
      position:fixed;top:0;width:100%;z-index:1000;
      background:#020617cc;backdrop-filter:blur(10px);
      display:flex;justify-content:space-between;align-items:center;
      padding:16px 10%;
    }
    header.nav h2{color:#fff}
    header.nav ul{display:flex;gap:25px;list-style:none}
    header.nav a{color:#93c5fd;text-decoration:none;font-weight:500}
    header.nav a:hover{color:#fff}

    /* HERO */
    .hero{
      min-height:100vh;display:flex;align-items:center;justify-content:center;
      background:radial-gradient(circle at top,#2563eb,#020617);
      text-align:center;padding:40px;
    }
    .hero img{
      width:180px;height:180px;border-radius:50%;border:4px solid #60a5fa;
      margin-bottom:20px;object-fit:cover;
    }
    .hero h1{font-size:3.3rem}
    .hero h3{font-weight:400;color:#bfdbfe}

    .btn{
      display:inline-block;margin:15px 8px;padding:12px 30px;
      border-radius:30px;font-weight:600;text-decoration:none;transition:.3s;
    }
    .btn.primary{background:#2563eb;color:#fff}
    .btn.primary:hover{background:#1d4ed8}
    .btn.outline{border:2px solid #2563eb;color:#bfdbfe}
    .btn.outline:hover{background:#2563eb;color:#fff}

    section{padding:100px 12%}
    h2{text-align:center;font-size:2.4rem;margin-bottom:40px;color:#60a5fa}

    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:30px}
    .card{
      background:#020617;padding:30px;border-radius:18px;
      box-shadow:0 15px 35px rgba(0,0,0,.4);
    }

    .skills span{
      display:inline-block;background:#1e3a8a;padding:10px 18px;
      border-radius:22px;margin:8px;font-size:.9rem
    }

    footer{text-align:center;padding:40px;background:#020617;color:#9ca3af}

    .reveal{opacity:0;transform:translateY(40px);transition:.8s}
    .reveal.active{opacity:1;transform:none}
  </style>
</head>
<body>

<header class="nav">
  <h2>Mahabub</h2>
  <i class='bx bx-menu' id="menu-icon"></i>
  <ul id="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#education">Education</a></li>
    <li><a href="#certifications">Certification</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</header>

<section class="hero">
  <div>
    <img src="profile.jpg" alt="Mahabub Hasan">
    <h3>Hello, I'm</h3>
    <h1>Mahabub Hasan</h1>
    <h3>IT Project Manager & Senior Project Coordinator</h3>
    <a href="Mahabub_Hasan_CV.pdf" class="btn primary" download>Download CV</a>
    <a href="#contact" class="btn outline">Contact Info</a>
    <div style="margin-top:20px;font-size:1.8rem">
      <a href="https://www.linkedin.com/in/mahabubhasan-it" target="_blank"><i class='bx bxl-linkedin'></i></a>
      <a href="https://github.com/mtechhasan-it" target="_blank"><i class='bx bxl-github'></i></a>
    </div>
  </div>
</section>

<section id="about" class="reveal">
  <h2>About Me</h2>
  <div class="card">
    <p>Results-driven IT Project Manager with experience leading cross-functional teams, managing Agile & Waterfall projects, coordinating stakeholders, and delivering technology solutions on time and within scope.</p>
  </div>
</section>

<section id="experience" class="reveal">
  <h2>Experience</h2>
  <div class="grid">
    <div class="card"><h3>Senior Project Coordinator</h3><p>UpSkill Consultancy Inc</p></div>
    <div class="card"><h3>IT Project Coordinator</h3><p>Mahadev International LLC</p></div>
    <div class="card"><h3>Graduate Assistant</h3><p>Touro University</p></div>
    <div class="card"><h3>Project Associate</h3><p>Lux Sourcing Limited</p></div>
  </div>
</section>

<section id="skills" class="reveal">
  <h2>Skills</h2>
  <div class="card skills">
    <span>Agile</span><span>Scrum</span><span>Jira</span><span>Risk Management</span>
    <span>SQL</span><span>Python</span><span>Stakeholder Management</span>
  </div>
</section>

<section id="projects" class="reveal">
  <h2>Projects</h2>
  <div class="grid">
    <div class="card">Food Waste Reduction Program</div>
    <div class="card">Online Learning Platform</div>
  </div>
</section>

<section id="education" class="reveal">
  <h2>Education</h2>
  <div class="grid">
    <div class="card">M.S. in Information Systems – Touro University</div>
    <div class="card">B.S. Degree – BGMEA University</div>
  </div>
</section>

<section id="certifications" class="reveal">
  <h2>Certifications</h2>
  <div class="card">Google PM · IBM PM · Google Cybersecurity · Agile PM</div>
</section>

<section id="contact" class="reveal">
  <h2>Contact</h2>
  <div class="card">
    <p>Email: mtechhasan.it@gmail.com</p>
    <p>LinkedIn: mahabubhasan-it</p>
  </div>
</section>

<footer>
  <p>© 2024 Mahabub Hasan. All Rights Reserved.</p>
</footer>

<script>
  const reveals=document.querySelectorAll('.reveal');
  window.addEventListener('scroll',()=>{
    reveals.forEach(el=>{
      if(el.getBoundingClientRect().top < window.innerHeight-100){
        el.classList.add('active');
      }
    });
  });
</script>

</body>
</html>
