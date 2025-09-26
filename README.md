# sp500-analysis-ml
A data processing and machine learning analysis project on the S&amp;P 500 dataset, exploring financial market trends, feature engineering, clustering, and predictive modeling using regression, ensemble methods, and classification models.

# S&P 500 Analysis and Machine Learning Project

This repository contains data analysis, feature engineering, and machine learning models built on the [S&P 500 dataset](https://datahub.io/core/s-and-p-500#readme).  
The project focuses on exploring financial market trends, cleaning and processing data, applying statistical analysis, and building predictive models.

---

## 📊 Dataset
The dataset used in this project is the **S&amp;P 500 financial dataset**, which includes historical data such as:
- S&P 500 Index values
- Dividends
- Earnings
- Consumer Price Index (CPI)
- PE10 ratio
- Long-term interest rates  

Dataset source: [Core Data Hub – S&P 500](https://datahub.io/core/s-and-p-500#readme)

---

## ⚡ Project Workflow

### **1. Big Data Processing**
- Converted date strings into pandas datetime objects  
- Identified and handled duplicate rows (1833 → 1681 rows after cleaning)  
- Calculated statistical summaries of all fields  
- Explored correlations (e.g., strong correlation between S&P 500 and CPI)  
- Visualized relationships using scatter plots  

### **2. Feature Engineering**
- Created new features such as:
  - Year-over-year CPI change (%)
  - 12-month rolling average of earnings
  - Normalized S&P 500 index values  
- Identified top trends in CPI fluctuations and earnings growth  

### **3. Data Visualization**
- Histogram of S&P 500 values (non-normal distribution, long tail)  
- Box plot of PE10 ratio (right-skewed, with speculative bubble outliers)  
- Correlation heatmap of numerical features  
- Insights into stock valuations and interest rate effects  

### **4. Machine Learning Models**
- **K-Means Clustering**: Market regimes (early, mid, modern periods)  
- **Regression Models**:  
  - Linear Regression: R² = 0.99, MSE ≈ 4701 (overfitting risk)  
  - Random Forest: R² = 1.0, MSE ≈ 473 (high accuracy, possible overfitting)  
- **Classification Models (CPI Trend Prediction)**:
  - Logistic Regression: 67% accuracy  
  - Support Vector Machine (SVM): 67% accuracy (balanced precision/recall)  
  - KNN: 64% accuracy  
  - Neural Network: ~67% accuracy, comparable to Logistic Regression & SVM  

---

## 📂 Repository Structure
├── analysis.ipynb # Jupyter Notebook with code and analysis
├── analysis Report.pdf # Detailed project report
└── README.md # Project documentation