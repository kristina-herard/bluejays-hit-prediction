# bluejays-hit-prediction
Predicting Toronto Blue Jays base hits using launch speed, launch angle, release speed, and pitch type with logistic regression.

# MLB Base Hit Prediction Using Pitch & Contact Data

## Project Overview

This project analyzes MLB pitch-level and batted-ball data to predict whether a plate appearance results in a **base hit**. Using statistical modeling techniques, the goal was to determine which variables most strongly influence hit probability.

Predictors examined:
- Launch Speed (Exit Velocity)
- Launch Angle
- Pitch Type
- Pitch Release Speed

The analysis applies logistic regression, model selection techniques, and nonlinear transformations to improve predictive performance.

---

## Objectives

- Explore relationships between pitch characteristics and hit outcomes  
- Identify statistically significant predictors of base hits  
- Compare multiple logistic regression models  
- Improve model fit using transformations  
- Evaluate predictive performance using classification metrics  

---

## Methods

- Exploratory Data Analysis (EDA)
- Logistic Regression (GLM with binomial family)
- AIC and BIC model selection
- ANOVA model comparison
- Nonlinear polynomial terms
- Multicollinearity assessment (VIF)
- Confusion matrix evaluation
- Precision, Recall, and F1 Score analysis

All analysis was conducted in **R**.

---

## Key Findings

- **Launch speed** and **launch angle** were the strongest predictors of base hits.
- Pitch type and pitch release speed were not statistically significant after accounting for contact quality.
- Incorporating nonlinear terms significantly improved model performance.
- Final model accuracy: **~73%**
- Model performance reflects the inherent difficulty of predicting hits in baseball.

These findings align with baseball intuition: harder contact at optimal launch angles increases hit probability.

---

## Model Performance

- Accuracy: 73%
- Sensitivity (Recall): 66%
- Precision: 41%
- F1 Score: 0.51

The model identifies a majority of true hits but produces false positives — consistent with the rarity and unpredictability of hits in baseball.

---

## Full Report

[View Full Technical Report (PDF)](markdown.pdf)

---

## How to Run

1. Clone this repository
2. Open the project in RStudio
3. Run the analysis scripts
4. Review model outputs and visualizations

---

## Author

Kristina Herard  
Statistics & Sports Analytics  
Aspiring MLB Statistician | Canada 🇨🇦
