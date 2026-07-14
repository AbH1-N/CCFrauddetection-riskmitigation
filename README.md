# Credit Card Fraud Detection & Risk Mitigation Engine

---

### Project Overview

This project tackles one of the most complex challenges in enterprise data analysis: detecting highly imbalanced, anomalous events (fraud) without blocking legitimate customer activity. Using a dataset of over 280,000 real-world credit card transactions, I developed a machine learning classification model to predict fraud probability and deployed the results into a high-level Business Intelligence dashboard for risk management teams.

All original data features were transformed using Principal Component Analysis (PCA) prior to modeling, ensuring strict consumer privacy and compliance with standard data governance frameworks (e.g., GDPR, ISO 31000).

---

### Tools & Technologies Used

| Tools | Use |
|--|--|
| **Python (Pandas, Scikit-Learn)** | Extracted, cleaned, and normalized data using StandardScaler |
| **Machine Learning** | Trained a Logistic Regression classification model. Implemented the class_weight='balanced' parameter to successfully penalize the algorithm for missing rare fraud cases within a highly imbalanced dataset (only 0.17% actual fraud) |
| **DAX** | Engineered logical risk-tier categories based on the model's exact probability outputs |
| **Power BI** | Designed an executive-level Risk & Compliance Command Center to visualize systemic threats |

---

### Key Business Insights

• Actionable Risk Tiers: Translated raw AI probability scores (0.0 to 1.0) into plain-English risk categories (Critical Risk, High Risk, Low Risk), allowing security teams to immediately prioritize manual reviews versus automated blocking.

• System Accuracy Validation: Visualized the model's performance by comparing actual fraud against AI predictions, proving the efficacy of the balanced machine learning approach.

• Anomaly Profiling: Mapped fraud risk levels against transaction sizes to identify behavioral correlations and systemic vulnerabilities.

---

### Repository Contents
| Contents | Description |
|---|---|
| **ccfraudproject.py** | The Python script detailing the data normalization, train/test splitting, and Logistic Regression model training |
| **fraud_preds4bi.zip** | The exported dataset containing the unseen test features and the model's calculated risk probability scores |
| **Fraudprediction.pbix** | The original Power BI dashboard file |
| **Dashboard** | A high-resolution export of the final interactive dashboard | 

---

| Dashboard |
|---|
| <img width="1326" height="743" alt="Screenshot 2026-02-25 160152" src="https://github.com/user-attachments/assets/3985da41-9aea-412b-8161-8fa550151b3d" /> |
