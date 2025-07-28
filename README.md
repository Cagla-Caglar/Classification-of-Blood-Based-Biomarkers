Blood Biomarker Classification Using Absorption Spectroscopy
This repository contains an independent machine learning project conducted by Çağla Çağlar. The study aims to classify three clinical biomarkers in blood samples—HDL cholesterol, LDL cholesterol, and hemoglobin—using spectral absorbance data.

The dataset consists of 13,140 samples with 170 absorbance values per sample, along with temperature and humidity measurements. Only the spectral data were used in the modeling process.

Initial data analysis included standardization, outlier examination using the IQR method, and dimensionality reduction with PCA. Logistic Regression was evaluated on PCA-reduced features but showed limited performance. XGBoost was trained directly on the full standardized spectra and achieved significantly better results.

Model performance was assessed using 10-fold cross-validation and tested on a held-out test set. SHAP analysis was applied to interpret model outputs and highlight the spectral regions most relevant to classification decisions.

The following test metrics summarize the final XGBoost results:

HDL cholesterol
ROC AUC: 0.9866
Accuracy: 0.9825

LDL cholesterol
ROC AUC: 0.9883
Accuracy: 0.9863

Hemoglobin
ROC AUC: 0.9868
Accuracy: 0.9897

This work was completed independently without external supervision or collaboration. All analysis, code, and documentation were prepared by Çağla Çağlar.
