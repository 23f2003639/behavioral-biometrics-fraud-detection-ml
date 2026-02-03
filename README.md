# Behavioral Biometrics-Based Fraud Detection for Digital Payments

This repository contains my machine learning contributions to a research project focused on fraud detection in digital payment systems using behavioral biometrics.

The project explores both supervised and unsupervised machine learning approaches to detect fraudulent behavior based on user interaction patterns.

---

## Models Implemented

### 1. XGBoost Fraud Detection
- Supervised learning model trained on transaction-level data.
- Used to classify transactions as fraudulent or non-fraudulent.
- Evaluated using classification report, ROC–AUC score, and confusion matrix.

### 2. Isolation Forest Behavioral Anomaly Detection
- Unsupervised anomaly detection model.
- Trained on behavioral biometric features such as keystroke and interaction patterns.
- Anomalies are mapped to potential fraud cases.
- Evaluated using confusion matrix, ROC–AUC, and anomaly score analysis.

---

## Repository Structure

- `notebooks/` – Jupyter/Colab notebooks containing model implementation.
- `data/` – Dataset used for experimentation.
- `docs/` – Documentation of model pipeline and methodology.

---

## Research Context

This work is part of an academic research project titled:

**A Multi-Layered Security Framework for Digital Payments: Behavioral Biometrics-Based Fraud Detection Using Machine Learning**

The paper is currently unpublished.  
This repository documents my individual contributions to the machine learning components of the project.

---

## Tools & Technologies
- Python
- pandas, NumPy
- scikit-learn
- XGBoost
- Matplotlib, Seaborn
