# 🏦 Bank Term Deposit Prediction & Analysis

## 📌 Project Overview
This project analyzes a direct marketing campaign (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe to a term deposit (variable `y`).

Our analysis combines **Exploratory Data Analysis (EDA)** and **Statistical Hypothesis Testing** (T-Test, Chi-Square, ANOVA) to identify the ideal customer profile, optimal contact times, and actionable strategies to increase the subscription rate.

## 📊 Key Insights & Findings

### 1. 🎯 The "Golden" Customer Profile
Our statistical tests confirm that **Wealth** and **Life Stage** are the strongest predictors of success.
* **Financials (T-Test):** Wealth is a major driver. Subscribers have **38% higher average balances** ($1,234) compared to non-subscribers ($894).
* **Debt Status:** Customers **without a housing loan** are **2x more likely** to subscribe.
* **Demographics (Chi-Square):** **Students** and **Retirees** have the highest conversion rates, likely due to a need for low-risk savings.
* **Marital Status (ANOVA):** **Married** customers require significantly more effort (~7% more calls) to convert compared to Single customers, likely due to spousal consultation.

### 2. 📅 The "Winning" Season (When to Call)
* **Winter Opportunity (Q1 & Q4):** The highest subscription rates occur in **Jan-Mar** and **Oct-Dec**, driven by New Year resolutions and year-end planning.
* **Summer Trap (Q2):** The bank currently expends the most effort in **May**, but it yields the lowest success rate. This represents a significant inefficiency in budget allocation.

### 3. ⚡ Operational Efficiency (How to Call)
* **The "3-Strike" Rule:** The average successful sale takes **~2 calls**. Effectiveness drops sharpyl after 3 attempts.
* **Mobile First:** Prioritize **Cellular** numbers (15% conversion) over Unknown/Landline numbers (4% conversion).

---

## 💡 Strategic Recommendations
**"Precision over Volume"**
Instead of aggressive mass-calling in May (Q2), the strategy should shift to:
1.  **Filter the list:** Remove low-balance (<$500) and housing-loan-burdened leads.
2.  **Segment the Script:** Pitch "Safety" to Students/Retirees and "Liquidity" to Management professionals.
3.  **Reallocate Resources:** Move 30% of the Q2 budget to the high-performing Winter months (Q1 & Q4).

---

## 🛠️ Instructions to Run
1.  **Setup:** Install required libraries:
    ```bash
    pip install pandas matplotlib seaborn scipy
    ```
2.  **Load Data:** Place `cleaned_day2.csv` in your working directory.
3.  **Preprocessing:**
    * Map `month` to `quarters` (Q1-Q4).
    * Convert target `y` to binary (0/1).
4.  **Execute:** Run the Jupyter Notebook to generate the visualizations and statistical test results included in this report.


---

**Author:** Muhammed Jaseem VT
**Email:** vtjaseem7@gmail.com

