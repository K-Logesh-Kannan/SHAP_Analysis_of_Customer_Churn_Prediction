# SHAP_Analysis_of_Customer_Churn_Prediction
**Interpretable Machine Learning:** SHAP-Driven Customer Churn Prediction
**Dataset:** Telco Customer Churn
**Model Used:** LightGBM
**Focus:** Predictive performance + Explainability using SHAP

**Project Overview:**
This project builds a churn prediction model using the Telco Customer Churn dataset, emphasizing model interpretability using SHAP (SHapley Additive exPlanations).
The goal is not just to reach strong predictive performance, but to justify predictions at both global and local levels and derive real business-ready retention strategies.

**Objectives:**
Data preprocessing & feature engineering
Train & tune a non-linear, high-performance model (LightGBM)
Evaluate using AUC, Accuracy & F1 Score
Explain predictions using SHAP global & local interpretation
Provide actionable business recommendations

**Tech Stack:**
| Component          | Tools Used      |
| ------------------ | --------------- |
| Language           | Python          |
| Data Preprocessing | Pandas, NumPy   |
| Modeling           | LightGBM        |
| Explainability     | SHAP            |
| Evaluation         | sklearn metrics |
| Model Persistence  | pickle (.pkl)   |

**Data Preprocessing Summary:**
✔ Handled missing values
✔ Converted categorical variables using One-Hot Encoding
✔ Engineered customer behavior features
✔ Balanced dataset to avoid class bias

**Model Performance:**
| Metric            | Result                        | Notes                             |
| ----------------- | ----------------------------- | --------------------------------- |
| **AUC**           | **0.7965**                    | Good classification separation    |
| **Best Accuracy** | **0.7850** (Threshold = 0.90) | Strong precision-oriented cut-off |
| **Best F1 Score** | **0.5859** (Threshold = 0.01) | Best balanced performance         |

**Saved Models & Artifacts:**
| File                                   | Description                     |
| -------------------------------------- | ------------------------------- |
| `model_lightgbm_optimized.pkl`         | Serialized model for deployment |
| `SHAP_Telco_Optimized.ipynb`           | Full reproducible notebook      |
| `Telco_Churn_Project_Optimized.zip`    | Consolidated project            |
| `WA_Fn-UseC_-Telco-Customer-Churn.csv` | Dataset                         |

**Business-First Narrative:**
Customer churn is one of the most critical business challenges for subscription-based industries, where retaining existing customers is often more cost-effective than acquiring new ones. To support data-driven retention strategies, this project builds a high-performing churn prediction model using the Telco Customer dataset and applies advanced explainable AI techniques to convert predictions into actionable business insights.

The data was rigorously preprocessed, engineered, and modeled using a Gradient Boosting-based algorithm (LightGBM) to maximize predictive accuracy and ranking capability in real-world scenarios. Multiple thresholds and metrics were evaluated, and AUC was prioritized over accuracy to ensure that the model performs reliably across varying decision boundaries. The final LightGBM model achieved an AUC score of 0.7965, with best threshold-based accuracy of 0.7850 and best F1 score of 0.5859, demonstrating strong model performance and balanced prediction capability.

To unlock interpretability, SHAP (SHapley Additive exPlanations) was implemented at both global and local levels. Global SHAP results identified MonthlyCharges, TotalCharges, tenure, and customer engagement-based features as key drivers influencing churn behavior. Local SHAP force plots were further generated for high-risk, low-risk, and borderline customers, enabling precise understanding of individual churn triggers that can directly inform retention decisions such as loyalty offers, billing adjustments, personalized support, or service upgrades.

The model artifacts, SHAP visualizations, and optimized feature importance were exported and saved for reproducibility, including a pickle (.pkl) model file. Combined, this work transforms machine learning output into clear and strategic business value that can help organizations proactively reduce churn, strengthen long-term customer relationships, and improve profitability.


**Conclusion:**
This project successfully developed a robust churn prediction framework using LightGBM, paired with SHAP-based explainability, enabling both accurate forecasting and clear interpretation of churn drivers. Key behavioral and billing-related features were identified as major influencers, providing practical insights into customer risk segments. Beyond prediction, this solution empowers businesses to design targeted retention strategies such as personalized engagement, pricing optimization, and proactive service support. Overall, the project demonstrates how combining machine learning performance with transparent explainability can drive informed decisions, minimize churn, and strengthen customer lifetime value.
