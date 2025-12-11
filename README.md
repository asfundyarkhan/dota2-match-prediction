# +++++ Dota 2 Match Outcome Prediction using Gradient Boosting ++++

This repository contains the full code, tutorial, and explainability analysis for predicting Dota 2 match outcomes using XGBoost (gradient boosting). The project demonstrates:

Why gradient boosting is effective for esports analytics

How early-game features influence match results

How to interpret model predictions using Feature Importance and SHAP values

Ethical considerations of predictive analytics in competitive gaming

This repository serves as both an educational tutorial and a reproducible machine-learning workflow for esports analysts, students, and researchers.

++++ Repository Structure ++++
dota2-match-prediction/
│
├── README.md                → Project overview
├── LICENSE                  → MIT License
│
├── notebooks/
│   └── dota2_xgboost_prediction.ipynb
│
├── tutorial/
│   └── tutorial.pdf         → <2000-word tutorial for assignment
│
└── images/                  → Plots used in tutorial
    ├── feature_importance.png
    ├── shap_summary.png
    └── confusion_matrix.png

# ++++ Dataset +++++

We use the Dota 2: Predicting Match Outcome dataset from Kaggle:

# ++++ https://www.kaggle.com/competitions/dota-2-prediction/data +++++

This includes early-game match statistics and the target variable radiant_win.

# ++++ Machine Learning Model ++++

We use XGBoost, a gradient-boosting method known for:

High performance on structured/tabular data

Ability to model non-linear interactions

Built-in handling of missing values

Strong interpretability through SHAP and feature importance

The notebook includes:

Data loading & preprocessing

Training/validation split

Feature imputation

Model training

Evaluation metrics (accuracy, AUC, confusion matrix)

Explainability analysis

# +++ Explainability Tools ++++
Feature Importance

Shows which variables most affected predictions (e.g., gold advantage, tower status).

SHAP Values

Provides both global and local explanations:

Global → overall behaviour of the model

Local → why a specific match was predicted as a Radiant win or loss

This is essential for ethical, transparent AI in esports analytics.

# ++++ Ethical Considerations ++++

The tutorial discusses the impact of ML in esports, including:

Competitive imbalance

Gambling risks

Data bias

Transparency in analytical tools

# ++++ How to Run the Notebook ++++

Open in Google Colab:

Upload your Kaggle API token to Colab

Download dataset using:

!kaggle competitions download -c dota-2-prediction
!unzip *.zip


Run the notebook end-to-end.

#  ++++ License ++++

This project uses the MIT License, allowing academic and commercial use.
