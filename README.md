# 🏀 NCAA March Madness Bracket Outcome Prediction

## Overview
This project, developed as part of a case competition at Purdue University's Daniels School of Business, focuses on predicting the outcomes of the final two rounds of the NCAA March Madness tournament. The goal was twofold: build a highly accurate ensemble model for national championship forecasting and analyze how school affinity (e.g., loyalty and location) influences bracket submission behavior.

Our team used XGBoost models for three perspectives—team performance, geographic proximity, and institutional scale—and combined them through ensemble voting techniques. The final model achieved strong predictive accuracy and placed 5th out of 87 teams.

Additionally, we created an interactive Tableau dashboard to visualize trends in school size, submission behavior, and win probability by region.

## Tech Stack
- Python: XGBoost, Optuna, scikit-learn, Pandas, NumPy
- Tableau: Data visualization for submission patterns and team affinity
- Feature Engineering: DMA region matching, weighted win scores, tenure scaling

## Modeling Highlights
- Built three separate XGBoost models focusing on:
  - **Performance**: Win %, average score, tenure
  - **Geography**: DMA region match, lat/long
  - **Institutional Scale**: Enrollment, attendance
- Hyperparameter tuning using **Optuna** and **RandomizedSearchCV**
- Voting ensemble: Weighted Hard Voting (Geo: 3, Perf: 2, Scale: 1)
- Accuracy:
  - National Champion: 0.462
  - Semifinal (East/West): 0.692
  - Semifinal (South/Midwest): 0.641

## Key Insights
- Larger institutions drive significantly higher bracket engagement.
- Team performance is the dominant driver of bracket picks.
- Local affiliation plays a stronger role in states with top-performing programs (e.g., UConn in Connecticut).
- School size alone doesn't ensure success, but influences visibility and participation.

## Repository Contents
- `model/`: Python scripts for each XGBoost model and ensemble voting logic
- `dashboard/`: Tableau screenshots and insights
- `README.md`: Project overview

## Visual Preview
_TODO: Add Tableau screenshots or model output images here_

---

**Developed by:**  
Tzu-Yun (Daisy) Huang, Leanna Jeon, Yi Shiuan Chiang, Shih Min Lin  
📍 Purdue University, Daniels School of Business
🎖️ **Competition Result:** 5th out of 87 teams  
📅 **Date:** Feb – Mar 2025


