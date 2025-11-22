Solubility Prediction — Machine Learning for Drug Development
This project predicts aqueous solubility of chemical compounds using machine learning.
It mirrors the type of early-stage formulation modelling done in pharmaceutical R&D, including the workflow I use for my consulting work with Solid State Pharma.
The pipeline covers:
Data cleaning and standardisation
Molecular featurization (RDKit fingerprints)
Regression models (Random Forest, XGBoost, LightGBM)
SHAP explainability
A Streamlit interface for quick solubility predictions
The goal is a clean, practical ML workflow for solubility estimation — useful for screening, prioritisation, and drug design support.

🔍 What this project does
Reads molecular structures (SMILES) or descriptors
Generates fingerprint vectors using RDKit
Trains regression models to predict solubility (logS)
Evaluates models with RMSE, MAE, and R²
Explains predictions using SHAP
Provides a simple Streamlit UI for demo usage
This is a compact, research-friendly version of a typical property prediction pipeline used in computational chemistry.

📂 Project structure
app/
    main.py                 # Streamlit interface for predictions

data/
    AqSolDB.csv             # public solubility dataset (or placeholder)

models/
    solubility_model.pkl    # trained regression model
    feature_info.pkl        # fingerprint metadata / descriptor list

notebooks/
    01_eda.ipynb
    02_featurization.ipynb
    03_model_training.ipynb
    04_shap_analysis.ipynb

▶️ How to run
Install dependencies:

pip install -r requirements.txt

Launch the Streamlit demo:

streamlit run app/main.py

You’ll get a small app where you input a SMILES string and see:
Predicted solubility
Top SHAP contributors
Fingerprint-based explanation

🧪 Models included
This repo includes multiple models for comparison:
Random Forest Regressor
XGBoost Regressor
LightGBM Regressor
Gradient Boosting
Baseline Linear Regression
Performance is reported using:
RMSE
MAE
R² score
Models are trained using both molecular fingerprints and numeric descriptors.

🧠 Explainability (SHAP)
SHAP analysis is provided to:
reveal molecular fragments that raise or lower solubility
allow chemists to interpret model behaviour
connect predictions to underlying chemical structure
Explainable AI is important in chemistry because black-box predictions are rarely accepted without justification.

🚀 Future improvements
Include graph neural networks (GNN-based property prediction)
Integrate Mordred descriptors
Add Optuna hyperparameter optimisation
Create a full docking-like batch prediction tool
Deploy the Streamlit demo online

📘 Summary
This repo demonstrates a realistic solubility prediction pipeline used in pharmaceutical data science:
✔️ molecular featurization
✔️ regression modelling
✔️ explainability
✔️ Streamlit interface
✔️ reproducible notebooks
It’s clean, simple, and easy to extend into a more advanced chemoinformatics workflow.

requirements.txt
README.md
