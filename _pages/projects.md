---
permalink: /projects/
title: "Projects"
layout: single
---


Here are some of my recent data science and machine learning projects:

---

<style>
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.project-card {
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  background: #fff;
  transition: box-shadow 0.2s ease-in-out;
}

.project-card:hover {
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.1);
}

.project-card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
}

.project-card-content {
  padding: 1rem;
}

.project-card h3 {
  margin-top: 0;
  font-size: 1.2rem;
}

.project-card p {
  font-size: 0.95rem;
  color: #444;
}

.project-card a {
  display: inline-block;
  margin-top: 0.5rem;
  font-weight: bold;
  color: #007acc;
}
</style>

<div class="project-grid">
  <div class="project-card">
    <img src="{{ '/assets/images/nlp.jpg' | relative_url }}" alt="Twitter Sentiment Project">
    <div class="project-card-content">
      <h3>Stock Prediction with Twitter Sentiment</h3>
      <p>Built an ML pipeline to predict stock movements based on tweet sentiment. Strategy outperformed a benchmark in backtests.</p>
      <a href="./project-twitter-sentiment">Read more →</a>
    </div>
  </div>

  <div class="project-card">
    <<img src="{{ '/assets/images/nlp.jpg' | relative_url }}" alt="PCA Index Arbitrage">
    <div class="project-card-content">
      <h3>Index Arbitrage using PCA</h3>
      <p>Used Principal Component Analysis to detect index mispricings and design a z-score based mean reversion strategy.</p>
      <a href="./project-pca-strategy">Read more →</a>
    </div>
  </div>

  <!-- Add more cards here -->
</div>
