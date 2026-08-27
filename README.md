# Club Football Match Data: Analysis and Modelling

Exploratory analysis, statistical testing, and predictive modelling on 25 seasons (2000–2025) of Premier League match data, using Arsenal as a case study before extending to home advantage and match outcome prediction across the league.

View the original notebook on Kaggle: [Club Football Match Data: Analysis and Modelling](https://www.kaggle.com/code/samueldalbyquenet/final-version-atm)

## Contents
- Data cleaning and validation (team name standardisation, missing data checks)
- Exploratory analysis of Arsenal's season-by-season performance
- League-wide home advantage analysis (top 6 and all clubs)
- Correlation and chi-square significance testing
- Match outcome prediction using logistic regression and random forest

## Data

This notebook uses the [Club Football Match Data (2000–2025)](https://www.kaggle.com/datasets/adamgbor/club-football-match-data-2000-2025) dataset by Adam Gbor, available on Kaggle.

To run this notebook yourself:
1. Download `Matches.csv` and `EloRatings.csv` from the Kaggle dataset page above.
2. Update the file paths in the notebook's data-loading cell to point to wherever you've saved the files locally (the original paths assume a Kaggle notebook environment, e.g. `/kaggle/input/...`).

## Key findings
- Goal difference is the strongest single predictor of Arsenal's final points tally (r = 0.839)
- Home advantage is statistically significant league-wide (χ² = 329.21, p < 0.001), not confined to top clubs
- A random forest model using Elo rating and form differentials achieves 64.72% accuracy predicting home wins, versus a 45.38% naive baseline

## Requirements
pandas, numpy, matplotlib, scipy, scikit-learn
