
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Protfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to right, #141e30, #243b55);
      color: #fff;
      line-height: 1.6;
    }

    header {
      background: rgba(0, 0, 0, 0.7);
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      color: #00c6ff;
    }

    nav a {
      margin: 0 1rem;
      color: #fff;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #00c6ff;
    }

    section {
      padding: 60px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .home {
      text-align: center;
      padding-top: 100px;
    }

    .home h2 {
  font-size: 3rem;
  background: linear-gradient(to right, #00c6ff, #0072ff);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  color: transparent;
  display: inline-block;
  margin-bottom: 20px;
}


    .home p {
      font-size: 1.2rem;
      color: #ccc;
    }

    .about, .projects, .contact, .skills, .blog {
      background: rgba(255, 255, 255, 0.05);
      margin: 40px 0;
      border-radius: 10px;
      padding: 40px 20px;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
    }

    .skills .skill {
      margin-bottom: 20px;
    }

    .skills .skill span {
      display: inline-block;
      margin-bottom: 5px;
    }

    .bar {
      width: 100%;
      background: #333;
      border-radius: 10px;
      overflow: hidden;
    }

    .bar-fill {
      height: 20px;
      background: linear-gradient(to right, #00c6ff, #0072ff);
      width: 0;
      animation: fill 2s forwards;
    }

    @keyframes fill {
      to { width: var(--fill); }
    }

    .projects .card {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }

    .projects .item {
      flex: 1 1 calc(33.333% - 20px);
      background: #1e2a38;
      padding: 20px;
      border-radius: 10px;
      transition: transform 0.3s ease;
    }

    .projects .item:hover {
      transform: scale(1.05);
    }

    .blog .testimonial {
      background: #1a1a1a;
      padding: 20px;
      margin-top: 20px;
      border-left: 5px solid #00c6ff;
    }

    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: none;
      border-radius: 5px;
    }

    form button {
      padding: 10px 20px;
      background: #00c6ff;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    form button:hover {
      background: #0072ff;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #111;
    }

    @media (max-width: 768px) {
      .projects .item {
        flex: 1 1 100%;
      }

      nav a {
        margin: 0 0.5rem;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Protofolio</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#blog">Blog</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="home" id="home">
    <h2>Welcome to Mruganshi's Protfolio</h2>
    <p>My one-stop showcase of creativity, projects, and professionalism.</p>
  </section>

  <section class="about" id="about">
    <h2>About Me</h2>
    <p>I am currently pursuing engineering and have a deep interest in the intersection of software and hardware. Whether it’s a smart road divider or a full-stack learning platform, I enjoy the challenge of making things that matter.</p>
  </section>

  <section class="skills" id="skills">
    <h2>Skills</h2>
    <div class="skill">
      <span>HTML</span>
      <div class="bar"><div class="bar-fill" style="--fill: 90%;"></div></div>
    </div>
    <div class="skill">
      <span>CSS</span>
      <div class="bar"><div class="bar-fill" style="--fill: 85%;"></div></div>
    </div>
    <div class="skill">
      <span>JavaScript</span>
      <div class="bar"><div class="bar-fill" style="--fill: 75%;"></div></div>
    </div>
  </section>

  <section class="projects" id="projects">
    <h2>Projects</h2>
    <div class="card">
      <div class="item"><h3>Smart Road Divider</h3><p>IoT-based dynamic lane management system using sensors and microcontrollers for real-time traffic optimization and road safety improvements.</p></div>
      <div class="item"><h3>Startup Website</h3><p>Developed a fast, responsive website for a startup with animated components, custom branding, and mobile-first design using HTML5, CSS3, and JS.</p></div>
      <div class="item"><h3>E-Learning Website</h3><p>Created an online education platform with interactive course listings, smooth navigation, and responsive layout for all screen sizes.</p></div>
    </div>
  </section>

  <section class="blog" id="blog">
    <h2>Testimonials</h2>
    <div class="testimonial">
      <p>"Working with Protofolio was a fantastic experience. The website exceeded our expectations!"</p>
      <strong>- Client A</strong>
    </div>
    <div class="testimonial">
      <p>"Creative, professional, and always on time. Highly recommend!"</p>
      <strong>- Client B</strong>
    </div>
  </section>

  <section class="contact" id="contact">
    <h2>Contact Me</h2>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>
  <section id="contact">
    <h2>Contact</h2>
    <p>Email: your.email@example.com</p>
    <p>LinkedIn: linkedin.com/in/yourprofile</p>
    <p>GitHub: github.com/yourusername</p>
  </section>  <footer>
    <p>&copy; 2025 Mruganshi. Designed with passion and precision.</p>
  
  </footer>

</body>
</html>
# credora
