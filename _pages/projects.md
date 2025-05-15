---
permalink: /projects/
title: "Projects"
---

<style>
  /* === Projects Page Background === */
  .projects-page {
    position: relative;
    padding: 60px 20px;
    background: url("/assets/images/background.jpg") center/cover no-repeat;
    color: #fff;
  }

  .projects-page::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: rgba(0, 0, 0, 0.4);
    z-index: 0;
  }

  .projects-page > * {
    position: relative;
    z-index: 1;
  }

  /* === Projects Grid (vertical stack) === */
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 20px;
    margin-top: 40px;
  }

  /* === Individual Project Cards === */
  .project-card {
    background: rgba(255, 255, 255, 0.9);
    border-radius: 8px;
    padding: 20px;
    text-align: center;
    color: #333;
  }

  .project-card img {
    width: 100%;
    height: auto;
    border-radius: 8px;
    margin-bottom: 15px;
  }

  .project-card h3 {
    margin-top: 0;
  }

  .project-card a {
    display: inline-block;
    margin-top: 15px;
    text-decoration: none;
    color: #007bff;
  }
</style>

<div class="projects-page">

  <h1>Projects</h1>
  <p>Welcome to the Projects section of my website! Below, you'll find a showcase of some of the projects I've been working on. Each project is linked to its GitHub repository, where you can explore the code, documentation, and additional details.</p>

  <!-- ONE grid wrapper for ALL cards -->
  <div class="projects-grid">

    <!-- Project 1 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/seg1.png" alt="UAV Disaster Damage Detection screenshot" />
      <h3>UAV Disaster Damage Detection: Using Semantic Segmentation</h3>
      <p>After natural disasters…</p>
      <a href="https://github.com/Jhansen19/DisasterRecoverySegmentation" target="_blank">View on GitHub</a>
    </div>

    <!-- Project 2 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="Project 2 screenshot" />
      <h3>Project 2</h3>
      <p>A brief description…</p>
      <a href="https://github.com/your-username/project2" target="_blank">View on GitHub</a>
    </div>

    <!-- Project 3 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="Project 3 screenshot" />
      <h3>Project 3</h3>
      <p>This is the description…</p>
      <a href="https://github.com/your-username/project3" target="_blank">View on GitHub</a>
    </div>

  </div>
</div>
