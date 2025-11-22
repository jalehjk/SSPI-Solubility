Solubility Prediction (In Progress) — Machine Learning for Pharmaceutical R&D
This repository contains my ongoing solubility prediction project, part of my consulting work with Solid State Pharma.
The goal is to build a clean, reproducible ML pipeline that predicts aqueous solubility using molecular structures, featurization, and regression models.
This project is not finished yet.
The repository will evolve as I complete the modelling pipeline, notebooks, and Streamlit app.

🔧 Current Status: Under Active Development
Completed:
Project folder structure
Initial requirements setup
Placeholder directories for notebooks, models, and app interface

In progress:
Data cleaning + dataset preparation
RDKit featurization (fingerprints & descriptors)
Regression model training (RF, XGB, LightGBM)
Evaluation (RMSE, MAE, R²)
SHAP explainability
Streamlit UI for predictions

Next steps:
Add dataset (AqSolDB or ESOL)
Begin exploratory data analysis
Build featurization pipeline
Train and export models into /models
Finalize Streamlit app in /app/main.py

📂 Repository Structure
app/                # Streamlit app (to be developed)
data/               # Dataset (to be added)
models/             # Trained models (once ready)

📌 Notes
This is a work in progress, not a final model.
More files, notebooks, and code will be added soon.
This project supports my ongoing contract work in pharmaceutical ML.

🚧 Coming Soon
Molecular fingerprint generation
Solubility regression models
SHAP visualisation
Interactive solubility prediction UI

Contact
For collaboration or questions about this project, feel free to reach out.
notebooks/          # EDA, featurization, training notebooks
requirements.txt    # Project dependencies
README.md           # Project documentation
