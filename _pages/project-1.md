---
permalink: projects/project-twitter-sentiment/
title: "Stock Prediction with Twitter Sentiment"
layout: single
classes: container

header:
  overlay_image: /assets/images/nlp.jpg
  overlay_filter: 0.3
---

<h2 style="font-size: 22px; margin-top: 0; color: #333;">Stock Prediction with Twitter Sentiment</h2>

<p style="font-size: 15px; line-height: 1.7; color: #444;">
This project explores whether social media sentiment—specifically Twitter/X mentions of Amazon and Netflix—can predict stock price movements. Using Natural Language Processing (NLP) and supervised machine learning models, I developed a sentiment-based trading strategy and evaluated its performance against traditional buy-and-hold benchmarks.
</p>

<h3 style="font-size: 18px; color: #333;"> Project Workflow</h3>

<ol style="font-size: 15px; line-height: 1.7; color: #444; padding-left: 20px;">
  <li><strong>Tweet Scraping:</strong> Historical tweets were collected using Playwright from accounts mentioning Amazon and Netflix.</li>
  <li><strong>Sentiment Analysis:</strong> Tweets were cleaned, processed, and analyzed using VADER to assign sentiment scores (positive, neutral, negative).</li>
  <li><strong>ML Modeling:</strong> Trained Logistic Regression, Support Vector Machine (SVM), and Multi-Layer Perceptron (MLP) models to predict price direction from sentiment.</li>
  <li><strong>Strategy Development:</strong> Built a trading algorithm using model outputs to generate long/short signals, then backtested performance.</li>
</ol>

<h3 style="font-size: 18px; color: #333;"> Sentiment Distribution</h3>

<p style="font-size: 15px; line-height: 1.7; color: #444;">
The chart below shows the distribution of sentiment extracted from tweets mentioning Amazon and Netflix.
</p>

<img src="https://Ilse-hutten.github.io/my-portfolio/assets/images/twitter_sentiment_distribution.png" alt="Sentiment Distribution" style="width: 100%; border-radius: 8px; margin: 20px 0;"/>

<h3 style="font-size: 18px; color: #333;"> Model Performance</h3>

<p style="font-size: 15px; line-height: 1.7; color: #444;">
The models achieved high recall, meaning they successfully captured most of the positive stock movement signals. However, precision remained relatively low, indicating many false positives. This imbalance is partly due to the skewed nature of the dataset — with a higher proportion of positive sentiment labels, the models tend to overpredict positive outcomes. Addressing this through class balancing techniques (such as resampling or adjusting class weights) could improve precision and overall model robustness. These findings also align with academic research, which shows that sentiment alone offers limited predictive power unless combined with other indicators.
</p>

<img src="https://Ilse-hutten.github.io/my-portfolio/assets/images/twitter_model_performance.png" alt="Model Performance" style="width: 100%; border-radius: 8px; margin: 20px 0;"/>

<h3 style="font-size: 18px; color: #333;"> Strategy vs. Buy & Hold</h3>

<p style="font-size: 15px; line-height: 1.7; color: #444;">
The backtested trading strategy outperformed a buy-and-hold approach on both Amazon and Netflix. Below are performance comparison charts and a metrics summary.
</p>

<img src="https://Ilse-hutten.github.io/my-portfolio/assets/images/twitter_strategy_vs_buyhold.png" alt="Trading Strategy vs Buy and Hold" style="width: 100%; border-radius: 8px; margin: 20px 0;"/>

<img src="https://Ilse-hutten.github.io/my-portfolio/assets/images/twitter_strategy_vs_buyhold_table.png" alt="Strategy Performance Table" style="width: 100%; border-radius: 8px; margin: 20px 0;"/>

<h3 style="font-size: 18px; color: #333;"> Technologies Used</h3>

<ul style="font-size: 15px; line-height: 1.7; color: #444;">
  <li>Python, Pandas, scikit-learn</li>
  <li>Playwright (for scraping), VADER (for sentiment analysis)</li>
  <li>Matplotlib, Seaborn (for visualization)</li>
</ul>

<h3 style="font-size: 18px; color: #333;"> Results Summary</h3>

<ul style="font-size: 15px; line-height: 1.7; color: #444;">
  <li>For both Amazon and Netflix, the sentiment-based trading strategies outperformed a basic buy-and-hold strategy during the backtesting period.</li>
  <li>However, model performance metrics (accuracy, precision, recall) were relatively low, aligning with findings in similar academic research.</li>
  <li>This suggests that results could be driven by chance.</li>
  <li>Further improvements, including more features, alternative sentiment models, and larger datasets, are recommended for enhanced strategy robustness.</li>
</ul>


<h3 style="font-size: 18px; color: #333;"> Future Improvements</h3>

<ul style="font-size: 15px; line-height: 1.7; color: #444;">
  <li>Integrate additional sentiment sources like Reddit and financial news headlines</li>
  <li>Expand to more stocks and incorporate transaction costs</li>
  <li>Enhance models using LSTM or ensemble techniques</li>
  <li>Add technical indicators to enrich the feature set</li>
</ul>

<p style="margin-top: 20px;">
  <a href="https://github.com/Ilse-hutten/tweet-stock-prediction" style="font-size: 16px; color: white; background-color: #007acc; padding: 8px 14px; border-radius: 5px; text-decoration: none;">
    🔗 View on GitHub
  </a>
</p>

<p style="font-size: 15px; line-height: 1.7; margin-top: 30px;">
  <a href="https://ilse-hutten.github.io/my-portfolio/projects/" style="text-decoration: none; color: #007acc;">🔙 Back to Projects</a>
</p>
