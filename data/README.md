```
# Data

This folder documents the datasets used in the phishing website detection project.

## Primary Dataset

**Dataset:** Web Page Phishing Detection  
**Authors:** Abdelhakim Hannousse and Salima Yahiouche  
**Source:** Mendeley Data  
**Version:** 3  
**DOI:** `10.17632/c2gw7fy2j4.3`

The dataset contains **11,430 website samples** with behavioral, URL, HTML, domain, and page-related features.

After preprocessing, **81 features** were used for model development.

### Usage

The primary dataset was used for:

- Data preprocessing
- Baseline model training
- Hyperparameter tuning
- XGBoost, CatBoost, and Random Forest evaluation
- SHAP feature analysis
- SHAP-based feature selection
- Stacking ensemble experiments
- Feature ablation studies

---

## External Validation Dataset

**Dataset:** Datasets for Phishing Websites Detection  
**Authors:** Grega Vrbančič, Iztok Fister Jr., and Vili Podgorelec  
**Publication:** Data in Brief, 2020  
**DOI:** `10.1016/j.dib.2020.106438`

This dataset was used as an independent dataset for **cross-dataset evaluation**.

The experiment used **88,647 samples**, with overlapping features aligned between the primary and external datasets before evaluation.

---

## Dataset Usage in the Project

| Dataset | Purpose |
|---|---|
| Web Page Phishing Detection | Training, testing, SHAP analysis, feature selection, stacking, and ablation |
| Datasets for Phishing Websites Detection | External cross-dataset validation |

---

## Important Note

The raw datasets are not included directly in this repository.

To reproduce the experiments:

1. Download the datasets from their original sources using the DOI links above.
2. Place the downloaded files inside this `data/` directory.
3. Update the dataset paths in the notebook if necessary.
4. Run the notebook from the preprocessing section onward.

Keeping the original datasets outside the repository helps keep the project lightweight while ensuring that the data is obtained from its official source.


```