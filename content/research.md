---
title: "Research Focus"
description: "Key research initiatives, methodologies, and clinical screening frameworks."
---

## Core Research Topic

### Machine Learning-Based Multiclass Prediction of Postpartum Mental Health Conditions

Postpartum mental health screening remains a critical area in clinical decision-support systems. This research investigates robust supervised machine learning models to classify maternal health data into distinct screening categories:

1. **Normal**
2. **Baby Blues**
3. **Anxiety**
4. **Postpartum Depression**

> **Academic Note:** This research presents an analytical screening and decision-support tool meant to assist clinical data interpretation. It is not intended to diagnose patients directly.

---

## Technical Methodology & Models

To handle class imbalances and complex feature interactions in tabular maternal health data, the evaluation framework compares multiple baseline and ensemble models:

- **K-Nearest Neighbors (KNN)**
- **Support Vector Machines (SVM)**
- **Random Forest Classifier**
- **XGBoost (Extreme Gradient Boosting)**
- **Stacking Ensemble Architecture**

### Stacking Ensemble Pipeline

The proposed architecture utilizes a heterogenous stacking mechanism to combine complementary meta-learners:

Base Learners: Random Forest + XGBoost --> Meta-Learner: Logistic Regression --> Final Prediction

- **Base Layer:** Combines Random Forest (bagging) and XGBoost (boosting) to capture non-linear patterns and complex relationships.
- **Meta-Layer:** Uses Logistic Regression to weigh the probabilistic outputs of base learners and generate refined multiclass predictions.
