# Financial Consulting Case Study: Credit Card Consumer Spend & Portfolio Risk Analysis
Financial consulting case study performing exploratory data analysis (EDA), behavioral segmentation, and risk assessment on 8,950 credit card accounts using Python, Pandas, and Seaborn.

## 📌 Project Overview
This project simulates a financial consulting engagement for a major retail banking institution facing stagnation in credit card revenue and underlying portfolio risks. Utilizing Python, this analysis performs advanced exploratory data analysis (EDA), behavioral segmentation, and risk assessment on a dataset of **8,950 active credit card holders** to uncover actionable growth levers and mitigate credit defaults.

### 💼 Business Objectives & Framework
Leveraging a blend of statistical analysis and commercial strategy, this project addresses three core executive mandates:
1. **Strategic Customer Segmentation:** Categorizing users based on balance-to-spend ratios to optimize targeted cross-selling.
2. **Purchase Mechanism Dynamics:** Evaluating customer preference for direct One-off Purchases vs. structured Installment Plans (EMIs).
3. **Credit Liquidity Risk Mapping:** Testing the risk hypothesis regarding high-interest Cash Advance utilization across different credit limits.

---

## 🛠️ Technical Stack & Tools
* **Language:** Python
* **Data Manipulation:** Data Cleaning, Median Imputation, Data Aggregation (`Pandas`, `NumPy`)
* **Data Visualization:** Exploratory Data Analysis, Distribution Mapping (`Seaborn`, `Matplotlib`)
* **Environment:** Jupyter Notebook

---

## 📊 Key Insights & Executive Deliverables

### 1. Customer Segmentation Portfolio
Using median distribution thresholds ($df['BALANCE'].median()$ and $df['PURCHASES'].median()$), the portfolio was segmented into four distinct behavioral quadrants:

* **VIP Spenders (2,098 Users):** The highest-value segment, driving **$5.09 Million** in total purchases with an average spend of **$2,430/customer** and an average credit line of $6,105.
* **Active Budgeters (2,377 Users):** High-velocity spenders ($1,455 avg. purchase) maintaining low revolving balances despite restricted credit lines ($4,474 avg. limit).
* **Risky / Inactive Accounts (2,377 Users):** Customers holding substantial credit capacity ($4,447 avg. limit) but generating minimal transaction volume ($66 avg. spend).

### 2. Purchase Preference Analysis
* **Finding:** The portfolio yields a **1.44 One-off to Installment Ratio**. 
* **Strategic Recommendation:** Capital spend heavily outpaces structured payment plans. The bank should deploy an automated, in-app EMI conversion feature for single-ticket purchases over $500 to capture high-margin interest income.

### 3. Disproving the Cash Advance Risk Hypothesis
* **Hypothesis:** Retail banks frequently assume lower-limit, lower-income users utilize high-risk Cash Advances.
* **Empirical Reality:** Statistical analysis revealed a weak-to-moderate positive correlation (**0.3040**). The highest-value cash advance spikes ($10,000+) overwhelmingly occurred among mid-to-high credit tier accounts ($5,000 - $15,000 limits). 
* **Risk Action:** Recommend tightening cash-draw limits on high-tier cards to minimize capital exposure right before potential defaults.

---

## 🚀 How to Run the Project
1. Clone this repository.
2. Ensure you have dependencies installed: `pip install pandas numpy matplotlib seaborn`
3. Open `credit_card_analysis.ipynb` in Jupyter Notebook and execute all cells.
