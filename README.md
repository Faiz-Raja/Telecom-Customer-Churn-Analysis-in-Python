# 📊 Telecom Customer Churn Analysis (TCA)

This project aims to analyze customer churn patterns for a telecom company using customer demographics, account details, and service usage. The goal is to identify key drivers of churn and provide actionable business insights to reduce customer attrition.

---
## 📌 Overview

This data analysis project explores a telecom company's customer churn dataset to uncover patterns and trends that impact customer retention. The dataset includes various attributes like service usage, demographics, and billing behavior.

**The project includes:**

• Data cleaning and transformation.

• Exploratory Data Analysis (EDA).

• Visualization of churn trends across demographics and service categories.

• Actionable recommendations to reduce churn.

---
## 🎯 Objective

• Understand why customers are leaving the telecom service.

• Identify the most influential factors leading to churn.

• Provide actionable recommendations to improve customer retention and profitability.

---
## 🛠️ Tools & Technologies

**Python:** Pandas, NumPy, Matplotlib, Seaborn.

**Jupyter Notebook:** Interactive development

**Data Visualization:** Bar plots, pie charts, heatmaps

---
## 📂 Project Structure

```
├── notebooks/
│   └── TCA.ipynb                   # Main notebook (Telecom Customer Churn Analysis)
├── assets/
│   └── plots/                      # Visual insights (EDA charts, graphs)
├── Customer Churn.csv             # Dataset used
├── README.md                      # Project documentation
```

---
## 🔍 Methodology

### **🧹 Data Collection**

• Imported Customer Churn.csv into a Pandas DataFrame

• Dataset includes 7,043 records with 21 features:

• **Demographics:** Gender, SeniorCitizen, Partner, Dependents

•  **Services:** PhoneService, InternetService, StreamingTV, etc.

• **Billing:** MonthlyCharges, TotalCharges, PaymentMethod
  
• **Target:** Churn (Yes/No)


### **📊 Exploratory Data Analysis (EDA)**

**Key Insights & Graphs:**

**🔑 Primary Visualization:** Churn by Payment Method

• **Graph:** Seaborn countplot analyzing churn distribution across PaymentMethod.

**Details:**

• **X-axis:** PaymentMethod (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))

• **Hue:** Churn status (Yes/No), distinguishing churned vs. non-churned customers

• **Enhancements:** Bar labels for exact counts, 45° x-axis rotation for readability, 4x5-inch figure size, titled "Churned Customers by Payment Method"

• **Insight:** Customers using Electronic Check or Mailed Check exhibit significantly higher churn rates compared to those using automatic payment methods (Bank transfer, Credit card). This suggests manual payment processes may contribute to customer dissatisfaction or inconvenience.

• **Implication:** Encouraging automatic payment methods could reduce churn by streamlining billing.

---

**🔐 Potential Other Visualization:** Tenure vs. Churn

**Graph:** A boxplot comparing tenure (months with the company) for churned vs. non-churned customers.

**Expected Insight:** Customers with shorter tenure are likely to have higher churn rates, as newer customers may be less loyal or still evaluating the service. A boxplot could reveal that churned customers have a median tenure significantly lower than non-churned customers (e.g., <6 months vs. >24 months).

**Implication:** Retention strategies targeting new customers (e.g., onboarding incentives) could reduce early churn.

---

## EDA Summary

• The primary visualization confirms payment method as a critical churn factor, with manual methods (Electronic check, Mailed check) linked to higher attrition.

• Additional analyses on tenure, MonthlyCharges, and Contract could further uncover churn drivers, as these features are present in the dataset and likely influence customer behavior.

• The visualizations provide clear, data-driven insights for stakeholders, highlighting actionable areas for retention strategies.

---
## Key Findings

• **Top Insight 🚨:** Customers using Electronic Check or Mailed Check are significantly more likely to churn, likely due to the inconvenience of manual payment processes.

• **Visualization 🎨:** The countplot clearly illustrates higher churn counts for Electronic check, followed by Mailed check, compared to automatic payment methods.

**Additional Potential Insights 🔎:**

• Shorter tenure may correlate with higher churn, suggesting a need to target new customers.

• Higher monthly charges could drive churn among price-sensitive customers.

• Month-to-month contracts likely increase churn risk compared to longer-term contracts.

**Recommendation 💡:** Promote automatic payment methods (Bank transfer, Credit card) and consider incentives for longer contracts or lower-cost plans to reduce churn.

---
## 📚 Appendix

**Dataset:** Customer Churn.csv

**Key Features:**

**customerID:** Unique customer identifier

**PaymentMethod:** Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)

**Churn:** Binary target (Yes/No)

**Others:** tenure, MonthlyCharges, TotalCharges, gender, Contract, etc.

**Libraries:** pandas, numpy, matplotlib, seaborn

---
## 📄 Explore the Full Analysis
**For a deeper dive, explore:**

• 📓 TCA.ipynb in the notebooks/ directory for detailed code and visualizations

• 📋 Customer Churn.csv for the raw dataset
