# Master Thesis Data Science
# Burnout Prediction Among Medical Students

This repository contains 4 experiments focused on predicting **burnout** and **burnout severity** among medical students using a publicly available dataset from **Carrard et al. (2022)**.

## Project Overview

The goal of this project was twofold:
1. **Classify** students as experiencing burnout or not (binary classification).
2. **Predict burnout severity** using the continuous **MBI total score** (regression).

Each experiment included model training, evaluation, and error analysis. Feature importance was additionally conducted for top-performing models.

---

## Experiments

### **Experiment 1: Binary Burnout Classification (Imbalanced Dataset)**
- **Goal**: Classify students into burnout vs. no burnout
- **Dataset**: imbalanced
- **Models**: 
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - Support Vector Machine (SVM)
  - XGBoost
  - TabNet
- **Notes**:
  - XGBoost was the best-performing model.
  - Feature importance was analyzed using the trained XGBoost model.

---

### **Experiment 2: Binary Burnout Classification (SMOTE-ENN Oversampling)**
- **Goal**: Improve classification under class imbalance
- **Technique**: Applied SMOTE-ENN during training
- **Models**: Same as Experiment 1


---

### **Experiment 3: Binary Burnout Classification (Borderline-SMOTE Oversampling)**
- **Goal**: Explore an alternative oversampling method
- **Technique**: Borderline-SMOTE
- **Models**: Same as above


---

### **Experiment 4: Predicting Burnout Severity (Regression)**
- **Goal**: Predict continuous **MBI total score**
- **Models**:
  - Decision Tree Regressor
  - Random Forest Regressor
  - SVR (Support Vector Regressor)
  - XGBoost Regressor
  - TabNet Regressor
- **Notes**:
  - SVR showed the best performance.
  - Feature importance was conducted on the trained SVR model.
  - Residual analysis and error distribution were evaluated for all models.

---

## Evaluation Metrics

- **Classification**: AUC, F1 Score, Precision, Recall, PR-AUC
- **Regression**: R², MAE, RMSE, Residual Plots
- **Error Analysis**: Included for all models in each experiment

---

## Contents

- `data/`: Original and preprocessed dataset
- `notebooks/`: Google Colab notebooks
- `results/`: Metrics, plots, and residual analysis
- `models/`: Saved model files and feature importance outputs

---

## Acknowledgments

- Dataset: Carrard, V., et al. (2022). [Carrard, V., Bourquin, C., Berney, S., Schlegel, K., Gaume, J., Bart, P., Preisig, M., Mast, M. S., & Berney, A. (2022a). Dataset for the paper “The relationship between medical students’ empathy, mental health, and burnout: A cross-sectional study” published in Medical Teacher (2022) [Dataset]. In Zenodo (CERN European Organization for Nuclear Research). https://doi.org/10.5281/zenodo.5702895

]
- Project developed as part of the Master's program in **Data Science and Society** at **Tilburg University**.

---

