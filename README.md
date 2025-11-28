# loan-predictor-basic-ai
A minimal AIML pipeline for binary loan-approval prediction using a Kaggle dataset. Includes a trained model, a sample prediction CLI, dataset for local testing, and instructions to run the project locally. Designed for learning and local experimentation (not production/deployed).
# loan-approval-predictor

**Minimal AIML model for loan approval prediction**  
This repository contains a compact pipeline for predicting whether a loan application will be approved. It is intended for local experimentation and learning using a Kaggle-derived dataset.

> ⚠️ This project is for educational/local use only. The model is not production hardened nor deployed.

## Repo contents
- `data/loan_data.csv` — Example dataset used for testing and demonstration. :contentReference[oaicite:3]{index=3}  
- `model/loan_model.pkl` — Trained model and metadata saved with joblib. The pickle holds at least two keys: `model` (the estimator) and `columns` (expected feature columns). :contentReference[oaicite:4]{index=4}  
- `src/predict_W_model.py` — CLI prediction script that loads the model, reads the CSV, builds a single-row input, performs preprocessing (fills missing values, gets dummies, inserts missing columns) and prints the prediction + probabilities. This is the script you supplied (slightly annotated below). :contentReference[oaicite:5]{index=5}

## Quickstart (local)
1. Clone the repo:
   ```bash
   git clone https://github.com/<bhaveshsagathiya03-tech>/loan-approval-predictor.git
   cd loan-approval-predictor
