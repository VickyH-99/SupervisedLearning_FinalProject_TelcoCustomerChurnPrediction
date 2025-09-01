# Telco Customer Churn Prediction  
**Supervised Learning Final Project**  

## Project Overview  
Customer churn is a critical challenge for subscription-based businesses, leading directly to revenue loss and higher acquisition costs. This project applies supervised machine learning to answer the central question:  
**Which customers are most likely to churn, and how can we prevent it?**

In my professional experience as a data analyst in a logistics platform, customer retention has always been closely tied to business outcomes such as Gross Transaction Value (GTV) and operational efficiency. For example, every day thousands of potential customers leave their information, but due to limited resources, we cannot follow up with all of them. If we can accurately identify those at highest risk of churn, we can optimize retention strategies, focus outreach where it matters most, and maximize return on investment. This same principle applies to telecom and subscription businesses, which is the motivation behind this project.  

## Objectives  
1. Explore customer patterns through exploratory data analysis (EDA)  
2. Build and compare predictive machine learning models  
3. Identify the most important drivers of churn  
4. Translate technical results into actionable business strategies  

## Dataset  
The project uses the **Telco Customer Churn dataset** from Kaggle:  
[Telco Customer Churn - Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  

## Methodology  
1. **Data Preparation** – cleaning, encoding categorical features, scaling numeric variables, and addressing class imbalance with SMOTE  
2. **Model Building** – Logistic Regression, Random Forest, XGBoost, LightGBM, SVM, KNN, and Stacking  
3. **Model Evaluation** – primarily ROC-AUC (all models ≈ 0.84–0.85), complemented by Precision, Recall, F1, and confusion matrices  
4. **Interpretation & Action** – feature importance, permutation importance, PDP/ICE plots, and linking results to business decisions  

## Key Findings  
- **Model performance**: Logistic Regression and Random Forest achieved the highest AUC (≈0.846). Boosting models (XGBoost, LightGBM) showed clear improvements over their baselines and remain promising for richer datasets.  
- **Churn drivers**: ARPU, tenure, contract type, payment method, internet service, and monthly/total charges consistently emerged as the most influential factors.  
- **Business impact**: Reducing churn by just 5% translates into approximately **$293K in retained annual revenue** for a customer base of 7,000 with ARPU of $840/year.  

## Conclusion & Next Steps  
The value of this project lies not only in comparing algorithms but in converting insights into retention strategies:  
- Prioritize outreach for high-ARPU, short-tenure customers  
- Promote longer-term contracts and stable payment methods  
- Strengthen value perception for high-bill customers through transparent pricing and bundled services  

**Next steps**: enrich feature engineering with behavioral data, test boosting methods on larger datasets, and integrate predictions into real business workflows. Continuous monitoring and recalibration are essential to ensure the model adapts as customer behavior evolves.  

## Repository Contents  
- `TelcoChurn_Notebook_SLFinalProject.ipynb` → Full analysis and modeling notebook  
- `TelcoChurn_Slides_SLFinalProject.pdf` → Presentation slides  
