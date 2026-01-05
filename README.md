# Telco Customer Churn Analysis Dashboard

**Data Analytics • Customer Retention Insights • Looker Studio Dashboard**

This project analyzes over 7,000 customer records from a telecommunications company to uncover churn patterns, service usage behaviors, and revenue impacts. It is built as an end-to-end analytics workflow from data cleaning and exploratory analysis to visualization and strategic recommendations to support more informed and data-driven retention strategies.

---

## 1. Background

The telecommunications industry faces high customer churn rates, where the cost of acquiring new customers is significantly higher than retaining existing ones. Understanding *why* customers leave whether due to pricing, service quality, or contract flexibility is crucial. This project addresses that challenge by leveraging historical customer data to identify at-risk segments and guide measured interventions to improve loyalty.

---

## 2. Analytical Workflow

### 1. Business Understanding
**Defined business goals:**
* Identify the profile of customers most likely to churn.
* Determine which services build customer stickiness.
* Provide actionable insights to reduce revenue loss.

### 2. Data Collection
* Dataset: **Telco Customer Churn** (Source: Kaggle).
* Volume: 7,043 rows with 21 features (Demographics, Services, Account Info).

### 3. Data Preparation
**Performed rigorous cleaning:**
* Handled missing values in `TotalCharges`.
* Converted data types for accurate calculation.
* Encoded categorical variables for analysis.
* Verified data integrity (duplicates and null checks).

### 4. Exploratory Data Analysis
**Identified trends:**
* Analyzed churn rates across tenure groups.
* Evaluated the impact of payment methods and contract types.
* Correlated monthly charges with churn probability.

### 5. Dashboard Development
* Built an interactive **Looker Studio dashboard** to deliver fast, insight-driven decision support for stakeholders.

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
 ├── deliverables/
 │   ├── dashboard/            # Looker Studio screenshots
 │   └── report/               # Final insights report
 └── README.md
