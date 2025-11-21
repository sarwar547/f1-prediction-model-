# f1-prediction-model-
A full Formula 1 analytics system using data from 1950–2024 to predict 2025 results. It preprocesses race data, builds driver/team metrics, forecasts winners with RF/XGBoost, clusters performance tiers, detects anomalies, predicts lap times, and creates pro visualizations for insights.
🏎️ F1 Performance Analytics & Race Outcome Prediction System

A complete end-to-end data science project that analyzes historical Formula 1 performance and predicts future race outcomes using machine learning. This project integrates data engineering, feature engineering, supervised & unsupervised ML, anomaly detection, and advanced visualizations.

🚀 Project Overview

This system processes Formula 1 data (1950–2024) to produce driver/team insights and forecast 2025 season behavior. The workflow covers:

Loading & cleaning historical F1 datasets

Standardizing driver/constructor names and race formats

Feature engineering for performance metrics

Training ML models for winner prediction

Clustering drivers into tiers

Detecting anomalous performances

Predicting expected lap times using regression

Creating high-quality visual analytics

The goal is to deliver a complete F1 analytics toolkit—both predictive and explanatory.

📂 Features Included
1️⃣ Data Engineering

Combined race results, qualifying, constructor standings, and lap times

Fixed naming inconsistencies across seasons

Engineered advanced features:

Driver consistency, racecraft, qualifying strength

Team dominance & reliability

Track-specific tendencies

Pace deviation & pit-stop stability

2️⃣ Performance Metrics

Driver points, podium patterns, finishing consistency

Team pace progression

Overtake & racecraft metrics

Season-long performance trends

Correlation and sector/lap timing analysis

3️⃣ Machine Learning Models
Winner Prediction

RandomForestClassifier

XGBClassifier

Lap Time Prediction

RandomForestRegressor

XGBRegressor

Methods Used:

Time-series cross-validation

Robust scaling

Feature selection

Hyperparameter search

4️⃣ Unsupervised Learning

K-Means clustering for driver tiers

DBSCAN for grouping unusual patterns

PCA for dimensionality reduction and visualization

5️⃣ Anomaly Detection

Isolation Forest detects:

Exceptional qualifying laps

Sudden performance drops

Overperformance vs expected pace

6️⃣ Visualizations

Generates clean, professional charts:

Heatmaps

Scatter plots

Bubble plots

Radar charts

Team/driver progression charts

Correlation matrices

🧠 Tech Stack

Languages: Python
Libraries:
pandas, numpy, matplotlib,
scikit-learn, xgboost,
RandomForest, DBSCAN, PCA,
joblib, scipy

📁 Project Structure
/data                   → CSV datasets
/models                 → Saved ML models (joblib)
/notebooks              → Development notebooks
/visuals                → Exported plots
src/
   preprocessing.py
   feature_engineering.py
   model_training.py
   clustering.py
   anomaly_detection.py
   visualization.py
   predict.py
README.md

▶️ How to Run

Install dependencies:

pip install pandas numpy matplotlib scikit-learn xgboost scipy joblib


Place datasets in a /data/ folder.

Run the notebook or execute the scripts:

python src/model_training.py


View predictions, clusters, and analytics in the output folders.

📌 Outputs Generated

Driver & team performance tables

2025 race winner probability forecasts

Lap-time predictions per track

Driver-tier clusters

Anomaly detection logs

Professional-grade visual charts
