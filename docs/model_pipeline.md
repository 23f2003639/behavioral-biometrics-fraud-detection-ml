# Model Pipeline

This document describes the machine learning pipeline used for behavioral biometrics–based fraud detection in digital payment systems.

---

## 1. Data Collection

The pipeline uses publicly available datasets to simulate real-world digital payment transactions and behavioral data.

---

## 2. Data Preprocessing

The raw datasets were preprocessed to ensure consistency and model readiness:
- Removal of irrelevant and identifier-based features.
- Handling missing values using appropriate imputation techniques.
- Encoding categorical variables.
- Scaling numerical features to ensure uniform feature contribution.

---

## 3. Feature Engineering

Relevant features were extracted to capture user behavior and transaction patterns, including:
- Transaction-based features such as amount, frequency, and timing.
- Behavioral features representing deviations from normal user activity.

Feature selection was performed to reduce noise and improve model performance.

---

## 4. Model Training

Two machine learning models were trained independently:

### XGBoost
- Used for supervised transaction-level fraud classification.
- Captures non-linear relationships between transaction features.
- Trained using labeled fraud and non-fraud samples.

### Isolation Forest
- Used for unsupervised behavioral anomaly detection.
- Identifies deviations from normal user behavior.
- Effective for detecting rare and unseen fraudulent patterns.

---

## 5. Inference and Decision Logic

Each model produces an independent fraud or anomaly score. The outputs are combined using rule-based decision logic to determine whether a transaction should be classified as legitimate or fraudulent.

---

## 6. Model Evaluation

Model performance was evaluated using:
- Confusion matrix
- Precision, recall, and F1-score
- ROC-AUC for classification effectiveness

The evaluation focused on minimizing false positives while maintaining high fraud detection accuracy.

---

## 7. Outcome

The pipeline demonstrates the effectiveness of combining supervised and unsupervised learning techniques for fraud detection using behavioral biometrics, providing an additional security layer for digital payment systems.
