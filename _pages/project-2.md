---
permalink: projects/project-pca-strategy/
title: "Index Arbitrage Trading Strategy Using PCA"
layout: single
author_profile: true
---

# Index Arbitrage Trading Strategy Using PCA

This project implements a **PCA-based index arbitrage trading strategy** designed to replicate major stock indexes like the FTSE100 using Principal Component Analysis (PCA) and statistical mean reversion principles.

Developed during the **Le Wagon Data Science and AI Bootcamp**, I implemented the PCA method to identify stocks that closely mirror the behavior of a target index. The strategy assumes that the spread between the replicated portfolio and the index will revert to the mean, providing trading signals.

---

### Objective

The goal of this project was to explore an **index arbitrage strategy** using **PCA** to identify stocks whose returns closely mimic an index, enabling the construction of a **replicated portfolio**. The portfolio is then monitored for mean reversion signals to execute trades, assuming the spread between the portfolio and index would revert over time.

---

### Approach

1. **Data Collection**: Stock price data was sourced from publicly available financial datasets (e.g., FTSE100).
2. **PCA Implementation**: I applied **Principal Component Analysis (PCA)** to extract the principal components of the stock returns and used these components to identify a group of stocks that could replicate the index.
3. **Mean Reversion Strategy**: Using the **z-score** of the spread between the replicated portfolio and the index, I created **buy** and **sell** signals based on mean reversion (e.g., buying when the spread is too negative and selling when it’s too positive).
4. **Backtesting**: The strategy was backtested on historical data to simulate real-world trading and evaluate the effectiveness of the model.

---

### Results

- **Performance**: The strategy successfully detected **mean reversion opportunities** with a high level of consistency, achieving a **positive return on trades**.
- **Visualization**: Below is an example of the **z-score** analysis that drove the trading signals. The trading decisions are based on deviations greater than **±2 standard deviations**.

![Z-Score Chart](./assets/zscore_chart.png)

- **Interactive Web Interface**: The project includes a **Streamlit app** that allows users to explore and interact with the strategy’s performance, adjust parameters, and view results in real-time.

**Click below to explore the Streamlit app live**:
[Explore Interactive Demo](#)

---

### Key Takeaways

- The project demonstrated how **PCA** can be effectively used to replicate an index and develop an arbitrage strategy.
- **Mean reversion trading** strategies can be useful in capturing short-term inefficiencies in the market.
- The project also emphasizes the importance of **visualizing model results**, which helps in **understanding model performance** and making data-driven decisions.

---

### Demo (Optional)

You can interact with the trading strategy live by visiting the **Streamlit app**. The app allows for experimenting with different market conditions, backtest performance, and visualize the data.

---

[🔙 Back to Projects](/projects/)
