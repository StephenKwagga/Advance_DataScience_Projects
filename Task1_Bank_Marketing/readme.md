# 📌 INTRODUCTION  

Dataset:  
- UCI Bank Marketing Repository — records from a marketing campaign promoting term deposits.  
Content:  
- Includes customer details such as age, job, call duration, previous campaign outcome, and contact month.  

# 🎯 OBJECTIVE  
- Predict whether a customer will subscribe to a term deposit.  
- Preprocess the data, including encoding categorical features.  
- Train and evaluate Logistic Regression and Random Forest models using Accuracy, F1-score, and ROC AUC.  
- Use LIME to explain predictions and highlight the most influential factors.

# ✅ FINAL CONCLUSION

Model Results:  
- Logistic Regression: Accuracy = 0.80, F1-score = 0.78, ROC AUC = 0.885  
- Random Forest: Accuracy = 0.82, F1-score = 0.81, ROC AUC = 0.89  

Insights from LIME Explanations:  
LIME analysis of 5 predictions per model showed that the most influential features were:  
- Call duration — longer conversations strongly increased the likelihood of subscription  
- Previous campaign outcome — successful past responses led to higher conversion chances  
- Month of contact — timing had a measurable effect on outcomes  
- Customer age — older customers were more likely to subscribe in some cases  

# 🔍 Strategic Suggestions:

1. Deploy Random Forest in production systems due to its superior performance and ability to capture complex patterns in customer behavior.

2. Target high-potential leads by focusing on:
   - Customers with long call durations
   - Those with previously successful campaign interactions

3. Refine campaign timing by launching marketing efforts during months with historically higher response rates.

4. Segment customers by age and interaction history to personalize messages and improve engagement.

5. *Use LIME periodically* to audit model decisions, improve transparency, and ensure fairness in targeting strategies.


Summary: 
Random Forest combined with LIME delivers both predictive power and interpretability. These tools enable data-driven, targeted marketing that can increase subscription rates while reducing wasted outreach.

