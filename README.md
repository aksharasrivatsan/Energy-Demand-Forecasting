# Energy-Demand-Forecasting
Developed a comprehensive Deep Learning framework to address the complexities of energy demand forecasting across different temporal scales. This project implements a Three-Tier Architecture that transitions from immediate grid operations to long-term national strategic planning by utilizing three distinct global datasets.

Multi-Horizon Energy Load Forecasting: A Three-Tier LSTM Framework
This repository contains a comprehensive deep learning solution for electrical load forecasting, validated across three distinct global regions and temporal horizons. The project was presented at the International Conference on Sustainable and Efficient Energy Solutions (ICSEES) 2026, AICTE.

Project Overview
Traditional forecasting models often struggle with the non-linear complexity of energy grids. This project addresses the gap by implementing a Three-Tier Architecture, training specialized LSTM models for Operational, Seasonal, and Strategic forecasting.

The Three-Tier Architecture
1. Short-Term Operational Tier (PJM Dataset - USA)
Objective: Capture hourly volatility for daily grid stability.

Data: 10+ years of high-frequency hourly load data.

Key Innovation: High-resolution peak demand tracking using Stacked LSTMs.

Horizon: Hourly / Daily.

2. Seasonal Climatic Tier (Spain Dataset)
Objective: Map energy consumption to climatic and seasonal cycles.

Data: 4 years of energy and temporal data from the Spanish grid.

Key Innovation: 48-hour sequence windowing to capture weather-driven cooling and heating shifts.

Horizon: Weekly / Monthly / Quarterly.

3. Long-Term Strategic Tier (Isuranga Dataset - Sri Lanka)
Objective: Forecast structural demand growth based on economic development.

Data: 5 years of load data integrated with GDP and Electricity Pricing.

Key Innovation: Socio-economic feature fusion to predict baseline shifts in developing economies.

Horizon: Yearly / Multi-year.

Tech Stack
Language: Python 3.x

Deep Learning: TensorFlow, Keras (LSTM, Dropout, Dense Layers)

Data Science: Scikit-learn (MinMaxScaler, Regressors), Pandas, NumPy

Visualization: Matplotlib, Seaborn

Key Results
The LSTM framework was benchmarked against Linear Regression, Random Forest, KNN, and Decision Trees. In all three tiers, the Deep Learning approach outperformed traditional regressors by effectively capturing the temporal dependencies and non-linearities in the data.
