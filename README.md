# 📊 Telco Customer Churn Analysis
#### by Korir Edwin
![Python](https://img.shields.io/badge/Python-Data%20Analysis-blue)
![SQL](https://img.shields.io/badge/SQL-Data%20Cleaning-red)
![Power BI](https://img.shields.io/badge/PowerBI-Visualization-yellow)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Random Forest](https://img.shields.io/badge/Algorithm-Random%20Forest-green)
![Dataset](https://img.shields.io/badge/Dataset-Telco%20Customer%20Churn-purple)
![Project](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)   
## 📌 Project Overview
This project analyzes the Telco Customer Churn dataset from Kaggle to identify patterns behind customer churn and build a machine learning model to predict customer retention.

The workflow includes **data cleaning using SQL, exploratory analysis through Power BI dashboards, and predictive modeling using Python** with a **Random Forest classifier**.

---

<details>
<summary>🛠 Tools & Technologies</summary>

<br>

**SQL Server** – Data cleaning and preprocessing  
**Power BI** – Interactive dashboards and visual insights  
**Python (Jupyter Notebook)** – Machine learning and model evaluation  

**Libraries Used**
- pandas
- matplotlib
- seaborn
- scikit-learn

</details>

---

<details>
<summary>📂 Dataset</summary>

<br>

Dataset Source:  
https://www.kaggle.com/datasets/blastchar/telco-customer-churn  

The dataset contains information about:

- Customer demographics  
- Service subscriptions  
- Account information  
- Billing details  
- Churn status  

### Data Preparation

Data cleaning was performed in **SQL Server**, including:

- Handling missing values  
- Converting the **TotalCharges** column from string to numeric  
- Mapping the **Churn** column to binary values  

Yes → 1

No → 0


The cleaned dataset was then imported into **Power BI** for visualization and **Python** for machine learning.

</details>

---

<details>
<summary>📊 Data Visualization (Power BI)</summary>

<br>

An interactive Power BI dashboard was built to analyze:

- Customer churn patterns  
- Customer tenure  
- Contract types  
- Internet service types  
- Customer Lifetime Value (LTV)

These insights helped identify churn drivers before building the predictive model.

</details>

---

<details>
<summary>🤖 Machine Learning Model</summary>

<br>

A **Random Forest Classifier** was used to predict customer churn.

**Model Configuration**

- Train/Test Split: **80 / 20**
- Estimators: **100**
- Random State: **42**

### Model Evaluation

| Metric | Class 0 (Retained) | Class 1 (Churned) |
|------|------|------|
| Precision | 83% | 67% |
| Recall | 92% | 46% |
| F1 Score | 87% | 55% |

**Overall Accuracy:** **80%**

</details>

---

<details>
<summary>🔎 Key Insights</summary>

<br>

**1️⃣ Customer Tenure**

Churned customers stay for an average of **18 months**, while retained customers stay around **38 months**.  
Longer-tenured customers are less likely to churn.

**2️⃣ Internet Service Impact**

- Fiber Optic: **~42% churn**
- DSL: **~20% churn**
- No Internet: **~6% churn**

**3️⃣ Contract Type Influence**

- Month-to-month: **~45% churn**
- One-year contract: **~12% churn**
- Two-year contract: **~2% churn**

**4️⃣ Lifetime Value**

Retained customers generate significantly **higher LTV** compared to churned customers.

**5️⃣ Feature Influence**

- Strong impact: **Contract Type, Internet Service**
- Low impact: **Gender**

</details>

---

<details>
<summary>💡 Business Recommendations</summary>

<br>

**Encourage Long-Term Contracts**

Offer discounts or loyalty rewards to move customers away from month-to-month plans.

**Improve Fiber Optic Service Experience**

Investigate service quality or pricing concerns affecting fiber customers.

**Strengthen Early Customer Engagement**

Many customers churn within **18 months**, so focus on onboarding and early retention.

**Boost Lifetime Value**

Use segmentation and upselling strategies to increase revenue from existing customers.

**Provide Proactive Support**

Identify customers experiencing service issues and provide early support.

**Use Machine Learning for Retention**

Deploy the churn prediction model to flag high-risk customers and trigger retention campaigns.

</details>