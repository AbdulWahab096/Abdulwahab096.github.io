<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Abdul Wahab | Portfolio</title>

<style>
/* ===== Global ===== */
body {
  margin: 0;
  font-family: 'Segoe UI', Arial, sans-serif;
  background: #f8fafc;
  color: #1f2937;
  line-height: 1.7;
}

a {
  text-decoration: none;
  color: inherit;
}

/* ===== Header ===== */
header {
  background: linear-gradient(135deg, #0f172a, #1e293b);
  color: white;
  padding: 90px 20px;
  text-align: center;
}

header img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid white;
  margin-bottom: 20px;
}

header h1 {
  font-size: 42px;
  margin-bottom: 10px;
}

header p {
  font-size: 18px;
  opacity: 0.9;
}

/* ===== Sections ===== */
section {
  max-width: 1100px;
  margin: auto;
  padding: 70px 20px;
}

h2 {
  text-align: center;
  font-size: 32px;
  margin-bottom: 50px;
}

/* ===== Cards ===== */
.card {
  background: white;
  border-radius: 14px;
  padding: 30px;
  margin-bottom: 30px;
  box-shadow: 0 15px 30px rgba(0,0,0,0.08);
  transition: transform 0.3s ease;
}

.card:hover {
  transform: translateY(-8px);
}

/* ===== Experience Grid ===== */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
}

/* ===== Skills ===== */
.skills span {
  display: inline-block;
  background: #e5e7eb;
  padding: 10px 18px;
  margin: 6px;
  border-radius: 999px;
  font-size: 14px;
}

/* ===== Projects ===== */
.project img {
  width: 100%;
  border-radius: 12px;
  margin-bottom: 15px;
}

/* ===== Buttons ===== */
.buttons {
  text-align: center;
}

.button {
  display: inline-block;
  background: #2563eb;
  color: white;
  padding: 14px 26px;
  margin: 10px;
  border-radius: 10px;
  font-weight: bold;
  transition: background 0.3s;
}

.button:hover {
  background: #1d4ed8;
}

/* ===== Footer ===== */
footer {
  background: #0f172a;
  color: #cbd5f5;
  text-align: center;
  padding: 30px;
}

/* ===== Animations ===== */
.fade-in {
  opacity: 0;
  transform: translateY(40px);
  transition: all 0.9s ease;
}

.fade-in.show {
  opacity: 1;
  transform: translateY(0);
}
</style>
</head>

<body>

<header>
  <img src="https://images.unsplash.com/photo-1527980965255-d3b416303d12" alt="Profile Photo">
  <h1>Abdul Wahab</h1>
  <p>MSc Digital Marketing & Analytics | Helsinki, Finland</p>
</header>

<section class="fade-in">
  <h2>About Me</h2>
  <p style="max-width:800px;margin:auto;text-align:center;">
    I am a motivated and detail-oriented professional with experience in customer service,
    operations, and digital marketing. I enjoy building practical projects, learning new
    technologies, and continuously improving my skills.
  </p>
</section>

<section class="fade-in">
  <h2>Experience</h2>
  <div class="grid">
    <div class="card">
      <h3>Restaurant Worker – Fafa’s</h3>
      <p>Customer service, inventory handling, and working efficiently in a fast-paced environment.</p>
    </div>
    <div class="card">
      <h3>Cleaner – IHP</h3>
      <p>Maintained hygiene and safety standards with strong attention to detail.</p>
    </div>
    <div class="card">
      <h3>Assistant Group Shop Manager</h3>
      <p>Managed inventory, audits, and daily operations across multiple shops.</p>
    </div>
  </div>
</section>

<section class="fade-in">
  <h2>Skills</h2>
  <div class="skills" style="text-align:center;">
    <span>Digital Marketing</span>
    <span>SEO</span>
    <span>Microsoft Office</span>
    <span>Tableau</span>
    <span>SPSS</span>
    <span>MS Dynamics 365</span>
    <span>Analytics</span>
    <span>Teamwork</span>
  </div>
</section>

<section class="fade-in">
  <h2>Projects</h2>
  <div class="grid">
    <div class="card project">
      <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085" alt="Project">
      <h3>Personal Portfolio Website</h3>
      <p>Designed and built a responsive portfolio website using HTML, CSS, and GitHub Pages.</p>
    </div>
    <div class="card project">
      <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c" alt="Project">
      <h3>Marketing Analytics Practice</h3>
      <p>Hands-on analytics projects using Tableau, SPSS, and data visualization techniques.</p>
    </div>
  </div>
</section>

<section class="fade-in buttons">
  <a class="button" href="Abdul-Wahab-CV.pdf" download>Download CV</a>
  <a class="button" href="https://www.linkedin.com/in/abdulwahab96/" target="_blank">LinkedIn</a>
  <a class="button" href="mailto:abdulwahab_1096@yahoo.com">Email Me</a>
</section>

<footer>
  © 2025 Abdul Wahab | Portfolio
</footer>

<script>
const items = document.querySelectorAll('.fade-in');
const observer = new IntersectionObserver(entries => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('show');
    }
  });
});
items.forEach(item => observer.observe(item));
</script>

</body>
</html>
