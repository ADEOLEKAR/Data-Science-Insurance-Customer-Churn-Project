**Auto Insurance Churn Analysis**  
**Predicting Customer Retention Using Machine Learning**  

**Overview**  
This project analyzes **customer churn in auto insurance**, identifying key factors and predicting churn using machine learning models.  

**Business Problem**  
- **Why Predict Churn?**  
  - Retaining customers is **cheaper** than acquiring new ones.  
  - High churn signals **lost revenue** and **customer dissatisfaction**.  
- **Key Questions:**  
  1. **Who is likely to churn?**  
  2. **What factors drive churn?**  
  3. **How can insurers reduce churn?**  

---

**Data Overview**  
- **92,000 customers, 23 features** (Demographics, Financials, Policy Details, Geographic).  
- **Churn Indicator:** **1 = churned, 0 = retained**.  
- **Data Cleaning:**  
  - Filled missing values for **City, County, Latitude/Longitude**.  
  - Dropped **Account Suspension Date & redundant IDs**.  

**Feature Engineering**  
- **Log-transformed income** to reduce skewness.  
- **Binned home values** for better analysis.  
- **Created account suspension indicator** for readability.  

**Model Performance Comparison**  

| **Model** | **Accuracy** | **Precision** | **Recall** | **F1 Score** |  
|-----------|------------|-------------|-----------|-----------|  
| **Decision Tree (SMOTE)** | **0.82** | **0.32** | **0.47** | **0.38** |  
| **Logistic Regression (Optimal)** | **0.86** | **0.37** | **0.36** | **0.37** |  
| **KNN (K=5)** | **0.88** | **0.44** | **0.19** | **0.26** |  
| **Voting Classifier** | **0.89** | **0.50** | **0.33** | **0.39** |  

**Best Model:** **Decision Tree with SMOTE**  
- **Balanced precision and recall**  
- **Scalable for large datasets**  

**Key Findings & Business Recommendations**  

| **Factor** | **Impact on Churn** | **Strategy** |  
|-----------|----------------|----------------|  
| **Short tenure (<1 year)** | **Increases** | Offer onboarding incentives |  
| **Long tenure (>5 years)** | **Decreases** | Provide loyalty rewards |  
| **Homeowners (82%)** | **Decreases** | Promote bundling discounts |  
| **Lower-income customers** | **Increases** | Offer budget-friendly plans |  
| **Recently relocated customers** | **Increases** | Engage with personalized incentives |  

**Final Thought**  
_"Understanding churn helps insurers retain customers, optimize pricing, and improve satisfaction."_  
