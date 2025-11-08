# Viksit-Bharat
Viksit Bharat portal
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Viksit Bharat Portal</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Merriweather:wght@700&display=swap');
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(180deg, #fff7e0 0%, #ffffff 30%, #e9fff2 100%);
      color: #222;
      overflow-x: hidden;
      position: relative;
    }

    body::before {
      content: "";
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: linear-gradient(180deg, #ff9933 33%, #ffffff 33%, #ffffff 66%, #138808 66%);
      opacity: 0.15;
      animation: wave 8s ease-in-out infinite;
      z-index: -1;
    }

    @keyframes wave {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    header {
      text-align: center;
      padding: 2rem 1rem;
      background: linear-gradient(90deg, #ff9933, #ffffff, #138808);
      border-bottom: 4px solid #000080;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    header h1 {
      font-family: 'Merriweather', serif;
      font-size: 2.8rem;
      color: #000080;
      text-shadow: 1px 1px 2px #fff;
    }

    header p {
      font-style: italic;
      font-size: 1.1rem;
    }

    nav {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 1rem;
      margin-top: 1rem;
    }

    nav a {
      text-decoration: none;
      color: #fff;
      background: #000080;
      padding: 0.6rem 1.2rem;
      border-radius: 30px;
      transition: 0.3s;
      box-shadow: 0 0 8px rgba(0,0,0,0.2);
    }

    nav a:hover {
      background: #ff9933;
      color: #000;
      transform: scale(1.05);
    }

    .hero {
      text-align: center;
      padding: 4rem 1rem;
      position: relative;
      background: url('https://upload.wikimedia.org/wikipedia/commons/3/37/India_Gate_in_New_Delhi_03-2016_img3.jpg') center/cover no-repeat;
      border-radius: 0 0 40px 40px;
      color: #fff;
      text-shadow: 1px 1px 4px #000;
      animation: fadeIn 2s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .hero::after {
      content: "";
      position: absolute;
      top: 0; left: 0; width: 100%; height: 100%;
      background: rgba(0,0,0,0.4);
      border-radius: 0 0 40px 40px;
      z-index: 0;
    }

    .hero h2, .hero p, .cta-row { position: relative; z-index: 1; }

    .hero h2 { font-size: 2.5rem; color: #fff; }

    .cta-row { margin-top: 1.5rem; }

    .btn {
      background: #138808;
      color: #fff;
      padding: 0.7rem 1.4rem;
      border-radius: 25px;
      text-decoration: none;
      margin: 0.4rem;
      display: inline-block;
      transition: 0.3s;
      box-shadow: 0 0 10px rgba(0,0,0,0.3);
    }

    .btn:hover { background: #ff9933; transform: translateY(-3px); }

    .btn.outline { background: transparent; border: 2px solid #fff; color: #fff; }

    main {
      padding: 2rem 1rem;
      display: grid;
      gap: 2rem;
      max-width: 1000px;
      margin: auto;
    }

    section.card {
      background: #fff;
      padding: 1.5rem;
      border-radius: 15px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      border-top: 4px solid #ff9933;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    section.card:hover { transform: scale(1.02); box-shadow: 0 4px 15px rgba(0,0,0,0.2); }

    section h3 { color: #000080; margin-bottom: 1rem; }

    ul, ol { margin-left: 1.5rem; line-height: 1.8; }

    .grid {
      display: grid;
      gap: 1rem;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    }

    .tile {
      background: #f0f9ff;
      padding: 1rem;
      border-radius: 10px;
      border-left: 4px solid #138808;
      transition: 0.3s;
    }

    .tile:hover { background: #e6ffe6; transform: scale(1.03); }

    .feedback textarea, form textarea {
      width: 100%; padding: 0.7rem; border-radius: 8px; border: 1px solid #ccc; margin-top: 0.5rem; resize: vertical; font-family: inherit;
    }

    input {
      width: 100%; padding: 0.6rem; margin-top: 0.3rem; border: 1px solid #ccc; border-radius: 6px; font-family: inherit;
    }

    .form-actions { margin-top: 1rem; }

    footer {
      text-align: center; padding: 1rem; background: linear-gradient(90deg, #138808, #ffffff, #ff9933); color: #000; margin-top: 2rem; border-top: 4px solid #000080; font-weight: 600;
    }

    footer p { text-shadow: 1px 1px 2px #fff; }
  </style>
</head>
<body>
  <header>
    <h1>🇮🇳 Viksit Bharat 🇮🇳</h1>
    <p>Vision • Initiatives • Participation</p>
    <nav>
      <a href="#home">Home</a>
      <a href="#vision">Vision 2047</a>
      <a href="#initiatives">Initiatives</a>
      <a href="#projects">Projects & Work</a>
      <a href="#participation">Participation</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section id="home" class="hero">
      <h2>Welcome to Viksit Bharat</h2>
      <p>Together, we are shaping a strong, self-reliant, and inclusive India by 2047.</p>
      <div class="cta-row">
        <a class="btn" href="#vision">Our Vision</a>
        <a class="btn outline" href="#participation">Get Involved</a>
      </div>
    </section>

    <section id="vision" class="card">
      <h3>Vision 2047</h3>
      <p>By 2047, India will emerge as a global leader — prosperous, green, and driven by innovation and unity.</p>
      <ul>
        <li>Economic growth and employment for all</li>
        <li>Accessible education and healthcare</li>
        <li>Sustainability and environmental harmony</li>
      </ul>
    </section>

    <section id="initiatives" class="card">
      <h3>Key Initiatives</h3>
      <div class="grid">
        <div class="tile"><h4>Digital India</h4><p>Empowering citizens through technology and transparency.</p></div>
        <div class="tile"><h4>Skill Bharat</h4><p>Preparing youth for innovation and global opportunities.</p></div>
        <div class="tile"><h4>Green Mission</h4><p>Renewable energy and clean environment initiatives.</p></div>
        <div class="tile"><h4>Health for All</h4><p>Universal and affordable healthcare for every Indian.</p></div>
      </div>
    </section>

    <section id="projects" class="card">
      <h3>Links – Ongoing Projects & Work</h3>
      <p>Explore key ongoing national projects shaping a Viksit Bharat:</p>
      <ul>
        <li><a href="https://www.pppinindia.gov.in/infrastructure_projects_statewise" target="_blank">Infrastructure Projects – PPP India</a></li>
        <li><a href="https://www.investindia.gov.in/team-india-blogs/10-indian-mega-projects-are-redefining-infrastructure-2025" target="_blank">10 Indian Mega Projects Transforming India 2025</a></li>
        <li><a href="https://en.wikipedia.org/wiki/Amrit_Bharat_Station_Scheme" target="_blank">Amrit Bharat Station Scheme – Indian Railways</a></li>
        <li><a href="https://www.projectstoday.com/" target="_blank">Projects Today – Real-time Project Tracker</a></li>
      </ul>
    </section>

    <section id="participation" class="card">
      <h3>Citizen Participation</h3>
      <p>Development thrives when citizens engage actively. Here’s how you can join in:</p>
      <ol>
        <li>Volunteer locally to strengthen your community.</li>
        <li>Engage in public discussions and policy feedback.</li>
        <li>Share your ideas and suggestions for change.</li>
      </ol>
      <div class="feedback">
        <h4>Quick Feedback</h4>
        <textarea placeholder="Share your suggestion or feedback..."></textarea>
        <button class="btn">Submit (Demo)</button>
      </div>
    </section>

    <section id="contact" class="card">
      <h3>Contact / Feedback</h3>
      <form>
        <label>Name <input type="text" required></label>
        <label>Email <input type="email" required></label>
        <label>Message <textarea rows="5" required></textarea></label>
        <div class="form-actions">
          <button class="btn" type="submit">Send (Demo)</button>
          <button class="btn outline" type="reset">Reset</button>
        </div>
      </form>
    </section>
  </main>

  <footer>
    <p>© Viksit Bharat — Built with ❤️ for a Stronger India</p>
  </footer>
</body>
</html>


Here’s your finished Viksit Bharat Portal — a colorful, animated, and interactive static website you
