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
    position: relative;                  /* for absolutely-positioned date */
    background: rgba(0, 0, 0, 0.5);      /* semi-transparent dark */
    backdrop-filter: blur(8px);          /* blur behind the card */
    border: 1px solid rgba(255, 255, 255, 0.5);
    border-radius: 12px;
    padding: 40px;
    color: #fff;
  }

  /* Date in the top-right corner */
  .project-card .date {
    position: absolute;
    top: 16px;
    right: 16px;
    font-size: 0.85em;
    font-weight: 500;
    color: rgba(255, 255, 255, 0.8);
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
      <div class="date">May 2025</div>
      <h3>UAV Disaster Damage Detection: Computer Vision Segmentation</h3>
      <img src="{{ site.baseurl }}/assets/images/segphoto.jpg" alt="UAV Disaster Damage Detection screenshot" />
      <p>After natural disasters, a quick and accurate damage assessment is crucial for an effective response. The core problem our project seeks to address is how to provide a faster and reliable damage assessment of disaster areas. To achieve this goal, the project performed fine-tuning on a DeepLabV3 model with a natural disaster image dataset called RescueNet. The model achieved an IoU score of 50.6% after only 7 epochs of training. While not the level of performance the team was looking for, the model performed well given the limited computational resources.</p>
      <a href="https://github.com/Jhansen19/DisasterRecoverySegmentation/tree/main" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>
    
    <!-- Project 2 -->
    <div class="project-card">
      <div class="date">Mar 2025</div>
      <h3>Housing Price Prediction: Using DL Models SOM and ANN</h3>
      <img src="{{ site.baseurl }}/assets/images/HousingPred.jpg" alt="Housing Price Prediction screenshot" />
      <p>A Python-based project that predicts Boston-area home values by first using Deep Learning (SOM and ANN) to automatically group similar neighborhoods, then feeding those groupings into a neural network for price forecasting. Built with tools (pandas, scikit-learn, MiniSom and TensorFlow), it delivers strong accuracy which explains over 80% of the variation in sale prices while showcasing how unsupervised clustering can bolster deep learning models.</p>
      <a href="https://github.com/Jhansen19/Housing_Pred_AnnSOM/tree/main" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>
    
    <!-- Project 3 -->
    <div class="project-card">
      <div class="date">Jun 2025</div>
      <h3>US Freight Rail Risk Analysis: Indiana Accident Prediction</h3>
      <img src="{{ site.baseurl }}/assets/images/accidentpred.jpg" alt="US Freight Rail Risk Analysis screenshot" />
      <p>Integrated train volume, historical accident, commodity hazard, and community vulnerability data to predict accident risk on Indiana rail segments. Generated an interactive Folium map highlighting high-risk corridors—especially those carrying hazardous goods through vulnerable communities—for state safety planning.</p>
      <a href="https://github.com/Jhansen19/Rail_Accident_Predictions" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>
    
    <!-- Project 4 -->
    <div class="project-card">
      <div class="date">Feb 2025</div>
      <h3>Airline Prediction: Azure Data Lake Pipeline</h3>
      <img src="{{ site.baseurl }}/assets/images/AzurePipe.jpg" alt="Airline Prediction screenshot" />
      <p>Built an end-to-end ELT pipeline in Azure that ingests raw CSVs from the Bureau of Transportation Statistics into Data Lake Storage Gen2, cleans and transforms them with Azure Data Factory and Spark, and publishes ready-to-use silver and gold tables for machine learning. I configured resource groups, integration runtimes, Data Factory pipelines, and Key Vault–secured credentials, while leveraging geo-redundant storage and a medallion architecture to ensure scalability, reliability, and cost efficiency. This project demonstrates my ability to design and deploy robust cloud data pipelines that handle big data at scale.</p>
      <a href="https://github.com/Jhansen19/Airline_Predictions" target="_blank">
        <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>
        View on GitHub
      </a>
    </div>

  </div>
</div>


