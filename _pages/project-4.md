---
permalink: projects/project-strategy-simulator/
title: "Operational Strategy Simulator"
layout: single
classes: "container medium"

header:
  overlay_image: /assets/images/simulator_header.png
  overlay_filter: 0.3
---

<h2 style="font-size: 22px; margin-top: 0; color: #333;">Optimizing Strategic Initiatives under Budget & Resource Constraints</h2>

<p style="font-size: 15px; line-height: 1.7; color: #444;">
This Streamlit app helps simulate and optimize combinations of strategic initiatives for a fintech company based on cost, engineering effort, to maximize ARR / ROI. It allows for both manual selection and automated optimization using a knapsack model, while also visualizing ROI risk through Monte Carlo simulations.
</p>

<h3 style="font-size: 18px; color: #333;">Features</h3>
<ul style="font-size: 15px; line-height: 1.7; color: #444;">
  <li>Dynamic budget and engineering constraints</li>
  <li>Manual and automated initiative selection</li>
  <li>Optimization based on either ARR or ROI</li>
  <li>Monte Carlo simulation for ROI uncertainty</li>
  <li>Clean, responsive UI with intuitive summaries</li>
</ul>

<h3 style="font-size: 18px; color: #333;">Optimization Logic</h3>
<ul style="font-size: 15px; line-height: 1.7;">
  <li>Each initiative is a binary decision: selected (1) or not (0)</li>
  <li><strong>Maximize ARR:</strong> sum of expected ARR impact from selected initiatives</li>
  <li><strong>Maximize ROI:</strong> total ROI (ARR used as proxy, minus cost)</li>
  <li><strong>Constraints:</strong> total cost & engineering days must stay within user-defined limits</li>
</ul>

<h3 style="font-size: 18px; color: #333;">Exploratory Insights</h3>
<ul style="font-size: 15px; line-height: 1.7;">
  <li><strong>ROI by Confidence Level:</strong> High/Medium confidence initiatives show higher median ROI (~7.5–8), while Low confidence hovers around ~5 with limited upside.</li>
  <li><strong>ROI vs Engineering Days:</strong> No clear correlation. High ROI can come from both low and medium engineering efforts.</li>
  <li><strong>ARR vs Confidence:</strong> High confidence initiatives offer more consistent and higher ARR potential. Low confidence may appear high-ARR, but often pair with low ROI.</li>
  <li><strong>ARR vs Engineering:</strong> Higher ARR generally requires more effort, but rare low-effort/high-impact outliers exist.</li>
</ul>

<img src="https://Ilse-hutten.github.io/my-portfolio/assets/images/initiative_performance.png" alt="exploratory insights" style="width: 80%; border-radius: 8px;"/>

<h3 style="font-size: 18px; color: #333;">Monte Carlo Simulation</h3>
<p style="font-size: 15px; color: #444;">
Each run simulates ARR outcomes with randomized noise based on initiative confidence levels. In "Bad" scenarios, additional cost overruns are introduced. This enables risk-adjusted ROI forecasting across scenarios.
</p>
<img src="https://Ilse-hutten.github.io/my-portfolio/assets/images/monte_carlo_roi.png" alt="exploratory insights" style="width: 80%; border-radius: 8px;"/>

<video autoplay loop muted playsinline style="width: 100%; border-radius: 8px; margin: 20px 0;">
  <source src="https://Ilse-hutten.github.io/my-portfolio/assets/videos/strategy_simulator.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<h3 style="font-size: 18px; color: #333;">Live App</h3>
<p style="font-size: 15px;"><a href="https://operational-strategy-simulator-hxdqqzqz8i6s5kagkvryc3.streamlit.app" target="_blank">🔗 Launch Operational Strategy Simulator</a></p>

<p style="font-size: 15px;">
<a href="https://ilse-hutten.github.io/my-portfolio/projects/" style="text-decoration: none; color: #007acc;">🔙 Back to Projects</a>
</p>
