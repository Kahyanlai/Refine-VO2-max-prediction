# Refine-VO2-max-prediction

# VO₂ Max Prediction Using Wearable Activity Data

This project aims to predict VO₂ Max from wearable-derived activity data (running and cycling) by combining physiological, performance, and environmental features. The model focuses on both accuracy and explainability.

## Table of Contents
- [Dataset](#dataset)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)

## Dataset

Data sourced from simulated or real activity logs. Key features include:
- Heart rate (max/average)
- Distance, speed, cadence
- Elevation, terrain type
- Power, work, temperature

## Feature Engineering

We created several derived features such as:
- Pace (sec/km)
- Power-to-weight ratio
- Elevation gain per km
- Terrain type (flat, moderate, hilly)

We also removed highly correlated or redundant features using correlation matrix and VIF analysis.

## Modeling

Multiple regression models were trained:
- Linear Regression (Best: R² = 0.943)
- SVR
- Random Forest
- Gradient Boosting

The final model was selected based on R², RMSE, and interpretability.



