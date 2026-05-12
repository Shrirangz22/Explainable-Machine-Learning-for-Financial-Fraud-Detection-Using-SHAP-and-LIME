# Explainable-Machine-Learning-for-Financial-Fraud-Detection-Using-SHAP-and-LIME
The project compares three models:

- Logistic Regression
- Random Forest
- Artificial Neural Network (ANN)

It then explains model decisions using:

- SHAP (global + local explainability)
- LIME (transaction-level local explainability)

## Objectives
- Build a reproducible fraud detection pipeline for imbalanced data
- Compare LR, RF, and ANN using fraud-focused metrics
- Generate interpretable explanations for model predictions
- Demonstrate how explainability supports trust and auditability

## Dataset
- Source: ULB/Kaggle Credit Card Fraud Detection Dataset
- Records: 284,807
- Fraud cases: 492 (~0.17%)
- Features: `V1`–`V28` (PCA-anonymized), `Time`, `Amount`
- Target: `Class` (0 = non-fraud, 1 = fraud)

> Note: Dataset file is not included in this repo by default. Place `creditcard.csv` in the expected data folder. Uploaded the csv file link (https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## Repository Structure
```text
.
├── data/
│   └── creditcard.csv                  # add locally
├── notebooks/
│   ├── final_fraud_xai_pipeline_dissertation.ipynb
│   └── ...
├── outputs/
│   ├── final_notebook_artifacts/
│   │   ├── metrics/
│   │   └── plots/
│   └── ...
├── reports/
│   ├── draft_dissertation.docx
│   └── fraud_xai_10min_presentation.pptx
├── requirements.txt
└── README.md
