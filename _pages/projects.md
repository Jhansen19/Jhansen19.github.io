---
permalink: /projects/
title: "Projects"
classes: wide
---

<div class="profile-shell">
  <section class="section-card glass-panel project-hero">
    <div class="section-label">Project portfolio</div>
    <h2>Data science work explained through the decision it supports</h2>
    <p>
      My projects are not just tool demonstrations. They show how I define a practical question, structure messy data, choose a method that fits, and communicate the result so someone can act.
    </p>
  </section>

  <div class="project-grid">
    <article class="project-card impact-card">
      <img src="{{ site.baseurl }}/assets/images/segphoto.jpg" alt="Computer vision project preview">
      <div class="small-meta">May 2025</div>
      <h3>UAV damage detection with computer vision</h3>
      <div class="project-value">
        <span>Decision value</span>
        <p>Help response teams review disaster imagery faster so field attention can move toward damaged areas sooner.</p>
      </div>
      <div class="project-copy">
        <div class="project-copy-block">
          <div class="project-label">Operational question</div>
          <p>Disaster response teams need a faster way to understand damage across large areas. Manual review can take too long when speed matters.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Technical path</div>
          <p>I fine tuned a DeepLabV3 segmentation model on RescueNet imagery so damaged regions could be identified more quickly from aerial views. The model reached an IoU score of 50.6 percent in seven training epochs.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Methods</div>
          <p>Python, PyTorch, image segmentation, model evaluation</p>
        </div>
      </div>
      <div class="link-row">
        <a class="site-button site-button--ghost" href="https://github.com/Jhansen19/DisasterRecoverySegmentation/tree/main" target="_blank" rel="noopener noreferrer">Open GitHub repo</a>
      </div>
    </article>

    <article class="project-card impact-card">
      <img src="{{ site.baseurl }}/assets/images/HousingPred.jpg" alt="Housing prediction project preview">
      <div class="small-meta">March 2025</div>
      <h3>Housing value prediction with clustering and neural networks</h3>
      <div class="project-value">
        <span>Decision value</span>
        <p>Improve forecasting by capturing neighborhood patterns that a simpler model may miss.</p>
      </div>
      <div class="project-copy">
        <div class="project-copy-block">
          <div class="project-label">Analytical question</div>
          <p>Home values depend on many connected neighborhood features. The challenge was to improve prediction quality while capturing hidden structure in the data.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Technical path</div>
          <p>I used self organizing maps to group similar neighborhoods, then passed those groupings into an artificial neural network for forecasting. The final model explained more than 80 percent of the variation in sale prices.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Methods</div>
          <p>Python, pandas, scikit learn, MiniSom, TensorFlow</p>
        </div>
      </div>
      <div class="link-row">
        <a class="site-button site-button--ghost" href="https://github.com/Jhansen19/Housing_Pred_AnnSOM/tree/main" target="_blank" rel="noopener noreferrer">Open GitHub repo</a>
      </div>
    </article>

    <article class="project-card impact-card">
      <img src="{{ site.baseurl }}/assets/images/accidentpred.jpg" alt="Rail risk analysis project preview">
      <div class="small-meta">December 2024</div>
      <h3>Freight rail risk analysis for Indiana</h3>
      <div class="project-value">
        <span>Decision value</span>
        <p>Give planners a clearer view of where hazardous rail movement and community vulnerability overlap.</p>
      </div>
      <div class="project-copy">
        <div class="project-copy-block">
          <div class="project-label">Planning question</div>
          <p>Rail safety planning is stronger when agencies can see where freight activity, past incidents, hazardous materials, and community vulnerability overlap.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Technical path</div>
          <p>I combined accident records, traffic volume, commodity hazard, and community data to estimate risk by rail segment. The result was an interactive map that highlighted corridors where safety attention could have the greatest value.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Methods</div>
          <p>Python, geospatial analysis, Folium, risk modeling</p>
        </div>
      </div>
      <div class="link-row">
        <a class="site-button site-button--ghost" href="https://github.com/Jhansen19/Rail_Accident_Predictions" target="_blank" rel="noopener noreferrer">Open GitHub repo</a>
      </div>
    </article>

    <article class="project-card impact-card">
      <img src="{{ site.baseurl }}/assets/images/AzurePipe.jpg" alt="Azure data pipeline project preview">
      <div class="small-meta">November 2024</div>
      <h3>Azure pipeline for airline data</h3>
      <div class="project-value">
        <span>Decision value</span>
        <p>Create trusted data layers so analytics and machine learning can start from cleaner, more reliable inputs.</p>
      </div>
      <div class="project-copy">
        <div class="project-copy-block">
          <div class="project-label">Operating question</div>
          <p>Large transportation datasets are difficult to use when the data arrives in raw files and analysts need reliable tables for reporting and modeling.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Technical path</div>
          <p>I built an end to end ELT workflow in Azure that ingested raw CSV files into Data Lake Storage Gen2, transformed them with Data Factory and Spark, and published silver and gold layers for machine learning use.</p>
        </div>
        <div class="project-copy-block">
          <div class="project-label">Methods</div>
          <p>Azure Data Factory, Spark, Data Lake Storage Gen2, Key Vault, medallion architecture</p>
        </div>
      </div>
      <div class="link-row">
        <a class="site-button site-button--ghost" href="https://github.com/Jhansen19/Airline_Predictions" target="_blank" rel="noopener noreferrer">Open GitHub repo</a>
      </div>
    </article>
  </div>
</div>
