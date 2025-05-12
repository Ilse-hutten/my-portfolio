---
layout: single
title: "CV"
permalink: /cv/
classes: wide
---

<style>
  /* Ensure full-width content stays centered */
  .wide {
    max-width: 1100px;
    margin: 0 auto;
  }

  /* Improve overall font styling for a professional look */
  body {
    font-family: 'Lato', 'Helvetica Neue', Helvetica, Arial, sans-serif;
    font-size: 15px;
    color: #232323;
    line-height: 1.7;
    background-color: #ffffff !important; /* Force white background */
  }

  /* CV wrapper for structured layout */
  .cv-wrapper {
    max-width: 1100px; /* Wider for better spacing */
    margin: 40px auto;
    padding: 2rem 2rem;
    background: #fff;
    border-radius: 10px;
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.08);
    font-size: 1rem;
  }

  /* Header & title adjustments */
  .cv-header {
    text-align: center;
    margin-bottom: 2rem;
  }

  .cv-header h1 {
    font-size: 1.3rem;
    font-weight: 700;
    letter-spacing: 1px;
    margin-bottom: 0.2rem;
    color: #1e293b;
  }

  /* Consistent navigation title sizing */
  .site-title {
    font-size: 1.2rem !important;
    font-weight: 600;
    color: #1e293b;
  }

  /* Contact details */
  .cv-contact {
    font-size: 0.95rem;
    color: #52525b;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.2rem;
  }

  /* Section styling */
  .cv-section {
    margin-bottom: 1.5rem;
  }

  .cv-section h2 {
    font-size: 1rem;
    font-weight: 700;
    color: #2563eb;
    border-bottom: 1.5px solid #e5e7eb;
    padding-bottom: 0.25rem;
    margin-bottom: 1rem;
    letter-spacing: 0.5px;
    text-transform: uppercase;
  }

  /* Job titles and organization formatting */
  .cv-role {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 0.5rem;
  }

  .cv-role-title {
    font-weight: 600;
    color: #1e293b;
    font-size: 1rem;
  }

  .cv-organization {
    font-style: italic;
    color: #64748b;
    font-size: 0.95rem;
  }

  .cv-description {
    margin-left: 1rem;
    font-size: 0.95rem;
  }

  /* Bullet points formatting */
  ul.cv-bullets {
    margin: 0.3rem 0 0.5rem 1.2rem;
    font-size: 0.95rem;
    color: #374151;
  }

  /* Footer formatting */
  .cv-footer {
    text-align: center;
    font-size: 0.9rem;
    color: #9ca3af;
    margin-top: 2rem;
  }

  /* Responsive tweaks */
  @media (min-width: 1200px) {
    .cv-wrapper { font-size: 1rem; }
    .cv-header h1 { font-size: 1.3rem; }
    .cv-section h2 { font-size: 1rem; }
  }

  @media (max-width: 600px) {
    .cv-wrapper { padding: 1.1rem 0.5rem; }
    .cv-header h1 { font-size: 1.1rem; }
    .cv-section h2 { font-size: 0.95rem; }
    .cv-role { flex-direction: column; gap: 0.1rem; }
  }
</style>

<div class="cv-wrapper">
  <div class="cv-header">
    <h1>Ilse Hutten</h1>
    <div class="cv-contact">
      📞 +31 6 10738270 &nbsp;|&nbsp; 📧 huttenilse@gmail.com &nbsp;|&nbsp;
      <a href="https://www.linkedin.com/in/ilsehutten" style="color:#2563eb;text-decoration:none;">linkedin.com/in/ilsehutten</a>
    </div>
  </div>

  <div class="cv-section">
    <h2>Profile</h2>
    <p>Data science professional with 3+ years of experience in investment banking and financial analysis. Expertise in machine learning, data analysis, and financial modeling.</p>
  </div>

  <div class="cv-section">
    <h2>Skills</h2>
    <ul class="cv-bullets">
      <li>Python, SQL, Pandas, NumPy, Scikit-learn, TensorFlow, Matplotlib, Seaborn, Keras</li>
      <li>Financial Modeling, Data Visualization, Statistical Analysis</li>
      <li>VBA, Machine Learning, Time Series Analysis</li>
    </ul>
  </div>

  <div class="cv-section">
    <h2>Experience</h2>
    <div class="cv-role">
      <div>
        <div class="cv-role-title">Investment Banking Associate – Equity Advisory</div>
        <div class="cv-organization">Nomura, London, UK</div>
        <ul class="cv-bullets">
          <li>Advised clients on equity transactions and capital raising strategies.</li>
          <li>Built financial models and performed market analysis for IPOs and secondary offerings.</li>
        </ul>
      </div>
      <div>Apr 2022 – Jan 2025</div>
    </div>
    <div class="cv-role">
      <div>
        <div class="cv-role-title">Private Equity Intern</div>
        <div class="cv-organization">3i Group, Amsterdam, NL</div>
        <ul class="cv-bullets">
          <li>Supported due diligence and financial analysis for investment opportunities.</li>
        </ul>
      </div>
      <div>Sep 2021 – Dec 2021</div>
    </div>
  </div>

  <div class="cv-section">
    <h2>Education</h2>
    <div class="cv-role">
      <div>
        <div class="cv-role-title">Le Wagon, London, UK</div>
        <div class="cv-organization">Data Science & Machine Learning Bootcamp</div>
      </div>
      <div>Jan 2025 – Mar 2025</div>
    </div>
  </div>

  <div class="cv-section">
    <h2>Languages</h2>
    <p>Dutch (Native), English (Fluent)</p>
  </div>
</div>
