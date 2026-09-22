# Phishing Website Detection with Explainable Machine Learning

Machine learning project for detecting phishing websites using behavioral features, ensemble learning, SHAP-based feature selection, ablation analysis, and cross-dataset evaluation.

## Tech Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/XGBoost-EB5B29?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/CatBoost-FFCC00?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/SHAP-5C4EE5?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
</p>

## Key Results

| Model | Features | F1-Score | AUC |
|---|---:|---:|---:|
| XGBoost | 81 | **0.9648** | **0.9945** |
| XGBoost (Pruned) | 20 | 0.9647 | 0.9930 |
| Stacking Ensemble | 20 | 0.9643 | 0.9932 |
| Random Forest (External Dataset) | 35 | **0.8207** | **0.9258** |

SHAP-based feature selection reduced the feature space from **81 to 20 features (75.3%)** while maintaining nearly the same predictive performance.

## Project Workflow

- Data preprocessing and feature preparation
- Logistic Regression and Decision Tree baselines
- Random Forest, XGBoost, and CatBoost
- Hyperparameter tuning
- SHAP explainability
- SHAP-based feature selection
- Stacking ensemble with Logistic Regression
- Feature ablation study
- Cross-dataset evaluation
- ROC curves and confusion matrices

## Repository Structure


phishing-website-detection-ml/
├── data/
│   └── README.md
├── notebook/
│   └── phishing_website_detection.ipynb
├── results/
│   ├── figures/
│   └── tables/
├── README.md
└── requirements.txt


## Dataset

### Primary Dataset

**Web Page Phishing Detection**
Hannousse & Yahiouche — Mendeley Data
DOI: `10.17632/c2gw7fy2j4.3`

- 11,430 website samples
- 81 processed behavioral features
- Legitimate and phishing website classes

### External Dataset

**Datasets for Phishing Websites Detection**
Vrbančič, Fister Jr. & Podgorelec — *Data in Brief*, 2020
DOI: `10.1016/j.dib.2020.106438`

Used for cross-dataset evaluation.

## SHAP Feature Analysis

Important features identified during the experiments included:

google_index
page_rank
web_traffic
nb_hyperlinks
nb_www


SHAP was used both for model interpretation and feature selection.

## Skills Demonstrated

`Machine Learning` • `Ensemble Learning` • `Explainable AI` • `SHAP` • `Feature Selection` • `Hyperparameter Tuning` • `Stacking` • `Ablation Analysis` • `Cross-Dataset Evaluation` • `Data Visualization`

```
The reported metrics and dataset details above are supported by your coursework report. 
```
