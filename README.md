# ankitportfolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ankit Kumar Sonu | Portfolio</title>

  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Segoe UI", sans-serif;
    }

    body {
      background: #0f172a;
      color: #e5e7eb;
      scroll-behavior: smooth;
    }

    /* Navbar */
    header {
      position: fixed;
      width: 100%;
      top: 0;
      background: #020617;
      padding: 15px 40px;
      z-index: 1000;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    nav h2 {
      color: #38bdf8;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
    }

    nav a {
      color: #e5e7eb;
      text-decoration: none;
      transition: 0.3s;
    }

    nav a:hover {
      color: #38bdf8;
    }

    /* Hero */
    .hero {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0 20px;
    }

    .hero-card {
      display: flex;
      background: #020617;
      padding: 30px;
      border-radius: 20px;
      align-items: center;
      gap: 30px;
      max-width: 900px;
      width: 100%;
      flex-wrap: wrap;
      text-align: left;
      box-shadow: 0 10px 30px rgba(0,0,0,0.5);
    }

    .hero-card img {
      width: 150px;
      height: 150px;
      border-radius: 10px;
      object-fit: cover;
      border: 3px solid #38bdf8;
    }

    .hero-content h1 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    .hero-content h1 span {
      color: #38bdf8;
    }

    .typing {
      margin-top: 10px;
      font-size: 20px;
      color: #94a3b8;
      height: 24px;
    }

    .hero-content button {
      margin-top: 20px;
      padding: 12px 30px;
      border: none;
      border-radius: 30px;
      background: #38bdf8;
      color: #020617;
      cursor: pointer;
      font-size: 16px;
      transition: 0.3s;
    }

    .hero-content button:hover {
      transform: scale(1.05);
      box-shadow: 0 0 20px #38bdf8;
    }

    /* Sections */
    section {
      padding: 100px 10%;
      text-align: center;
    }

    section h2 {
      font-size: 32px;
      margin-bottom: 20px;
      color: #38bdf8;
    }

    /* About */
    .about p {
      max-width: 700px;
      margin: auto;
      line-height: 1.6;
      color: #cbd5f5;
    }

    /* Projects */
    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
      margin-top: 40px;
    }

    .card {
      background: #020617;
      padding: 25px;
      border-radius: 15px;
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 25px rgba(56,189,248,0.4);
    }

    .card-image {
      display: block;
      width: 100%;
      height: 140px;
      margin-bottom: 15px;
      border-radius: 10px;
      overflow: hidden;
    }

    .card-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.3s ease;
    }

    .card-image:hover img {
      transform: scale(1.08);
    }

    /* Contact */
    .contact p {
      margin: 10px 0;
    }

    .social-links {
      margin-top: 20px;
    }

    .social-links a {
      color: #e5e7eb;
      font-size: 28px;
      margin: 0 15px;
      transition: 0.3s;
    }

    .social-links a:hover {
      color: #38bdf8;
      transform: scale(1.2);
    }

    /* Footer */
    footer {
      background: #020617;
      text-align: center;
      padding: 20px;
    }

    /* Scroll animation */
    .hidden {
      opacity: 0;
      transform: translateY(40px);
      transition: 0.8s ease;
    }

    .show {
      opacity: 1;
      transform: translateY(0);
    }

    /* Responsive */
    @media (max-width: 768px) {
      nav ul {
        gap: 15px;
      }

      .hero-card {
        flex-direction: column;
        text-align: center;
        gap: 20px;
      }

      .hero-card img {
        width: 120px;
        height: 120px;
      }
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <header>
    <nav>
      <h2>Ankit Kumar Sonu</h2>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#Education">Education</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero -->
  <section id="home" class="hero">
    <div class="hero-card">
      <img src="image/ankitt.jpg" alt="Ankit Kumar Sonu">
      <div class="hero-content">
        <h1>Hi, I'm <span>Ankit Kumar Sonu</span></h1>
        <div class="typing" id="typing"></div>
        <button onclick="scrollToSection('projects')">View My Work</button>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="about hidden">
    <h2>About Me</h2>
    <p>
      I am Ankit Kumar Sonu, having Bachelor’s and Master’s degrees in Computer Applications
      (2021 & 2023) from L. N. Mishra Institute, Patna.  
      I'm a software engineer with a keen eye for design and a love for creating seamless 
      user experiences. Through a combination of clean code, modern technologies, and a deep 
      understanding of user needs, I craft stunning websites that captivate and engage visitors.
      <br><br>
      I have expertise in HTML, CSS, JavaScript, and frontend frameworks. I enjoy building interactive,
      responsive websites and continuously learning new technologies to deliver the best experience.
    </p>
  </section>

  <!-- Projects -->
  <section id="projects" class="hidden">
    <h2>Projects</h2>

    <div class="projects">
      <div class="card">
        <a href="https://gymtrainerpatna.netlify.app/" target="_blank" class="card-image">
          <img src="/image/Screenshot (16).png">
        </a>
        <h3>Gym trainer website </h3>
        <p>Web application built using HTML, CSS, JavaScript.</p>
        <p>The Gym Website Project aims to provide a user-friendly platform for gym enthusiasts. 
            <br>The website allows users to sign up and log in to access various features and resources
             related to fitness and workouts.
        </p>
      </div>

      <div class="card">
        <a href="https://quizwhiz.vercel.app/" target="_blank" class="card-image">
          <img src="/image/Screenshot (18).png" >
        </a>
        <h3>Quiz website</h3>
        <p>Interactive quiz application with dynamic UI.</p>
        <p>An online quiz website is a web-based application designed to deliver interactive tests, 
            trivia, or surveys, allowing users to measure knowledge, engage with content, or test skills
             in real-time. These platforms serve a variety of purposes, ranging from educational 
             assessment in schools to entertainment-driven quizzes, corporate training, and personality 
             tests.
        </p>
      </div>

      <div class="card">
        <a href="https://kanbanboard-tg5u.onrender.com/" target="_blank" class="card-image">
          <img src="image/Screenshot (13).png" alt="Kanban Board">
        </a>
        <h3>Kanban Board</h3>
        <p>Task management board with JavaScript logic.</p>
        <p>Kanban Group Project: This is a collaborative Kanban board project developed by me. 
            The purpose of this project is to create a digital 
            Kanban board using React JS and implement drag-and-drop functionality for managing tasks and
             workflows.
        </p>
      </div>
    </div>
  </section>

  <!-- Education -->
  <section id="Education" class="hidden">
    <h2>Education</h2>
    <div class="projects">
      <div class="card">
        <h3>PGDAC</h3>
        <p>Postgraduate Diploma in Advanced Computing</p>
        <p>from CDAC NOIDA IN 2025</p>
      </div>
      <div class="card">
        <h3>MCA</h3>
        <p>Master of Computer Applications</p>
        <p>from L N MISHRA Institute PATNA IN 2023 and got 7.79 CGPA</p>
      </div>
      <div class="card">
        <h3>BCA</h3>
        <p>Bachelor of Computer Applications</p>
        <p>from L N MISHRA INSTITUTE PATNA IN 2021 and got 71% marks</p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="contact hidden">
    <h2>Contact Details</h2>
    <p>Email: ankitkumarsonu0@gmail.com</p>
    <p>Phone: 9852743125</p>

    <div class="social-links">
      <a href="https://github.com/ankitcodehub45" target="_blank">
        <i class="fab fa-github"></i>
      </a>
      <a href="https://www.linkedin.com/in/ankit-kumar-sonu-425a2924a/" target="_blank">
        <i class="fab fa-linkedin"></i>
      </a>
      <a href="https://x.com/kumar_sonu63389" target="_blank">
        <i class="fab fa-twitter"></i>
      </a>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2026 Ankit Kumar Sonu. All rights reserved.</p>
  </footer>

  <!-- Scripts -->
  <script>
    // Smooth scroll
    function scrollToSection(id) {
      document.getElementById(id).scrollIntoView({ behavior: "smooth" });
    }

    // Typing effect
    const text = ["Web Developer", "Frontend Developer", "Software Engineer"];
    let index = 0, char = 0;
    const typingEl = document.getElementById("typing");

    function typeEffect() {
      if (char < text[index].length) {
        typingEl.textContent += text[index].charAt(char);
        char++;
        setTimeout(typeEffect, 100);
      } else {
        setTimeout(eraseEffect, 2000);
      }
    }

    function eraseEffect() {
      if (char > 0) {
        typingEl.textContent = text[index].substring(0, char - 1);
        char--;
        setTimeout(eraseEffect, 60);
      } else {
        index = (index + 1) % text.length;
        setTimeout(typeEffect, 500);
      }
    }

    typeEffect();

    // Scroll reveal animation
    const hiddenElements = document.querySelectorAll(".hidden");
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("show");
        }
      });
    }, { threshold: 0.2 });

    hiddenElements.forEach(el => observer.observe(el));
  </script>

</body>
</html>
