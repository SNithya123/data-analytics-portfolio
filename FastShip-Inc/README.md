# 🚚 FastShip-Inc | Feature Engineering for Logistics Optimization

## 📌 Project Overview

This project focuses on optimizing delivery logistics for **FastShip-Inc**, a tech-enabled courier company aiming to improve delivery forecasts and reduce inefficiencies in its supply chain.

The goal is to extract meaningful features from raw trip and delivery data using **feature engineering techniques** and **exploratory analysis**, thereby enabling the data science team to build more accurate forecasting models.

---

## 📓 Project Notebook

You can view the complete analysis in the [Jupyter Notebook](./).

---

## 🧰 Tools & Technologies

- **Language:** Python  
- **Libraries:** `pandas`, `numpy`, `seaborn`, `matplotlib`, `scipy`, `sklearn`  
- **Techniques:**  
  - Data Cleaning & Aggregation  
  - Feature Extraction from Timestamps & Text  
  - Handling Missing Values & Outliers  
  - Hypothesis Testing  
  - Data Normalization & Encoding  

---

## 🧠 Objectives

- Clean and standardize messy delivery data
- Derive new features from raw columns (timestamps, locations, durations)
- Perform time/distance-based hypothesis testing between key delivery metrics
- Handle outliers and missing values effectively
- Prepare the dataset for downstream predictive modeling

---

## 🔎 Key Features Engineered

| Feature Name | Description |
|-------------|-------------|
| `trip_month`, `trip_day` | Extracted from `trip_creation_time` |
| `source_city`, `source_state` | Parsed from `source_name` |
| `destination_city`, `destination_state` | Parsed from `destination_name` |
| `actual_time_taken` | Derived from `od_start_time` and `od_end_time` |
| `osrm_delay` | Difference between actual time and OSRM estimated time |
| `segment_vs_trip_comparison` | Analyzed difference between trip-level and segment-level durations/distances |

---

## 🧪 Hypothesis Testing Conducted

| Business Question | Method Used |
|------------------|-------------|
| Is there a significant difference between actual delivery time and OSRM predictions? | Paired t-test |
| Are trip-level and segment-level distance metrics consistent? | Paired t-test |
| Is the scan-to-delivery time consistent with expected delivery time? | Visual + Statistical comparison |

---

## 📈 Exploratory Insights

- 📦 **OSRM delivery estimates** tend to **underestimate** actual delivery times, especially on inter-city corridors.
- 🚦 **Segment-level data** often has **variance**, suggesting logistical bottlenecks during middle-mile operations.
- 🧭 Most trips originate from **key metros (Mumbai, Delhi, Bangalore)** and deliver across **Tier-2/3 cities**, indicating a hub-to-spoke distribution model.
- 🧮 Strong correlation found between **trip distance** and **delay variance**, emphasizing the need for better routing models.

---

## 🛠️ Data Preprocessing Steps

- **Missing Value Treatment:**  
  - Imputed or dropped based on column criticality  
  - Visualized with heatmaps and missingno library

- **Outlier Detection & Handling:**  
  - Used IQR method  
  - Visualized with boxplots for fields like `actual_time_taken`, `osrm_time`, `segment_time`

- **Normalization:**  
  - Applied `MinMaxScaler` and `StandardScaler` for model-readiness

- **Encoding:**  
  - One-hot encoded categorical features such as `route_type`, `state`, etc.

---


## ✅ Business Recommendations

- 🔁 **Review and update OSRM routing algorithms** to reflect real-time traffic and delays.
- 🧱 **Decompose trip segments** for micro-optimization — focus on where maximum delays occur.
- 📍 Focus on optimizing **long-haul deliveries** as they contribute to majority of the delivery variance.
- 📊 Use engineered features to build **predictive delivery time models** for SLA management.

---
