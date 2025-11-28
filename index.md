---
layout: default
title: "Smitha Reddy"
permalink: /
---

<style>
:root{
  --navy: #0a192f;
  --light-navy: #112240;
  --lightest-navy: #233554;
  --slate: #8892b0;
  --light-slate: #a8b2d1;
  --lightest-slate: #ccd6f6;
  --white: #e6f1ff;
  --green: #64ffda;
  --max-width: 1000px;
}

/* Page basics */
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  color: var(--lightest-navy);
  background: white;
  margin: 0;
  padding: 28px 20px;
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
}

/* Container */
.container {
  max-width: var(--max-width);
  margin: 0 auto;
}

/* Top nav (small, minimal) */
.site-nav {
  display:flex;
  justify-content:flex-end;
  gap:18px;
  align-items:center;
  margin-bottom: 14px;
  font-size:14px;
}
.site-nav a { color: var(--slate); text-decoration:none; }
.site-nav a:hover { color: var(--lightest-navy); }

/* Header hero */
.hero {
  display: grid;
  grid-template-columns: 1fr 220px;
  gap: 28px;
  align-items: center;
  padding: 26px;
  border-radius: 12px;
  background: linear-gradient(180deg, rgba(6,18,34,0.02), rgba(6,18,34,0.00));
  border: 1px solid rgba(10,25,47,0.04);
}

.hero h1 {
  font-size: 38px;
  margin:0;
  color: var(--navy);
  letter-spacing: -0.6px;
}
.hero p.lead {
  color: var(--lightest-slate);
  margin-top:10px;
  line-height:1.55;
}

/* Profile image */
.avatar {
  width:180px;
  height:180px;
  border-radius:12px;
  overflow:hidden;
  box-shadow: 0 8px 30px rgba(10,25,47,0.08);
  border: 1px solid rgba(10,25,47,0.06);
  display:block;
  object-fit:cover;
}

/* CV button */
.cv-row { margin-top:14px; }
.cv-btn {
  display: inline-flex;
  align-items:center;
  gap:10px;
  background: linear-gradient(135deg, var(--lightest-slate), var(--light-slate));
  color: var(--navy);
  padding: 10px 16px;
  border-radius: 999px;
  text-decoration: none;
  font-weight:600;
  box-shadow: 0 6px 18px rgba(10,25,47,0.06);
}
.cv-btn:hover { transform: translateY(-3px); }

/* Two-column sections */
.section {
  margin-top: 36px;
}
.section .two-col {
  display: grid;
  grid-template-columns: 1fr 320px;
  gap: 22px;
  align-items:start;
}

/* Projects grid */
.projects {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 18px;
}
.project {
  border-radius: 10px;
  background: white;
  padding: 16px;
  border: 1px solid rgba(10,25,47,0.04);
  box-shadow: 0 6px 18px rgba(10,25,47,0.02);
  transition: transform .18s ease, box-shadow .18s ease;
}
.project:hover { transform: translateY(-6px); box-shadow: 0 12px 30px rgba(10,25,47,0.06); }

.project h4 { margin: 0 0 6px 0; color: var(--navy); }
.project p { margin:0; color: var(--slate); font-size:14px; }

/* Headings */
h2 { color: var(--navy); margin:0 0 14px 0; font-size:20px; }

/* Lists and small panels */
.side-panel {
  padding: 14px;
  border-radius: 10px;
  border: 1px solid rgba(10,25,47,0.04);
  background: linear-gradient(180deg, rgba(230,241,255,0.4), rgba(230,241,255,0.08));
  color: var(--navy);
}
.side-panel h3 { margin-top:0; }

/* Simple responsive */
@media (max-width:920px){
  .hero { grid-template-columns: 1fr; text-align:center; }
  .two-col { grid-template-columns: 1fr; }
  .site-nav { justify-content:center; margin-bottom:10px; }
  .hero p.lead { padding: 0 6px; }
}
</style>

<div class="container">
  <!-- nav -->
  <nav class="site-nav">
    <a href="#projects">Projects</a>
    <a href="#research">Research</a>
    <a href="#experience">Experience</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- hero -->
  <section class="hero" aria-label="intro">
    <div>
      <h1>Smitha Reddy</h1>
      <p class="lead">
        Machine Learning Researcher • Deep Learning & Computer Vision  
        <br>
        Currently on a career break; focusing on data-efficient ML, GANs, and applied research for social good.
      </p>

      <div class="cv-row">
        <!-- CV: replace file when ready -->
        <a class="cv-btn" href="assets/Smitha_Reddy_CV.pdf" download>
          📄 Download CV
        </a>
      </div>

    </div>

    <div style="text-align:center">
      <img class="avatar" src="assets/profile.jpg" alt="Smitha Reddy — profile photo">
      <div style="margin-top:10px; color:var(--slate); font-size:13px;">(Replace with your photo in assets/profile.jpg)</div>
    </div>
  </section>

  <!-- About + Quick info -->
  <section class="section">
    <div class="two-col">
      <div>
        <h2>About</h2>
        <p>
          I am the first woman in my family to pursue a four-year science degree. My work focuses on
          applying generative models and transfer learning to low-resource vision tasks, notably
          multiclass leaf classification and data augmentation with conditional GANs. I enjoy teaching,
          mentoring, and building tools that help improve dataset fairness and accessibility.
        </p>

        <h2 id="projects" style="margin-top:28px;">Projects</h2>

        <div class="projects">
          <article class="project">
            <h4>Conditional GAN for 30-class Leaf Dataset</h4>
            <p>Generated 128×128 & 256×256 images to reduce class imbalance and improve classifier recall. <br><strong>Repo:</strong> placeholder</p>
          </article>

          <article class="project">
            <h4>Multiclass Leaf Classification</h4>
            <p>ResNet50 / EfficientNet experiments using GAN-augmented training sets to boost rare-class performance. <br><strong>Repo:</strong> placeholder</p>
          </article>

          <article class="project">
            <h4>Preprocessing & Augmentation Pipeline</h4>
            <p>Modular pipeline with ImageDataGenerator and custom transforms to standardize inputs and augment low-sample classes. <br><strong>Repo:</strong> placeholder</p>
          </article>

        </div>
      </div>

      <aside class="side-panel">
        <h3>Quick Info</h3>
        <p><strong>Interests:</strong><br>GANs • Computer Vision • Transfer Learning • Foundation Models</p>
        <p><strong>Skills:</strong><br>Python, PyTorch, Keras, TensorFlow, OpenCV, Git</p>
        <p><strong>Location:</strong><br>India</p>
      </aside>
    </div>
  </section>

  <!-- Research -->
  <section id="research" class="section">
    <h2>Research & Publications</h2>
    <p>(Placeholders — replace with full citations and links)</p>
    <ol>
      <li><strong>Publication Title Placeholder 1</strong> — Authors. Journal / Conference (Year). <a href="#">link</a></li>
      <li><strong>Publication Title Placeholder 2</strong> — Authors. Journal / Conference (Year). <a href="#">link</a></li>
    </ol>
  </section>

  <!-- Experience -->
  <section id="experience" class="section">
    <h2>Experience</h2>

    <div class="two-col" style="align-items:flex-start;">
      <div>
        <h3>Research Assistant — Computer Vision & Deep Learning</h3>
        <ul>
          <li>Built conditional GAN models and synthesis pipelines.</li>
          <li>Developed training and evaluation workflows using Keras & PyTorch.</li>
          <li>Analyzed model robustness and improved minority-class performance.</li>
        </ul>

        <h3>STEM Mentor — Nonprofit</h3>
        <ul>
          <li>Led workshops for high-school students and organized STEM drives.</li>
          <li>Designed curriculum for coding and basic ML topics.</li>
        </ul>
      </div>

      <aside class="side-panel">
        <h3>Education</h3>
        <p><strong>B.Tech — Computer Science</strong><br>University / College (replace)</p>
        <h3 style="margin-top:12px">Awards</h3>
        <ul>
          <li>Award Placeholder 1</li>
          <li>Award Placeholder 2</li>
        </ul>
      </aside>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="section">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:smithareddy13@gmail.com">smithareddy13@gmail.com</a></p>
    <p>GitHub: <a href="https://github.com/mystique03">mystique03</a> • LinkedIn: <em>add link</em></p>
  </section>

  <footer style="margin-top:36px; color:var(--slate); font-size:13px; text-align:center;">
    <div>Made with a minimal Jekyll template — inspired by <a href="https://v4.brittanychiang.com" target="_blank">bchiang v4</a>.</div>
    <div style="margin-top:6px;">© Smitha Reddy</div>
  </footer>
</div>
