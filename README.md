# NBA Final Score Prediction with LSTM

Predicting NBA final scores from the first 3 quarters using a 
sequential LSTM model trained on real 2023-24 season data.

## Results
- Dataset: 400 real NBA games (2023-24 regular season)
- Model: 2-layer LSTM (64 → 32 units)
- MAE: ~5.1 points on final score prediction

## How it works
Given Q1, Q2, Q3 points scored by a team → predict the final score.

Input shape: (400, 3, 1) — 400 games, 3 timesteps, 1 feature
Target: final score (regression)

## Stack
- Python, TensorFlow/Keras, nba_api, scikit-learn, pandas

## Run it
Open the notebook in Google Colab and run all cells.
Data is already included in nba_quarters_2324.csv.
```

---

### .gitignore
```
__pycache__/
*.pyc
.ipynb_checkpoints/
nba_games_2324.csv
