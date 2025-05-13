---
permalink: projects/project-telco-churn/
title: "Customer Churn Prediction for Telco"
layout: single
classes: "container medium"

header:
  overlay_image: /assets/images/telco_header.png
  overlay_filter: 0.3
---

<h2 style="font-size: 22px; margin-top: 0; color: #333;">Customer Churn Prediction for a Telco Provider</h2>

<p style="font-size: 15px; line-height: 1.7; color: #444;">
This project applies supervised machine learning to predict customer churn for a telecommunications company. The goal is to identify customers at high risk of leaving and enable proactive retention strategies.
</p>

<h3 style="font-size: 18px; color: #333;"> Business Context</h3>

<ul style="font-size: 15px; line-height: 1.7; color: #444;">
  <li>Churn is costly: retaining existing customers is far cheaper than acquiring new ones.</li>
  <li>The dataset includes customer demographics, account info, contract types, and service usage.</li>
  <li>Understanding churn drivers enables more targeted offers, better customer support, and higher retention.</li>
</ul>

<h3 style="font-size: 18px; color: #333;"> Data Exploration & Key Insights</h3>

<p style="font-size: 15px;">The dataset is imbalanced: ~73% of customers do not churn.</p>

<img src="/assets/images/churn_distribution.png" alt="Churn Distribution" style="width: 50%; border-radius: 8px; margin: 20px 0;"/>

<p style="font-size: 15px; margin-top: 20px;">Key patterns observed across customer segments:</p>

<ul style="font-size: 15px; line-height: 1.7;">
  <li>Senior citizens have ~40% churn vs 23% for others.</li>
  <li>Customers without partners or dependents churn more.</li>
  <li>Gender is not a significant churn factor.</li>
</ul>

<img src="/assets/images/churn_rate_demographics.png" style="width: 100%; border-radius: 8px;"/>
<img src="/assets/images/customer_count_demographics.png" style="width: 100%; border-radius: 8px;"/>

<p style="margin-top: 20px;">Service and contract features also show strong signals:</p>

<ul style="font-size: 15px; line-height: 1.7;">
  <li>Fiber optic users churn ~2x more than DSL users.</li>
  <li>Churn is much higher without tech support or online security add-ons.</li>
  <li>Month-to-month contracts have the highest churn (~40%).</li>
</ul>

<img src="/assets/images/churn_rate_service_contract.png" style="width: 100%; border-radius: 8px;"/>

<h3 style="font-size: 18px; color: #333;"> Preprocessing</h3>

<ul style="font-size: 15px; line-height: 1.7;">
  <li>One-hot encoding applied to categorical features (no ordinal values).</li>
  <li>SMOTE used to address class imbalance in churn labels.</li>
  <li>Scaling applied where needed for model compatibility.</li>
</ul>

<h3 style="font-size: 18px; color: #333;"> Model Performance</h3>

<p style="font-size: 15px;">Four classifiers were tested and compared across evaluation metrics:</p>

<table style="font-size: 14px;">
<thead>
<tr>
  <th>Model</th><th>ROC AUC</th><th>Accuracy</th><th>Precision</th><th>Recall</th><th>F1 Score</th>
</tr>
</thead>
<tbody>
<tr><td>Random Forest</td><td>0.8263</td><td>0.7640</td><td>0.5438</td><td>0.6979</td><td>0.6112</td></tr>
<tr><td>Logistic Regression</td><td>0.8316</td><td>0.7356</td><td>0.5017</td><td><b>0.7914</b></td><td>0.6141</td></tr>
<tr><td>Gradient Boosting</td><td>0.8316</td><td><b>0.7719</b></td><td><b>0.5604</b></td><td>0.6578</td><td>0.6052</td></tr>
<tr><td>XGBoost</td><td><b>0.8318</b></td><td>0.7676</td><td>0.5512</td><td>0.6765</td><td><b>0.6074</b></td></tr>
</tbody>
</table>

<img src="/assets/images/roc_auc_across_models.png" alt="ROC AUC Comparison" style="width: 70%; border-radius: 8px; margin: 20px 0;"/>

<h3 style="font-size: 18px; color: #333;"> Feature Importance</h3>

<ul style="font-size: 15px; line-height: 1.7;">
  <li>Month-to-month contracts are consistently the top predictor of churn.</li>
  <li>Short tenure, lack of tech support, and use of electronic checks also indicate high churn risk.</li>
  <li>Gradient Boosting emphasizes a few key features, while XGBoost distributes importance more evenly.</li>
</ul>

<img src="/assets/images/feature_importance.png" alt="Feature Importance" style="width: 100%; border-radius: 8px;"/>

<h3 style="font-size: 18px; color: #333;"> Strategic Takeaways</h3>

<ul style="font-size: 15px; line-height: 1.7;">
  <li><strong>Target month-to-month users</strong> with incentives to switch to longer-term contracts.</li>
  <li><strong>Offer tech support and security add-ons</strong> to increase retention.</li>
  <li><strong>Review billing issues</strong> tied to electronic check users to reduce frustration-related churn.</li>
</ul>

<h3 style="font-size: 18px; color: #333;"> Technologies Used</h3>

<ul style="font-size: 15px; line-height: 1.7; color: #444;">
  <li>Python, Pandas, scikit-learn, XGBoost</li>
  <li>SMOTE (from imbalanced-learn), Matplotlib, Seaborn</li>
  <li>Jupyter, modular pipeline via custom scripts</li>
</ul>

<h3 style="font-size: 18px; color: #333;"> Future Improvements</h3>

<ul style="font-size: 15px; line-height: 1.7;">
  <li>Use SHAP or LIME for more explainable predictions</li>
  <li>Deploy model as a REST API or dashboard</li>
  <li>Incorporate customer lifetime value in retention targeting</li>
</ul>

<p style="margin-top: 20px;">
  <a href="https://github.com/Ilse-hutten/telco-customer-churn" style="font-size: 16px; color: white; background-color: #007acc; padding: 8px 14px; border-radius: 5px; text-decoration: none;">
    🔗 View on GitHub
  </a>
</p>

<p style="font-size: 15px; line-height: 1.7; margin-top: 30px;">
  <a href="https://ilse-hutten.github.io/my-portfolio/projects/" style="text-decoration: none; color: #007acc;">🔙 Back to Projects</a>
</p>
