# 🛒 MegaMart Black Friday Spend Analysis | Confidence Intervals & CLT

## 📌 Project Overview

This project explores customer purchase behavior at **MegaMart**, a leading retail chain, with a focus on **gender-based, age-based, and marital status-based spending patterns** during Black Friday sales.

The analysis leverages **Confidence Intervals** and the **Central Limit Theorem (CLT)** to generalize insights from sample data to the broader population. This helps answer key questions like:

- Do women spend more per transaction than men?
- Are there differences in spending across age groups?
- Can we draw statistically sound conclusions from sample data?

---

## 📓 Project Notebook

You can view the complete analysis in the [Jupyter Notebook](./Megamart_Business_Case.ipynb).

---

## 🧰 Tools & Technologies

- **Language:** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`  
- **Concepts Used:**  
  - Exploratory Data Analysis  
  - Confidence Interval  
  - Central Limit Theorem (CLT)  
  - Sampling  
  - Group-wise statistical comparisons  
  - Visualization (Boxplots, Histograms, Distribution Plots)

---

## 🧪 Key Analytical Steps

- Cleaned and explored transaction-level purchase data
- Detected and visualized **outliers** and **missing values**
- Grouped data based on:
  - **Gender**: Male vs Female
  - **Marital Status**: Married vs Unmarried
  - **Age Brackets**: 0-17, 18-25, 26-35, 36-50, 51+ years
- Applied **Central Limit Theorem** to create sampling distributions
- Calculated **95% and 99% confidence intervals** for mean purchase amount
- Compared spending patterns using visual and statistical inference

---

## 🔍 Core Questions Answered

1. **Do women spend more than men on average during Black Friday?**  
   → Applied CLT and visualized the sampling distribution for male and female spending.

2. **Are the average spends of married and unmarried customers statistically different?**  
   → Confidence intervals compared to check for overlap.

3. **Which age group contributes the most in terms of average spend?**  
   → Age-grouped sampling and confidence intervals were constructed.

4. **Are the observed differences significant at a 95% confidence level?**  
   → Yes — statistically backed insights for each demographic segment.

---

## 📈 Insights & Takeaways

- 👩 **Female customers consistently spent more per transaction** compared to male customers.
- 💍 **Unmarried customers** had slightly higher spending, possibly due to more discretionary income.
- 📊 **Age group 26–35** emerged as the highest spending demographic during Black Friday.
- ✅ The **confidence intervals for male vs. female spending did not overlap**, confirming significant difference.
- 📉 Spending **variance was higher among older age groups**, indicating inconsistent shopping behavior.

---

## ✅ Business Recommendations for MegaMart

- 📣 Tailor marketing campaigns to target **female customers in the 26–35 age group** — the most valuable segment.
- 💡 Launch curated offers for **unmarried individuals**, especially in electronics and lifestyle categories.
- 📊 Use insights from confidence intervals to drive **inventory planning** and **promotional strategies** for Black Friday sales.
- 🛍️ Introduce age-specific bundles or loyalty points to engage low-spend segments like 0–17 or 51+.

---

## 🧠 What I Learned

- How to apply **statistical inference** to large-scale customer data.
- Importance of **sampling** and how the **Central Limit Theorem** underpins population estimation.
- Practical use of **confidence intervals** in comparing demographic segments.
- Translating technical statistical outputs into **actionable business insights**.

---
