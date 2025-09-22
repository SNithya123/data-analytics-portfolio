# 🚲 CycleShare-Co Demand Analysis | Hypothesis Testing in Action

## 📌 Project Overview

This project explores demand patterns for **CycleShare-Co**, a shared electric cycle provider in India. The objective is to identify **factors that significantly impact the number of cycles rented**, helping the business make data-backed operational and marketing decisions.

Using statistical techniques like **t-tests, ANOVA, and chi-square tests**, we validate or refute hypotheses around customer behavior, seasons, and weather influence on rental patterns.

---

## 📓 Project Notebook

You can view the complete analysis in the [Jupyter Notebook](./).

---

## 🧰 Tools & Technologies

- **Language:** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy.stats`  
- **Concepts Used:**  
  - Exploratory Data Analysis  
  - Hypothesis Testing  
    - 2-sample t-test  
    - ANOVA  
    - Chi-Square Test  
  - Visual Analysis (Boxplots, Histograms, Countplots)

---

## 🧪 Key Analytical Questions & Tests Conducted

| Business Question | Test Type | Key Variable(s) |
|------------------|-----------|------------------|
| Does demand differ between working and non-working days? | 2-sample t-test | `workingday`, `count` |
| Is rental demand the same across different seasons? | One-way ANOVA | `season`, `count` |
| Does weather significantly affect the number of cycles rented? | One-way ANOVA | `weather`, `count` |
| Is weather type dependent on the season? | Chi-square test | `season`, `weather` |

---

## 🔍 Workflow Summary

1. **Data Exploration & Cleaning**
   - Loaded and inspected dataset
   - Identified data types, missing values, and outliers
   - Handled categorical features (`season`, `weather`, `workingday`) with `.astype('category')`

2. **Univariate Analysis**
   - Distribution plots for numerical variables (e.g. `count`)
   - Countplots for categorical variables

3. **Bivariate Analysis**
   - Explored how rental counts vary with season, weather, and workday status using boxplots

4. **Hypothesis Testing**
   - Defined null and alternate hypotheses
   - Checked assumptions (normality visually and via stats tests)
   - Ran appropriate tests and interpreted p-values

---

## 📈 Insights & Interpretations

- ✅ **Working days** show significantly higher average rentals than non-working days.  
  _→ Operational focus and fleet availability should increase during weekdays._

- 🍂 **Seasonality** plays a strong role: **Summer and Fall** show peak demand.  
  _→ Promotional offers and peak pricing can be explored in these months._

- 🌧️ Rentals are lower in poor weather conditions (e.g., light rain or mist).  
  _→ Real-time weather integration in pricing/demand models can optimize fleet allocation._

- 🔄 **Weather types are not independent of seasons**, confirmed via the chi-square test.  
  _→ Seasonal planning should account for expected weather disruptions._

---

## ✅ Business Recommendations

- 📅 **Increase marketing and availability on working days** — most customers commute on weekdays.
- 📊 Launch **season-based pricing models** and expand fleet in high-demand months.
- 🌤️ **Integrate weather forecasting** to optimize cycle deployment and improve customer experience.
- 🎯 Focus customer acquisition efforts in **urban areas** where weather has lower impact on commute choices.

---


## 🧠 What I Learned

- How to design and implement **hypothesis tests** to validate business questions
- Importance of **assumptions** in statistical tests and how to interpret **p-values**
- How to combine visual and statistical evidence for stronger storytelling
- Translating abstract statistical outputs into **clear business impact**


---
