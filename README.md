# Telco Customer Churn Analysis Dashboard

**Data Analytics • Customer Retention Insights • Looker Studio Dashboard**

This project analyzes over 7,000 customer records from a telecommunications company to uncover churn patterns, service usage behaviors, and revenue impacts. It is built as an end-to-end analytics workflow—from data cleaning and exploratory analysis to visualization and strategic recommendations to support more informed and data-driven retention strategies.

<p align="center">
  <img src="Deleverables/Dashboards/Dashboard%20Preview.png" alt="Telco Customer Churn Dashboard" width="35%" style="border-radius: 10px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);"/>
</p>

---

## 1. Background

The telecommunications industry faces high customer churn rates, where the cost of acquiring new customers is significantly higher than retaining existing ones. Understanding *why* customers leave—whether due to pricing, service quality, or contract flexibility—is crucial. This project addresses that challenge by leveraging historical customer data to identify at-risk segments and guide measured interventions to improve loyalty.

---

## 2. Methodology: CRISP-DM

This project follows the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** framework to ensure a structured, business-centric approach to data analysis.

<p align="center">
  <img src="Deleverables/Methodology/CRISP-DM.png" alt="CRISP-DM Methodology Workflow" width="35%" style="border-radius: 10px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);"/>
</p>

### 1. Business Understanding
**Objective:** Reduce customer churn and increase retention rates.
* **Key Questions:** What are the primary drivers of churn? Which customer segments are most vulnerable?
* **Goal:** Provide actionable insights to the marketing and retention teams to reduce revenue loss.

### 2. Data Understanding
* **Source:** **Telco Customer Churn** Dataset (Kaggle).
* **Volume:** 7,043 rows, 21 features.
* **Scope:** Customer demographics, services subscribed (Phone, Internet, Streaming), and account details (Tenure, Contract, Charges).

### 3. Data Preparation
**Rigorous cleaning process to ensure data quality:**
* **Handling Missing Values:** Imputed null values in `TotalCharges`.
* **Type Conversion:** Corrected data types for accurate numeric calculations.
* **Encoding:** Transformed categorical variables for analysis.
* **Integrity Check:** Verified duplicates and consistency.

### 4. Modeling & Analysis (EDA)
**Deep dive into data patterns:**
* **Univariate Analysis:** Distribution of churn across tenure and services.
* **Bivariate Analysis:** Impact of payment methods and contract types on churn.
* **Correlation:** Analyzed the relationship between `MonthlyCharges` and churn probability.

### 5. Evaluation
**Key Insights Validation:**
* Confirmed that **Month-to-month contracts** are the biggest churn driver.
* Validated that high churn in the first 12 months indicates onboarding issues.
* Identified **Electronic Check** as a high-friction payment method.

### 6. Deployment
* **Dashboarding:** Built an interactive **Looker Studio dashboard** to visualize KPIs.
* **Reporting:** Summarized strategic recommendations for stakeholders.

---

## 3. Key Findings

* **High Risk in First Year:** New customers (0-12 months tenure) have the highest churn rate (**47.7%**), making onboarding critical.
* **Payment Method Impact:** Customers using **Electronic Check** have a significantly higher churn rate (**45.3%**) compared to automated payment methods.
* **Pricing Sensitivity:** Churned customers have higher average monthly charges (**$74.44**) compared to retained customers (**$61.27**).
* **Service Bundles:** Customers with **no additional services** (like Tech Support or Security) are more likely to leave. Engagement drives retention.

---

## 4. Strategic Recommendations

* **Target the First Year:** Implement a dedicated "First-Year Success" program with check-ins to reduce early churn.
* **Migrate Payment Methods:** Incentivize users to switch from Electronic Check to Credit Card or Bank Transfer (Auto-pay) to improve stickiness.
* **Promote Bundling:** Offer discounts on Tech Support or Online Security to single-service users to increase switching costs.
* **Contract Strategy:** Encourage 1-year or 2-year contracts over Month-to-month plans through loyalty rewards.

---

## 5. Tools & Technologies

### 🛠 Languages and Tools
<p align="left">
  <a href="https://www.python.org" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" width="40" height="40"/></a>
  <a href="https://pandas.pydata.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/pandas/pandas-original.svg" width="40" height="40"/></a>
  <a href="https://numpy.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/numpy/numpy-original.svg" width="40" height="40"/></a>
  <a href="https://matplotlib.org/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" width="40" height="40"/></a>
  <a href="https://seaborn.pydata.org/" target="_blank"><img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" width="40" height="40"/></a>
  <a href="https://jupyter.org/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/jupyter/jupyter-original-wordmark.svg" width="40" height="40"/></a>
  <a href="https://www.kaggle.com/" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/kaggle/kaggle-original.svg" width="40" height="40"/></a>
  <a href="https://lookerstudio.google.com/" target="_blank"><img src="https://www.vectorlogo.zone/logos/google_datastudio/google_datastudio-icon.svg" width="40" height="40"/></a>
</p>

---

## 6. Project Structure

```text
 telco-customer-churn-analysis
 ├── data/
 │   ├── raw/                  # Original dataset
 │   ├── cleaned/              # Processed data for dashboard
 ├── notebooks/
 │   └── Telco_Dataset.ipynb   # Main analysis notebook
 ├── Deleverables/
 │   ├── Dashboards/
 │   │   └── Dashboard Preview.png  #  # Dashboard preview images
 │   ├── Methodology/
 │   │   └── CRISP-DM.png           # Methodology Workflow
 │   └── Report/
 │       └── PPT Telco Churn Analaysis.pdf # Project documentation
 └── README.md
