## From Chatgpt
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  ## Madison Conley | Portfolio
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet"/>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    :root 
    {
      --pink-lightest: #FBEAF0;
      --pink-light: #F4C0D1;
      --pink-mid: #ED93B1;
      --pink-strong: #D4537E;
      --pink-dark: #993556;
      --pink-text: #72243E;
      --white: #ffffff;
    }
    body { font-family: 'DM Sans', sans-serif; background: var(--white); color: #333; }
    nav { background: var(--white); border-bottom: 1px solid var(--pink-light); padding: 1rem 2.5rem; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 100; }
    .nav-name { font-family: 'Playfair Display', serif; font-size: 20px; color: var(--pink-text); }
    .nav-links { display: flex; gap: 2rem; list-style: none; }
    .nav-links a { font-size: 14px; color: var(--pink-dark); text-decoration: none; transition: color 0.2s; }
    .nav-links a:hover { color: var(--pink-text); }
    .hero { background: var(--pink-lightest); padding: 5rem 2rem; text-align: center; border-bottom: 1px solid var(--pink-light); }
    .avatar { width: 100px; height: 100px; border-radius: 50%; background: var(--pink-strong); display: flex; align-items: center; justify-content: center; font-size: 32px; font-weight: 500; color: var(--pink-lightest); margin: 0 auto 1.5rem; border: 3px solid var(--pink-light); font-family: 'Playfair Display', serif; }
    .hero h1 { font-family: 'Playfair Display', serif; font-size: 36px; font-weight: 400; color: var(--pink-text); margin-bottom: 0.75rem; }
    .hero p { font-size: 15px; color: var(--pink-dark); margin-bottom: 2rem; }
    .hero-btns { display: flex; gap: 12px; justify-content: center; flex-wrap: wrap; }
    .btn-primary { background: var(--pink-strong); color: var(--white); border: none; padding: 12px 28px; border-radius: 25px; font-size: 14px; cursor: pointer; font-family: 'DM Sans', sans-serif; text-decoration: none; display: inline-block; transition: background 0.2s; }
    .btn-primary:hover { background: var(--pink-dark); }
    .btn-secondary { background: transparent; color: var(--pink-strong); border: 1.5px solid var(--pink-strong); padding: 12px 28px; border-radius: 25px; font-size: 14px; cursor: pointer; font-family: 'DM Sans', sans-serif; text-decoration: none; display: inline-block; transition: all 0.2s; }
    .btn-secondary:hover { background: var(--pink-lightest); }
    .section { padding: 4rem 2rem; max-width: 800px; margin: 0 auto; }
    .section-title { font-family: 'Playfair Display', serif; font-size: 28px; font-weight: 400; color: var(--pink-text); margin-bottom: 0.5rem; text-align: center; }
    .section-line { width: 50px; height: 2px; background: var(--pink-mid); margin: 0 auto 2rem; border-radius: 2px; }
    .divider { height: 1px; background: var(--pink-light); max-width: 800px; margin: 0 auto; }
    .about-card { background: var(--pink-lightest); border: 1px solid var(--pink-light); border-radius: 16px; padding: 2rem; }
    .about-card p { font-size: 15px; color: var(--pink-dark); line-height: 1.8; }
    .skills-grid { display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; }
    .skill-pill { background: var(--pink-light); color: var(--pink-text); font-size: 13px; padding: 8px 18px; border-radius: 20px; }
    .projects-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px; }
    .project-card { background: var(--white); border: 1px solid var(--pink-light); border-radius: 16px; padding: 1.5rem; transition: border-color 0.2s; }
    .project-card:hover { border-color: var(--pink-strong); }
    .project-icon { width: 44px; height: 44px; background: var(--pink-lightest); border-radius: 10px; display: flex; align-items: center; justify-content: center; margin-bottom: 1rem; font-size: 22px; }
    .project-card h3 { font-size: 15px; font-weight: 500; color: var(--pink-text); margin-bottom: 8px; }
    .project-card p { font-size: 13px; color: #666; line-height: 1.7; }
    .contact-card { background: var(--pink-lightest); border: 1px solid var(--pink-light); border-radius: 16px; padding: 2rem; max-width: 500px; margin: 0 auto; }
    .contact-row { display: flex; flex-direction: column; gap: 14px; }
    .contact-input { width: 100%; padding: 12px 16px; border: 1px solid var(--pink-light); border-radius: 10px; font-size: 14px; background: var(--white); color: #333; outline: none; font-family: 'DM Sans', sans-serif; transition: border-color 0.2s; }
    .contact-input:focus { border-color: var(--pink-strong); }
    textarea.contact-input { height: 120px; resize: none; }
    .submit-btn { background: var(--pink-strong); color: var(--white); border: none; padding: 14px; border-radius: 10px; font-size: 14px; cursor: pointer; width: 100%; font-family: 'DM Sans', sans-serif; transition: background 0.2s; }
    .submit-btn:hover { background: var(--pink-dark); }
    footer { background: var(--pink-lightest); border-top: 1px solid var(--pink-light); padding: 2rem; text-align: center; }
    footer p { font-size: 13px; color: var(--pink-dark); margin-bottom: 8px; }
    .social-links { display: flex; gap: 20px; justify-content: center; margin: 12px 0; }
    .social-links a { color: var(--pink-strong); font-size: 15px; text-decoration: none; transition: color 0.2s; }
    .social-links a:hover { color: var(--pink-text); }
    @media (max-width: 600px) { .hero h1 { font-size: 26px; } nav { padding: 1rem; } .nav-links { gap: 1rem; } }
  </style>
</head>
<body>

  <nav>
    <span class="nav-name">Madison Conley</span>
    <ul class="nav-links">
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="avatar">MC</div>
    <h1>Hi, I'm Madison Conley</h1>
    <p>Computer Science Student &middot; Cybersecurity Researcher &middot; Leader</p>
    <div class="hero-btns">
      <a href="#projects" class="btn-primary">View my work</a>
      <a href="#contact" class="btn-secondary">Contact me</a>
    </div>
  </section>

  <div id="about" class="section">
    <p class="section-title">About me</p>
    <div class="section-line"></div>
    <div class="about-card">
      <p>I am a Computer Science student at Mississippi Valley State University passionate about cybersecurity, AI, and using technology to make a meaningful impact. I serve as Vice President of the Campus Activity Board, Secretary of Women in Science and Technology, and a member of NSBE and Student Government.</p>
    </div>
  </div>

  <div class="divider"></div>

  <div id="skills" class="section">
    <p class="section-title">Skills</p>
    <div class="section-line"></div>
    <div class="skills-grid">
      <span class="skill-pill">Java</span>
      <span class="skill-pill">C++</span>
      <span class="skill-pill">Python</span>
      <span class="skill-pill">Web Development</span>
      <span class="skill-pill">Cybersecurity</span>
      <span class="skill-pill">Visual Basic</span>
      <span class="skill-pill">Excel</span>
      <span class="skill-pill">PowerPoint</span>
      <span class="skill-pill">JGrasp</span>
      <span class="skill-pill">Dev C++</span>
    </div>
  </div>

  <div class="divider"></div>

  <div id="projects" class="section">
    <p class="section-title">Projects</p>
    <div class="section-line"></div>
    <div class="projects-grid">
      <div class="project-card">
        <div class="project-icon">🔐</div>
        <h3>Cybersecurity & AI Research</h3>
        <p>Analyzed network routing behavior, traceroute data, and Internet topology challenges across multiple ISPs.</p>
      </div>
      <div class="project-card">
        <div class="project-icon">🌐</div>
        <h3>Network Topology Study</h3>
        <p>Investigated MPLS labels in ICMP responses and documented findings in a structured technical report.</p>
      </div>
      <div class="project-card">
        <div class="project-icon">💻</div>
        <h3>Portfolio Website</h3>
        <p>Designed and built a personal portfolio using Jekyll and GitHub Pages to showcase my skills and projects.</p>
      </div>
    </div>
  </div>

  <div class="divider"></div>

  <div id="contact" class="section">
    <p class="section-title">Contact me</p>
    <div class="section-line"></div>
    <div class="contact-card">
      <div class="contact-row">
        <input class="contact-input" type="text" placeholder="Your name" />
        <input class="contact-input" type="email" placeholder="Your email" />
        <textarea class="contact-input" placeholder="Your message"></textarea>
        <button class="submit-btn">Send message</button>
      </div>
    </div>
  </div>

  <footer>
    <p>madison.conley@mvsu.edu &middot; (901) 949-2994</p>
    <div class="social-links">
      <a href="https://github.com/mconley712" target="_blank">GitHub</a>
      <a href="www.linkedin.com/in/madison-conley-a137293aa" target="_blank">LinkedIn</a>
    </div>
    <p style="margin-top: 8px; font-size: 12px;">© 2026 Madison Conley</p>
  </footer>

</body>
</html>
