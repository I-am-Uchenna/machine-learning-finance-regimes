# Machine Learning in Finance: Market Regime & Direction Prediction

**Author:** Uchenna Ejike  
**Date:** January 2026

## Executive Summary

This project applies advanced machine learning techniques to financial time-series data to solve two critical problems in quantitative finance: predicting daily market direction (binary classification) and identifying market volatility regimes (multiclass classification).

Using a dataset of eight major ETFs (including SPY, TLT, GLD, and VNQ) spanning 2015–2024, the analysis evaluates the efficacy of **Linear Discriminant Analysis (LDA)**, **Support Vector Machines (SVM)**, and **Neural Networks (NN)**.

## Key Objectives

1.  **Binary Classification:** Predict whether the market closes higher or lower on the next trading day.
2.  **Multiclass Classification:** Categorize market conditions into specific volatility-return regimes to inform risk management strategies.

## Methodology

The project implements a rigorous quantitative pipeline:

* **Data Engineering:** Generated 88 technical indicators/features from daily OHLCV data.
* **Dimensionality Reduction:** Utilized LDA to project high-dimensional financial data into a lower-dimensional space, maximizing class separability.
* **Non-Linear Modeling:** Applied SVM with Radial Basis Function (RBF) kernels and Neural Networks to capture complex, non-linear market dependencies.
* **Validation:** Employed K-Fold Cross-Validation to ensure model stability and prevent overfitting.

## Principal Findings

* **Market Efficiency:** Daily directional prediction proved challenging, with ROC-AUC scores converging near 0.5, supporting the weak-form Efficient Market Hypothesis (EMH) for short-term price movements.
* **Regime Identification:** Machine learning models significantly outperformed random baselines in detecting market regimes (volatility clusters), achieving accuracy gains of 13-15%.
* **Model Selection:** LDA provided the highest interpretability for regulatory compliance, while Neural Networks offered superior adaptability to non-linear patterns when sufficient data was available.

## Repository Structure

* `notebooks/` - Jupyter Notebook containing the end-to-end Python code for data fetching, preprocessing, and model training.
* `reports/` - A comprehensive PDF technical report detailing the mathematical theoretical background and literature review.

## Dependencies

* Python 3.8+
* `scikit-learn`
* `yfinance`
* `pandas` & `numpy`
* `matplotlib` & `seaborn`

## Disclaimer

This project is for educational and research purposes only. It does not constitute financial advice.

---
© 2026 Uchenna Ejike. All Rights Reserved.
