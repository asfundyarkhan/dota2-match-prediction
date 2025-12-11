# Dota 2 Match Outcome Prediction using Gradient Boosting

This repository contains the full code, tutorial, and explainability analysis for predicting Dota 2 match outcomes using XGBoost (gradient boosting). The project demonstrates:

Why gradient boosting is effective for esports analytics

How early-game features influence match results

How to interpret model predictions using Feature Importance and SHAP values

Ethical considerations of predictive analytics in competitive gaming

This repository serves as both an educational tutorial and a reproducible machine-learning workflow for esports analysts, students, and researchers.

# Repository Structure

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

#  Dataset

We use the Dota 2: Predicting Match Outcome dataset from Kaggle:

#  https://www.kaggle.com/competitions/dota-2-prediction/data

This includes early-game match statistics and the target variable radiant_win.

#  Machine Learning Model 

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

#  Explainability Tools
Feature Importance

Shows which variables most affected predictions (e.g., gold advantage, tower status).

SHAP Values

Provides both global and local explanations:

Global → overall behaviour of the model

Local → why a specific match was predicted as a Radiant win or loss

This is essential for ethical, transparent AI in esports analytics.

#  Ethical Considerations

The tutorial discusses the impact of ML in esports, including:

Competitive imbalance

Gambling risks

Data bias

Transparency in analytical tools

# How to Run the Notebook

Open in Google Colab:

Upload your Kaggle API token to Colab

Download dataset using:

!kaggle competitions download -c dota-2-prediction
!unzip *.zip


Run the notebook end-to-end.

#  License

This project uses the MIT License, allowing academic and commercial use.

# References

Chen, T. and Guestrin, C., 2016. XGBoost: A scalable tree boosting system. Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, pp.785–794.

Friedman, J.H., 2001. Greedy function approximation: A gradient boosting machine. Annals of Statistics, 29(5), pp.1189–1232.

Holmgård, C. et al., 2014. Evolving personas for player decision modeling. IEEE Conference on Computational Intelligence and Games, pp.1–8.

Kaggle, 2015. Dota 2: Predicting Match Outcome Dataset. Available at: https://www.kaggle.com/competitions/dota-2-prediction/data
 (Accessed: <insert date>).

Kalyan, Y. and Sangeetha, S., 2015. Predicting the outcome of Dota 2 matches using machine learning algorithms. International Journal of Applied Engineering Research, 10(17), pp.13131–13140.

Lundberg, S.M. and Lee, S.I., 2017. A unified approach to interpreting model predictions. Advances in Neural Information Processing Systems, pp.4765–4774.

Lundberg, S.M. et al., 2018. Explainable machine-learning predictions for the prevention of hypoxaemia during surgery. Nature Biomedical Engineering, 2(10), pp.749–760.

Pobiedina, N. et al., 2013. Role-based performance similarities in Dota 2. Procedia Computer Science, 22, pp.59–68.

Ravari, Y.N. and Moser, A., 2022. Predicting outcomes in MOBA games using machine learning: A case study of Dota 2. Journal of Computer Science and Technology, 37(3), pp.543–556.

Sapienza, A., Peng, H. and Ferrara, E., 2018. Performance prediction in MOBA games. IEEE Transactions on Games, 11(3), pp.239–251.

Yang, D., Harrison, B. and Roberts, D.L., 2014. Identifying patterns in MOBA gameplay: A data-driven approach. IEEE Conference on Computational Intelligence and Games, pp.1–8.

Zhou, Z.H., 2012. Ensemble Methods: Foundations and Algorithms. Boca Raton: CRC Press.
