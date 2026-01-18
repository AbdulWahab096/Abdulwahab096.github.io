<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Abdul Wahab | Portfolio</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f4f6f8;
  color: #333;
}

header {
  background: linear-gradient(135deg, #1f2937, #111827);
  color: white;
  text-align: center;
  padding: 80px 20px;
}

header h1 {
  font-size: 40px;
  margin-bottom: 10px;
}

section {
  max-width: 1000px;
  margin: auto;
  padding: 50px 20px;
}

h2 {
  text-align: center;
  margin-bottom: 30px;
}

.card {
  background: white;
  padding: 25px;
  border-radius: 10px;
  margin-bottom: 20px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.08);
}

.skills span {
  display: inline-block;
  background: #e5e7eb;
  padding: 8px 14px;
  margin: 6px;
  border-radius: 20px;
}

.buttons {
  text-align: center;
}

.button {
  display: inline-block;
  background: #2563eb;
  color: white;
  padding: 12px 22px;
  margin: 10px;
  border-radius: 6px;
  text-decoration: none;
}

footer {
  background: #111827;
  color: #bbb;
  text-align: center;
  padding: 20px;
}

.fade-in {
  opacity: 0;
  transform: translateY(30px);
  transition: 0.8s;
}

.fade-in.show {
  opacity: 1;
  transform: translateY(0);
}
</style>
</head>

<body>

<header>
  <h1>Abdul Wahab</h1>
  <p>MSc Digital Marketing & Analytics | Helsinki, Finland</p>
</header>

<section class="fade-in">
  <h2>About Me</h2>
  <p>
    I am a motivated and detail-oriented professional currently pursuing a Master’s
    degree in Digital Marketing and Analytics. I enjoy learning new technologies and
    building practical projects.
  </p>
</section>

<section class="fade-in">
  <h2>Experience</h2>

  <div class="card">
    <strong>Restaurant Worker – Fafa’s</strong>
    <p>Customer service and inventory handling in a fast-paced environment.</p>
  </div>

  <div class="card">
    <strong>Cleaner – IHP</strong>
    <p>Maintained hygiene standards with attention to detail.</p>
  </div>
</section>

<section class="fade-in">
  <h2>Skills</h2>
  <div class="skills">
    <span>SEO</span>
    <span>Digital Marketing</span>
    <span>Microsoft Office</span>
    <span>Tableau</span>
    <span>SPSS</span>
  </div>
</section>

<section class="fade-in">
  <h2>Projects</h2>
  <div class="card">
    <strong>Personal Portfolio Website</strong>
    <p>Built using HTML, CSS, and GitHub Pages.</p>
  </div>
</section>

<section class="fade-in buttons">
  <a class="button" href="Abdul-Wahab-CV.pdf" download>Download CV</a>
  <a class="button" href="https://www.linkedin.com/in/abdulwahab96/" target="_blank">LinkedIn</a>
</section>

<footer>
  © 2025 Abdul Wahab
</footer>

<script>
const sections = document.querySelectorAll('.fade-in');

const observer = new IntersectionObserver(entries => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('show');
    }
  });
});

sections.forEach(section => observer.observe(section));
</script>

</body>
</html>
