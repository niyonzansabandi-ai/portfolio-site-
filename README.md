# Customer Churn Prediction Project

## Overview
This project focuses on predicting customer churn using machine learning techniques. The goal is to identify customers who are likely to leave a subscription-based service so the business can take proactive retention actions. The project includes data cleaning, exploratory analysis, model development, evaluation, and business recommendations based on model insights.

## Dataset
The dataset contains customer demographic information, service usage details, billing information, and whether the customer churned. Key features include tenure, monthly charges, total charges, contract type, payment method, and internet service type.

## Modeling Approach
Several models were trained and compared:

- Logistic Regression  
- Random Forest  
- Balanced Random Forest  

Because churn is a minority class, accuracy alone is not sufficient. The primary focus was on recall for churners, ensuring the model correctly identifies customers who are at risk of leaving.

## Model Performance
The Balanced Random Forest model delivered the strongest performance:

- Recall for churners: 0.92  
- Precision for churners: 0.84  
- F1-score: 0.87  
- Overall accuracy: 0.805  

This model significantly improved recall compared to the baseline Random Forest, which only achieved a recall of 0.45 for churners.

## Key Insights from Feature Importance
The most influential features in predicting churn were:

- Tenure  
- Total charges  
- Monthly charges  
- Internet service type (fiber optic)  
- Payment method (electronic check)  

Customers with low tenure, low total charges, high monthly charges, fiber optic service, or electronic check payment method were more likely to churn.

## Business Recommendations
Based on the model results and feature importance analysis, the following actions are recommended:

1. Focus on customers with low tenure through onboarding and early engagement programs.  
2. Offer discounts or bundled pricing to customers with high monthly charges.  
3. Investigate service quality issues for fiber optic customers.  
4. Encourage customers using electronic check to switch to more stable payment methods.  
5. Provide targeted support to customers with low total charges who may be new or under-engaged.  
6. Use the model to generate weekly lists of high-risk customers for proactive retention outreach.

## Conclusion
This project demonstrates a complete end-to-end machine learning workflow for predicting customer churn. The Balanced Random Forest model provides strong performance, especially in identifying customers at risk of leaving. The insights gained from the model support actionable business strategies that can reduce churn and improve customer retention.

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Jupyter Notebook  

## How to Run the Project
1. Install required Python libraries.  
2. Open the Jupyter Notebook.  
3. Run the cells in order to reproduce the analysis and results.  
