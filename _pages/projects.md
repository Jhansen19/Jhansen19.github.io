---
permalink: /projects/
title: "Projects"
---

<!-- page-specific tweaks – no background here -->
<style>
.project-card {
  /* 1) semi-transparent dark background so you see the page BG behind */
  background: rgba(0, 0, 0, 0.5);
  /* 2) blur whatever is behind the card for that frosted-glass feel */
  backdrop-filter: blur(8px);
  /* 3) white border at 50% opacity */
  border: 1px solid rgba(255, 255, 255, 0.5);
  /* 4) rounded corners & spacing */
  border-radius: 12px;
  padding: 40px;
  /* 5) white text to stand out */
  color: #fff;
  /* optional: constrain card width and center it */
  max-width: 800px;
  margin: auto;
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
  margin-bottom: 16px;
}
  
.project-card a {
  /* make the link button white too */
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
<!--
<p>Welcome to the Projects section of my website! Below, you'll find a showcase of some of the projects I've been working on. Each project is linked to its GitHub repository, where you can explore the code, documentation, and additional details.</p>
-->

  <div class="projects-grid">
    <!-- Project 1 -->
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/seg1.png" alt="UAV Disaster Damage Detection screenshot" />
      <h3>UAV Disaster Damage Detection</h3>
      <p>After natural disasters, a quick and accurate damage assessment is crucial for an effective response. The core problem our project seeks to address is how to provide a faster and reliable damage assessment of disaster areas. To achieve this goal, the project performed fine-tuning on a DeepLabV3 model with a natural disaster image dataset called RescueNet. The model achieved an IoU score of 50.6% after only 7 epochs of training. While not the level of performance the team was looking for, the model performed well given the limited computational resources.</p>
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
