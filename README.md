# 🎮 League of Legends Win Prediction

**Author:** Justin Mundell  

---

## Overview
This project analyzes high-ranked League of Legends matches to predict the probability of a team winning based on in-game metrics from the first 10 minutes. Multiple machine learning models were applied to evaluate predictive performance and identify key factors influencing match outcomes. 

---

## Objectives
- Predict match outcomes using early-game features  
- Identify the most important variables affecting win probability  
- Compare performance across multiple machine learning models  

---

## Dataset
- ~10,000 ranked games (Diamond–Master tier)  
- Sourced from Riot Games API via Kaggle  
- Includes gameplay metrics such as:
  - gold difference  
  - experience difference  
  - kills, assists, objectives  
  - vision (wards) 

---

## Methods
- Logistic Regression  
- Stepwise Feature Selection  
- Cross-Validation:
  - LOOCV  
  - K-Fold CV  
- Decision Trees  
- Bagging  
- Random Forest  
- Boosting  

---

## Results

- Logistic Regression (K-Fold CV) performed best:
  - **~17% test error (~83% accuracy)** :contentReference[oaicite:2]{index=2}  
- Tree-based models showed higher error rates (~27–28%)  
- Ensemble methods improved stability but not significantly over trees  

---

## Key Insights

- **Gold difference** is the most important predictor across all models  
- **Experience difference and dragons** also strongly impact outcomes  
- Early-game metrics can predict match results with reasonable accuracy  
- Tree-based methods were easier to interpret but less accurate than logistic regression  

---

## Files
- `Math 4322 Project.pdf` – Full analysis and code  

---

## Notes
Model performance was limited by the complexity of the game and missing contextual features (e.g., champion selection, late-game dynamics), which may improve predictions in future work.
