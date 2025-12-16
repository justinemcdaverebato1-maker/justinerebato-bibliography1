<html lang="en"><head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Allen Santino L. Macarandan | Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&amp;family=Poppins:wght@300;400;500;600&amp;display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --primary-red: #b11226;
  --dark-red: #7a0c1b;
  --gold: #f5c77a;
  --glass: rgba(255,255,255,0.08);
  --text-main: #f5f5f5;
  --text-muted: #cfcfcf;
  --text-dark: #1e1e1e;
}

/* BODY */
body {
  font-family: 'Poppins', sans-serif;
  background: #121212;
  color: var(--text-main);
  min-height: 100vh;
}

/* BACKGROUND IMAGE */
body::before {
  content: "";
  background: url('background.jpg') center/cover no-repeat fixed;
  position: fixed;
  inset: 0;
  opacity: 0.45;
  filter: blur(6px) brightness(0.55);
  z-index: -1;
}

/* HEADER */
header {
  padding: 35px 70px;
  display: flex;
  align-items: center;
  border-bottom: 2px solid var(--primary-red);
  background: linear-gradient(
    to right,
    rgba(177,18,38,0.35),
    rgba(0,0,0,0.65)
  );
  backdrop-filter: blur(12px);
}

.profile {
  display: flex;
  align-items: center;
  gap: 30px;
}

.photo-box {
  width: 170px;
  height: 200px;
  border: 3px solid var(--gold);
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 15px 40px rgba(0,0,0,0.6);
}

.photo-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

header h1 {
  font-family: 'Playfair Display', serif;
  font-size: 3rem;
  color: var(--gold);
  letter-spacing: 1px;
}

header p {
  font-size: 1.2rem;
  color: var(--text-muted);
  font-weight: 600;
}

.sub-info {
  font-size: 1rem;
  margin-top: 6px;
  color: var(--text-main);
  font-weight: 500;
}

/* NAVIGATION */
nav.dashboard {
  padding: 30px 70px;
  display: flex;
  gap: 20px;
}

.nav-card {
  flex: 1;
  background: linear-gradient(135deg, var(--primary-red), var(--dark-red));
  padding: 22px;
  border-radius: 18px;
  text-align: center;
  cursor: pointer;
  transition: 0.35s;
  box-shadow: 0 10px 30px rgba(0,0,0,0.5);
}

.nav-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 15px 45px rgba(0,0,0,0.7);
}

.nav-card h4 {
  font-family: 'Playfair Display', serif;
  font-size: 1.4rem;
  color: var(--gold);
}

.nav-card p {
  font-size: 1rem;
  color: var(--text-main);
}

/* SECTIONS */
section {
  width: 100%;
  padding: 85px 80px;
}

.section-title {
  font-family: 'Playfair Display', serif;
  font-size: 2.6rem;
  color: var(--primary-red);
  text-align: center;
  margin-bottom: 20px;
}

.card {
  background: var(--glass);
  padding: 40px;
  border-radius: 22px;
  box-shadow: 0 20px 60px rgba(0,0,0,0.4);
}

.about-text {
  font-size: 1.18rem;
  line-height: 2;
  text-align: justify;
  color: var(--text-main);
}

ul.facts {
  margin-top: 15px;
  list-style: circle;
  padding-left: 20px;
  color: var(--text-muted);
}

ul.facts li {
  margin-bottom: 6px;
}

/* TAGS */
.tags {
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: 15px;
}

.tag {
  background: var(--primary-red);
  color: var(--text-main);
  padding: 12px 28px;
  border-radius: 30px;
  font-size: 1.05rem;
  cursor: pointer;
  font-weight: 600;
  transition: 0.3s;
  box-shadow: 0 6px 14px rgba(0,0,0,0.4);
}

.tag:hover {
  background: var(--dark-red);
}

/* IMAGE DISPLAY */
.image-display {
  margin-top: 25px;
  display: flex;
  justify-content: center;
  gap: 24px;
  flex-wrap: wrap;
}

.image-display > div {
  text-align: center;
}

.image-display img {
  width: 300px;
  border-radius: 18px;
  box-shadow: 0 15px 40px rgba(0,0,0,0.5);
  display: block;
  margin: 0 auto;
}

.caption {
  font-size: 1.05rem;
  margin-top: 10px;
  color: var(--text-main);
  font-weight: 500;
}

/* SOCIALS */
#socials .social-box {
  display: flex;
  justify-content: center;
  gap: 24px;
  margin-top: 18px;
}

.social-card {
  padding: 12px 28px;
  background: var(--primary-red);
  border-radius: 14px;
  box-shadow: 0 6px 14px rgba(0,0,0,0.4);
}

.social-card a {
  color: var(--text-main);
  font-size: 1.15rem;
  text-decoration: none;
  font-weight: 600;
}

.social-card a:hover {
  text-decoration: underline;
}

/* FOOTER */
footer {
  padding: 25px;
  text-align: center;
  background: var(--dark-red);
  color: var(--text-main);
  font-size: 1.1rem;
}

/* RESPONSIVE */
@media(max-width:900px) {
  header {
    flex-direction: column;
    text-align: center;
    gap: 18px;
  }
  nav.dashboard {
    flex-direction: column;
  }
  section {
    padding: 60px 25px;
  }
  .image-display img {
    width: 90%;
    max-width: 320px;
  }
}
</style>
</head>
<body>

<!-- HEADER -->
<header>
  <div class="profile">
    <div class="photo-box">
      <img src="myphoto.jpg" alt="Allen Santino L. Macarandan">
    </div>
    <div>
      <h1>Allen Santino L. Macarandan</h1>
      <p><strong>Student • Aspiring Developer &amp; Designer</strong></p>
      <div class="sub-info">Grade 12 – ICT 1 • University Honor</div>
    </div>
  </div>
</header>

<!-- NAV -->
<nav class="dashboard">
  <div class="nav-card" onclick="scrollToSection('about')">
    <h4>About Me</h4><p>Learn who I am</p>
  </div>
  <div class="nav-card" onclick="scrollToSection('skills')">
    <h4>Skills</h4><p>Click to view</p>
  </div>
  <div class="nav-card" onclick="scrollToSection('hobbies')">
    <h4>Hobbies</h4><p>Fun activities</p>
  </div>
  <div class="nav-card" onclick="scrollToSection('socials')">
    <h4>Contact</h4><p>Connect with me</p>
  </div>
</nav>

<!-- ABOUT -->
<section id="about">
  <div class="section-title">About Me</div>
  <div class="card">
    <div class="about-text">
      Hello! My name is Allen Santino L. Macarandan and I am 18 years old, born on September 5, 2007. I am currently a Grade 12 ICT student with a deep passion for technology, creativity, and human‑centered design. From a young age, I have always been fascinated by how technology shapes the way we live and interact with the world. What truly inspires me isn’t just the complexity or power of technology, but the way it connects people, simplifies everyday tasks, and opens doors to new possibilities. I believe that behind every great digital experience is thoughtful design and meaningful interaction something I continuously strive to understand and improve. My journey with technology began with curiosity, but over the years it has grown into a purposeful path focused on learning, experimenting, and building solutions that have a positive impact on others. Every project, whether big or small, teaches me something new and pushes me to blend logic, creativity, and empathy in everything I do.
      <ul class="facts">
        <li>I love sleeping</li>
        <li>I love reading</li>
        <li>I love my girlfriend</li>
        <li>Recognized as University Honor</li>
        <li>Passionate about UI/UX design</li>
      </ul>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="section-title">Skills</div>
  <div class="card">
    <div class="tags">
      <div class="tag" onclick="showSkill('ui.jpg','UI Design','Creating visuals and layouts that are beautiful and easy to use ✨')">UI Design</div>
      <div class="tag" onclick="showSkill('ux.jpg','UX Design','Designing experiences that feel smooth and natural 💡')">UX Design</div>
    </div>
    <div class="image-display" id="skillImages"></div>
  </div>
</section>

<!-- HOBBIES -->
<section id="hobbies">
  <div class="section-title">Hobbies</div>
  <div class="card">
    <div class="tags">
      <div class="tag" onclick="showHobby('cycling.jpg','Cycling gives me freedom and energy. Every ride feels like a refreshing break from routines.')">🚴 Cycling</div>
      <div class="tag" onclick="showHobby('gaming.jpg','Gaming challenges my strategy and creativity, and it’s a great way to relax with friends.')">🎮 Gaming</div>
      <div class="tag" onclick="showHobby('guitar.jpg','Playing guitar helps me express myself and unwind after a long day.')">🎸 Guitar</div>
      <div class="tag" onclick="showHobby('riding.jpg','Riding photos capture joyful moments spent outdoors and remind me of fun memories.')">🐎 Riding</div>
    </div>
    <div class="image-display" id="hobbyImages"></div>
  </div>
</section>

<!-- CONTACT -->
<section id="socials">
  <div class="section-title">Contact Me</div>
  <div class="card">
    <p style="text-align:center; font-size:1.15rem; margin-bottom:18px; color:var(--text-main);">
      You can reach me at: <br>📞 0927-404-8072
    </p>
    <div class="social-box">
      <div class="social-card"><a href="https://www.facebook.com/Allennn05" target="_blank">📘 Facebook</a></div>
      <div class="social-card"><a href="https://www.instagram.com/macarandanallen/" target="_blank">📸 Instagram</a></div>
      <div class="social-card"><a href="https://www.tiktok.com/@cinnamonlover7" target="_blank">🎵 TikTok</a></div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  © 2025 Allen Santino L. Macarandan
</footer>

<script>
function showSkill(img, title, desc){
  document.getElementById('skillImages').innerHTML =
    `<div>
       <img src="${img}" alt="${title}">
       <div class="caption"><strong>${title}</strong><br>${desc}</div>
     </div>`;
}

function showHobby(img, desc){
  document.getElementById('hobbyImages').innerHTML =
    `<div>
       <img src="${img}" alt="Hobby Image">
       <div class="caption">${desc}</div>
     </div>`;
}

function scrollToSection(id){
  document.getElementById(id).scrollIntoView({behavior:'smooth'});
}
</script>



</body></html>
