# 📈 Nifty 50 Stock Clustering using Machine Learning

A complete **Unsupervised Machine Learning** project that clusters **Nifty 50 stocks** based on their historical risk and return characteristics. This project demonstrates how machine learning can identify groups of stocks with similar behavior, helping investors understand market structure and portfolio diversification.

---

## 📌 Project Overview

The Indian stock market consists of companies from multiple sectors, each exhibiting different levels of return, volatility, and risk.

Instead of manually categorizing stocks, this project applies **K-Means Clustering** to automatically group Nifty 50 stocks based on their financial characteristics.

The workflow covers the complete machine learning pipeline:

- Data Collection
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Scaling
- Dimensionality Reduction (PCA)
- Unsupervised Machine Learning (K-Means Clustering)
- Cluster Visualization
- Business Insights

---

## 🎯 Objectives

- Analyze historical performance of Nifty 50 stocks.
- Engineer meaningful financial features.
- Cluster stocks with similar behavior using Machine Learning.
- Visualize clusters in two dimensions using PCA.
- Interpret each cluster from an investment perspective.

---



# 📊 Dataset

### Source

Historical stock price data was downloaded using the **Yahoo Finance API (yfinance)**.

### Stocks

The project uses companies from the **Nifty 50 Index**.

### Time Period

- January 2021 – December 2025

### Data Collected

For every stock:

- Open
- High
- Low
- Close
- Volume

---

# ⚙️ Technologies Used

| Category | Tools |
|-----------|-------|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Data Source | yfinance |
| Machine Learning | Scikit-learn |
| Dimensionality Reduction | PCA |
| Clustering | K-Means |

---

# 📈 Machine Learning Workflow

## 1. Data Collection

Historical stock prices were downloaded using **yfinance**.

---

## 2. Data Cleaning

- Removed missing values
- Aligned trading dates
- Calculated daily returns

---

## 3. Exploratory Data Analysis

Performed analysis such as:

- Return distributions
- Correlation heatmap
- Summary statistics

---

## 4. Feature Engineering

Each stock was represented using four financial features:

| Feature | Description |
|----------|-------------|
| Annual Return | Average yearly return |
| Annual Volatility | Annualized standard deviation of returns |
| Sharpe Ratio | Risk-adjusted return |
| Maximum Drawdown | Largest observed decline from peak |

These features summarize each stock's performance into a machine-learning-friendly format.

---

## 5. Feature Scaling

Used **StandardScaler** to standardize the features so that each has:

- Mean = 0
- Standard Deviation = 1

Standardization ensures that all features contribute equally to distance calculations, which is important for algorithms like **PCA** and **K-Means Clustering**.

---

## 6. Principal Component Analysis (PCA)

Reduced the feature space from **4 dimensions to 2 dimensions**.

Benefits:

- Easier visualization
- Reduced redundancy
- Better understanding of clusters

---

## 7. K-Means Clustering

Applied the **K-Means** algorithm to group similar stocks.

The **Elbow Method** was used to determine the optimal number of clusters.

---

## 8. Cluster Analysis

Calculated average statistics for every cluster:

- Annual Return
- Annual Volatility
- Sharpe Ratio
- Maximum Drawdown

This helps interpret each cluster from an investment perspective.

---

# 📊 Features Used

| Feature | Importance |
|----------|------------|
| Annual Return | Measures profitability |
| Annual Volatility | Measures risk |
| Sharpe Ratio | Measures risk-adjusted performance |
| Maximum Drawdown | Measures downside risk |

---

# 📉 Visualizations

The project includes several visualizations:

- Return Distribution
- Correlation Heatmap
- Elbow Method Plot
- PCA Scatter Plot

---

# 📌 PCA Cluster Visualization

After dimensionality reduction, every stock is plotted on a 2D plane.

- Each point represents one stock.
- Different colors represent different clusters.
- Nearby stocks have similar financial characteristics.

---

# 📊 Cluster Interpretation

Each cluster represents stocks with similar investment characteristics.

Examples:

- High Return – High Risk
- Stable Moderate Return
- Defensive Low Volatility
- Underperforming Stocks

The exact interpretation depends on the clustering results.

---


# 📌 Results

The model successfully grouped Nifty 50 stocks into distinct clusters based on risk and return characteristics.

The clustering enables:

- Identification of similar stocks
- Better understanding of market behavior
- Portfolio diversification insights
- Risk profiling of companies

---

# 📈 Key Insights

- **Cluster 0 – Balanced Performers:** Stocks in this cluster delivered **moderately high annual returns (22.99%)** with **controlled volatility (24.68%)** and the **lowest maximum drawdown (-29.90%)** among all clusters. These stocks offer a balanced risk-return profile.

- **Cluster 1 – Conservative / Underperforming Stocks:** This cluster recorded the **lowest annual returns (8.51%)** and the **lowest Sharpe Ratio (0.056)**, indicating poor risk-adjusted performance despite having volatility similar to Cluster 0.

- **Cluster 2 – Best Risk-Adjusted Performers:** Stocks in this cluster achieved the **highest annual return (36.80%)** along with the **highest Sharpe Ratio (0.906)**, suggesting the best balance between return and risk. Although volatility was higher than Clusters 0 and 1, the superior returns compensated for the additional risk.

- **Cluster 3 – High-Risk, High-Return Stocks:** This cluster generated **high annual returns (36.65%)** but also exhibited the **highest volatility (49.08%)** and the **largest maximum drawdown (-72.68%)**. These stocks may suit aggressive investors who can tolerate significant price fluctuations.

### Overall Observations

- The clustering successfully separated Nifty 50 stocks into groups with distinct **risk-return characteristics**.
- Higher returns generally came with increased volatility and larger drawdowns.
- **Cluster 2** offered the strongest **risk-adjusted performance**, while **Cluster 3** represented the most aggressive investment profile.
- The results demonstrate how **K-Means Clustering** can uncover meaningful patterns in financial data without predefined labels, helping investors understand stock behavior and support portfolio diversification.

---


# 💡 Learning Outcomes

This project demonstrates practical applications of:

- Data Collection
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Feature Scaling
- Principal Component Analysis (PCA)
- K-Means Clustering
- Cluster Interpretation
- Financial Data Analysis

---


# 🙋 Author

**Ashutosh Kashyap**

```