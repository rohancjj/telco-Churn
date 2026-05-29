Telecom Customer Churn Prediction & GenAI Retention Copilot
📌 Project Overview

This project is an end-to-end Machine Learning + Analytics + GenAI solution designed to predict telecom customer churn and generate AI-powered retention recommendations.

The system identifies customers likely to leave the telecom service using an XGBoost classification model, handles class imbalance using advanced techniques, explains predictions using SHAP Explainable AI, and integrates a Generative AI assistant to provide business-friendly churn explanations and retention strategies.

🚀 Business Problem

Customer churn is one of the biggest revenue challenges in the telecom industry.

Acquiring new customers is significantly more expensive than retaining existing ones. Telecom companies need proactive systems that can:

Detect customers at risk of leaving
Understand the reasons behind churn
Help retention teams take action before customers leave

This project solves that problem using Data Analytics, Machine Learning, Explainable AI, and Generative AI.

🎯 Project Goals
Predict whether a customer will churn
Improve churn recall using imbalance handling
Identify important churn-driving factors
Generate natural-language retention recommendations using GenAI
Create business dashboards for churn analysis
🛠️ Tech Stack
Category	Tools
Programming	Python
Data Processing	Pandas, NumPy
Visualization	Matplotlib, Seaborn
Machine Learning	XGBoost, Scikit-learn
Explainable AI	SHAP
Dashboarding	Power BI
GenAI	Mistral / Gemini API
Notebook Environment	Jupyter Notebook



📊 Dataset

Dataset: Telecom Customer Churn Dataset

Features include:

Customer demographics
Contract information
Internet services
Monthly charges
Payment methods
Customer tenure
Churn label

Target Variable:

Churn
0 = Customer stays
1 = Customer leaves
🧹 Data Preprocessing

Performed the following preprocessing steps:

Handled missing values
Converted TotalCharges to numeric
Binary encoding for Yes/No columns
One-hot encoding for categorical features
Feature engineering
Removed data inconsistencies
⚙️ Feature Engineering

Created additional business-focused features:

AvgSpend
AvgSpend = TotalCharges / (tenure + 1)
Tenure Groups

Customers segmented by subscription duration.

TotalServices

Combined service adoption count for engagement analysis.

🤖 Machine Learning Model

Model Used:

XGBoost Classifier

Techniques applied:

Train-test split
Class imbalance handling using scale_pos_weight
Threshold tuning
Feature importance analysis
📈 Model Performance
Initial Model
Recall (Churn): 48%
Improved Model

After imbalance handling and threshold tuning:

Recall (Churn): 77%
Accuracy: 70%
Why Recall Matters

In churn prediction, missing churn customers is more expensive than generating some false alarms.

The model was optimized for higher churn detection instead of raw accuracy.

🔍 Explainable AI with SHAP

SHAP was used to explain model predictions and identify the most important churn-driving features.

Top churn factors included:

Fiber optic internet
Short tenure
Month-to-month contracts
High monthly charges

SHAP enables transparent and interpretable AI predictions.

🧠 GenAI Retention Copilot

Integrated a Generative AI layer using Mistral/Gemini APIs.

The GenAI assistant:

Explains why a customer may churn
Generates retention recommendations
Converts ML outputs into business-friendly insights
Example Output
Customer is at high churn risk due to short tenure,
high monthly charges, and lack of contract commitment.

Recommended actions:
- Offer discounted annual plan
- Provide loyalty incentives
- Offer technical support bundle
📊 Power BI Dashboard

Dashboard includes:

Churn overview
Customer risk segmentation
Contract analysis
Internet service analysis
High-risk customer insights
ML prediction analytics
📌 Key Learnings

This project helped develop skills in:

Data cleaning and preprocessing
Feature engineering
Imbalanced classification
Explainable AI
Business analytics
GenAI integration
ML workflow organization
💡 Future Improvements
Deploy using Streamlit or FastAPI
Add real-time prediction API
Integrate customer support chatbot
Use RAG with customer support history
Add automated email retention workflows
🏁 Conclusion

This project demonstrates a complete industry-style workflow combining:

✅ Data Analytics
✅ Machine Learning
✅ Explainable AI
✅ Generative AI
✅ Business Intelligence

The system enables telecom companies to proactively identify at-risk customers and take retention actions before churn occurs.
