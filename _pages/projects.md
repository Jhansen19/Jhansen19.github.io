---
permalink: /projects/
title: "Projects"
---

<!-- page-specific tweaks – no background here -->
<style>
  /* === Projects Grid (vertical stack with spacing) === */
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 40px;   /* ↑ space between each project card */
    margin: 40px auto; /* optional top/bottom margin, center grid */
    max-width: 800px;
  }

  /* === Individual Project Cards (frosted-glass look) === */
  .project-card {
    background: rgba(0, 0, 0, 0.5);       /* semi-transparent dark */
    backdrop-filter: blur(8px);           /* blur behind the card */
    border: 1px solid rgba(255, 255, 255, 0.5);
    border-radius: 12px;
    padding: 40px;
    color: #fff;
  }

  .project-card img {
    width: 100%;
    max-width: 400px;
    height: auto;
    border-radius: 8px;
    margin-bottom: 15px;
    display: inline-block;
  }

  .project-card h3 {
    margin-top: 0;
    margin-bottom: 32px;  /* ↑ add space between title and paragraph */
  }

  .project-card p {
    line-height: 1.5;
  }

  .project-card a {
    display: inline-block;
    margin-top: 15px;
    padding: 8px 16px;
    text-decoration: none;
    color: #fff;
    border: 1px solid #fff;
    border-radius: 8px;
  }
</style>

<div class="projects-page">
  <div class="projects-grid">

    <!-- Project 1 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/seg1.png" alt="UAV Disaster Damage Detection screenshot" />
      <h3>UAV Disaster Damage Detection</h3>
      <p>After natural disasters, a quick and accurate damage assessment is crucial for an effective response. The core problem our project seeks to address is how to provide a faster and reliable damage assessment of disaster areas. To achieve this goal, the project performed fine-tuning on a DeepLabV3 model with a natural disaster image dataset called RescueNet. The model achieved an IoU score of 50.6% after only 7 epochs of training. While not the level of performance the team was looking for, the model performed well given the limited computational resources.</p>
      <a href="https://github.com/your-username/project1" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>

    <!-- Project 2 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="Project 2 screenshot" />
      <h3>Project 2</h3>
      <p>A brief description…</p>
      <a href="https://github.com/your-username/project2" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>

    <!-- Project 3 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="Project 3 screenshot" />
      <h3>Project 3</h3>
      <p>This is the description…</p>
      <a href="https://github.com/your-username/project3" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>

  </div>
</div>


