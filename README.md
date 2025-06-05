<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Niel Jasper Arangote - Web Developer Portfolio showcasing skills in frontend development, design, and various web technologies."/>
  <meta name="keywords" content="web developer, frontend developer, portfolio, HTML, CSS, JavaScript, React"/>
  <meta name="author" content="Niel Jasper Arangote"/>
  
  <!-- Open Graph / Social Media Meta Tags -->
  <meta property="og:title" content="Niel Jasper Arangote - Web Developer Portfolio"/>
  <meta property="og:description" content="Portfolio showcasing web development and design projects"/>
  <meta property="og:image" content="images/your-photo.jpg"/>
  <meta property="og:url" content="[Your website URL]"/>
  
  <title>Jasper Niel Arangote - Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet"/>
  <link rel="stylesheet" href="styles.css"/>
  <!-- Add Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css"/>
</head>
<body>
  <!-- Theme toggle button -->
  <button id="theme-toggle" aria-label="Toggle dark mode" class="theme-toggle">
    <i class="fas fa-moon"></i>
  </button>

  <header>
    <nav>
      <div class="logo">JNA</div>
      <button class="mobile-menu-btn" aria-label="Toggle menu">
        <i class="fas fa-bars"></i>
      </button>
      <ul>
        <li><a href="#home" aria-current="page">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#certificates">Certificates</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section id="home" class="hero">
      <div class="hero-content">
        <img src="images/your-photo.jpg" alt="Niel Jasper Arangote" class="hero-img" loading="lazy">
        <h1>Hello, I'm Niel Jasper C. Arangote</h1>
        <p>Web Developer | Designer | Lifelong Learner</p>
        <a href="#contact" class="cta-button">Let's Connect</a>
        <div class="social-links">
          <a href="https://github.com/[your-username]" target="_blank" rel="noopener noreferrer" aria-label="GitHub Profile">
            <i class="fab fa-github"></i>
          </a>
          <a href="https://linkedin.com/in/[your-username]" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn Profile">
            <i class="fab fa-linkedin"></i>
          </a>
          <a href="https://twitter.com/[your-username]" target="_blank" rel="noopener noreferrer" aria-label="Twitter Profile">
            <i class="fab fa-twitter"></i>
          </a>
        </div>
      </div>
    </section>

    <section id="about">
      <h2>About Me</h2>
      <p>I'm a dedicated web developer focused on building responsive and engaging digital experiences. I specialize in frontend development and love turning ideas into reality using HTML, CSS, and JavaScript.</p>
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <div class="skills-list">
        <div class="skill">HTML</div>
        <div class="skill">CSS</div>
        <div class="skill">JavaScript</div>
        <div class="skill">React</div>
        <div class="skill">Bootstrap</div>
        <div class="skill">Git & GitHub</div>
      </div>
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <div class="project">
        <h3>Portfolio Website</h3>
        <p>A clean and responsive personal website to showcase my skills and work.</p>
      </div>
    </section>

    <section id="certificates">
      <h2>Certificates</h2>
      <ul>
        <li>Frontend Development Certificate - XYZ Institute</li>
        <li>JavaScript Fundamentals - ABC Academy</li>
      </ul>
    </section>

    <section id="contact">
      <h2>Contact Me</h2>
      <form action="https://formsubmit.co/your-email@example.com" method="POST">
        <!-- Honeypot -->
        <input type="text" name="_honey" style="display: none;">
        
        <!-- Disable Captcha -->
        <input type="hidden" name="_captcha" value="false">
        
        <!-- Success Page -->
        <input type="hidden" name="_next" value="https://yourdomain.com/thanks.html">
        
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" name="name" placeholder="Your Name" required 
                 minlength="2" maxlength="50"/>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" name="email" placeholder="Your Email" required 
                 pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$"/>
        </div>
        <div class="form-group">
          <label for="subject">Subject</label>
          <input type="text" id="subject" name="subject" placeholder="Subject" required/>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" name="message" placeholder="Your Message" required 
                    minlength="10" maxlength="500"></textarea>
        </div>
        <button type="submit" class="submit-btn">
          <span>Send Message</span>
          <i class="fas fa-paper-plane"></i>
        </button>
      </form>
    </section>
  </main>

  <footer>
    <div class="footer-content">
      <p>&copy; 2025 Niel Jasper C. Arangote. All rights reserved.</p>
      <div class="social-links">
        <a href="https://github.com/[your-username]" target="_blank" rel="noopener noreferrer" aria-label="GitHub Profile">
          <i class="fab fa-github"></i>
        </a>
        <a href="https://linkedin.com/in/[your-username]" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn Profile">
          <i class="fab fa-linkedin"></i>
        </a>
        <a href="https://twitter.com/[your-username]" target="_blank" rel="noopener noreferrer" aria-label="Twitter Profile">
          <i class="fab fa-twitter"></i>
        </a>
      </div>
    </div>
  </footer>

  <!-- Back to top button -->
  <button id="back-to-top" aria-label="Back to top" class="back-to-top">
    <i class="fas fa-arrow-up"></i>
  </button>

  <script>
    // Theme toggle functionality
    const themeToggle = document.getElementById('theme-toggle');
    themeToggle.addEventListener('click', () => {
      document.body.classList.toggle('dark-mode');
      const icon = themeToggle.querySelector('i');
      icon.classList.toggle('fa-moon');
      icon.classList.toggle('fa-sun');
    });

    // Mobile menu functionality
    const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
    const nav = document.querySelector('nav ul');
    mobileMenuBtn.addEventListener('click', () => {
      nav.classList.toggle('show');
    });

    // Back to top functionality
    const backToTop = document.getElementById('back-to-top');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 300) {
        backToTop.classList.add('show');
      } else {
        backToTop.classList.remove('show');
      }
    });
    backToTop.addEventListener('click', () => {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    });

    // Smooth scrolling for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });
  </script>
</body>
</html>