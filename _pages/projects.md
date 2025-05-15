---
permalink: /projects/
title: "Projects"
---

<style>
  /* === Projects Page Specific Styles === */
  .projects-page {
    position: relative; /* Keeps the ::before pseudo-element positioned correctly */
    padding: 60px 20px;
    /*
      THE LINE BELOW IS COMMENTED OUT OR REMOVED:
      This ensures that the .projects-page div does NOT set its own background image,
      allowing the global background image (from your background.css applied to the <html> tag)
      to be visible.
    */
    /* background: url("/assets/images/background.jpg") center/cover no-repeat; */

    color: #fff; /* Text color for the H1 and intro paragraph. Adjust if needed for readability against your global background + overlay. */
  }

  /* This pseudo-element creates the dark overlay.
     It will now sit on top of the global background image within the bounds of .projects-page */
  .projects-page::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: rgba(0, 0, 0, 0.4); /* Semi-transparent black overlay */
    z-index: 0; /* Ensures it's behind the content but above the (now transparent) .projects-page div's own potential background layer */
  }

  /* Ensures direct children of .projects-page (like H1, P, .projects-grid)
     are stacked above the ::before pseudo-element. */
  .projects-page > * {
    position: relative;
    z-index: 1;
  }

  /* === Projects Grid (vertical stack) === */
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr; /* Each project card takes the full width, stacking them vertically */
    row-gap: 20px; /* Space between project cards */
    margin-top: 40px;
  }

  /* === Individual Project Cards === */
  .project-card {
    background: rgba(255, 255, 255, 0.9); /* Light, semi-transparent background for readability */
    border-radius: 8px;
    padding: 20px;
    text-align: center;
    color: #333; /* Dark text color for content inside the card */
  }

  .project-card img {
    width: 100%;
    max-width: 400px; /* Optional: constrain image width on larger cards if they stretch too much */
    height: auto;
    border-radius: 8px;
    margin-bottom: 15px;
    display: inline-block; /* Allows text-align: center on parent to center it if max-width is less than card width */
  }

  .project-card h3 {
    margin-top: 0;
  }

  .project-card a {
    display: inline-block;
    margin-top: 15px;
    text-decoration: none;
    color: #007bff; /* Link color */
  }
</style>

<div class="projects-page">

  <h1>Projects</h1>
  <p>Welcome to the Projects section of my website! Below, you'll find a showcase of some of the projects I've been working on. Each project is linked to its GitHub repository, where you can explore the code, documentation, and additional details.</p>

  <div class="projects-grid">

    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/seg1.png" alt="UAV Disaster Damage Detection screenshot" />
      <h3>UAV Disaster Damage Detection: Using Semantic Segmentation</h3>
      <p>After natural disasters…</p>
      <a href="https://github.com/Jhansen19/DisasterRecoverySegmentation" target="_blank">View on GitHub</a>
    </div>

    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="Project 2 screenshot" />
      <h3>Project 2</h3>
      <p>A brief description…</p>
      <a href="https://github.com/your-username/project2" target="_blank">View on GitHub</a>
    </div>

    <div class="project-card">
      <img src="{{ site.baseurl }}/assets/images/photo.jpg" alt="Project 3 screenshot" />
      <h3>Project 3</h3>
      <p>This is the description…</p>
      <a href="https://github.com/your-username/project3" target="_blank">View on GitHub</a>
    </div>

    </div>
</div>
