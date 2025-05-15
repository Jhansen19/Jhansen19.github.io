---
permalink: /projects/
title: "Projects"
---

<!--
  Insert your page-specific CSS here. 
  Jekyll will emit it into the <head> so your classes are defined.
-->
<style>
.projects-page {
  position: relative;
  padding: 60px 20px;
  background: url("/assets/images/your-bg.jpg") center/cover no-repeat;
  color: #fff;
}

.projects-page::before {
  content: "";
  position: absolute;
  top:0; left:0; right:0; bottom:0;
  background: rgba(0,0,0,0.4);
  z-index: 0;
}

.projects-page > * {
  position: relative;
  z-index: 1;
}

.projects-grid {
  display: grid;
  grid-template-columns: 1fr;
  row-gap: 20px;
  margin-top: 40px;
}

.project-card {
  background: rgba(255,255,255,0.9);
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
  <p>Welcome to the Projects section of my website! …</p>

  <div class="projects-grid">
    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/seg1.png" alt="">
      <h3>UAV Disaster Damage Detection</h3>
      <p>After natural disasters…</p>
      <a href="https://github.com/Jhansen19/DisasterRecoverySegmentation" target="_blank">View on GitHub</a>
    </div>

    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="">
      <h3>Project 2</h3>
      <p>A brief description…</p>
      <a href="https://github.com/your-username/project2" target="_blank">View on GitHub</a>
    </div>

    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="">
      <h3>Project 3</h3>
      <p>This is the description…</p>
      <a href="https://github.com/your-username/project3" target="_blank">View on GitHub</a>
    </div>
  </div>

</div>
