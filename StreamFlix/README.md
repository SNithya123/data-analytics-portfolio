# 📺 StreamFlix Content Analysis

**Tools Used:** Python, Pandas, Matplotlib, Seaborn

## 🧠 Project Overview

This project focuses on analyzing StreamFlix’s global content library to identify trends in content production and distribution across different countries. The primary goal is to provide actionable recommendations on:

- What types of shows/movies StreamFlix should focus on producing.
- How StreamFlix can strategically expand its business in new markets.

As a data analyst, the insights you generate from this analysis aim to assist content and strategy teams in making data-driven decisions.

## 📓 Project Notebook

You can view the complete analysis in the [Jupyter Notebook](./).

---

## 📂 Dataset

The dataset used is a publicly available dataset from Kaggle, containing StreamFlix’s title-level metadata, including:

- Title, type (Movie/TV Show), country, release year
- Director, cast, genre, date added, duration, rating, etc.

---

## 🔍 Key Questions Addressed

1. **Content Landscape:**
   - What types of content (TV Shows vs. Movies) dominate on StreamFlix?
   - What genres are most prevalent across regions?
   - How has content production changed over the past two decades?

2. **Global Expansion Strategy:**
   - What kind of content is available across different countries?
   - Which countries have the most diverse StreamFlix libraries?

3. **Content Timing & Launch:**
   - What is the ideal time of year to release a show or movie?
   - Are there seasonal trends in content additions?

4. **People Behind the Screen:**
   - Which directors and actors are most frequently featured?
   - Are there regional preferences in cast/creators?

---

## 📊 Exploratory Data Analysis (EDA)

### ✅ Data Cleaning & Preprocessing

- Converted date columns to datetime objects.
- Filled and handled missing values for `country`, `director`, and `cast`.
- Split multiple-value columns (e.g. `country`, `cast`) into lists for aggregation.

### 📈 Univariate Analysis

- **Content Type**: ~70% Movies, 30% TV Shows.
- **Genre**: Dominated by Dramas, International Movies, Comedies.
- **Release Year**: Steady increase in content from 2000s to 2019, drop after 2020.

### 📉 Bivariate Analysis

- **TV Shows vs. Movies Over Time**: TV Shows have grown faster than movies in the last decade.
- **Country vs. Content Volume**: US, India, UK, and Canada dominate content availability.
- **Monthly Trends**: December has the highest number of content additions — holiday strategy?

### 🌎 Content Availability by Country

- Used exploding techniques to account for multiple countries per title.
- US has the most titles overall; India leads in regional content.
- South Korea has a high volume of recent TV shows, indicating a growing market.

### 👥 Actor/Director Insights

- Directors like Raoul Peck and Jay Karas appear frequently.
- Cast includes recurring names like Anupam Kher, Jackie Chan, and Adam Sandler.

---

## 📌 Key Insights

- **TV Shows are Gaining Popularity**: StreamFlix has steadily shifted focus toward TV series.
- **Genre Preferences Vary by Region**: Indian users prefer thrillers and dramas, while US leans toward documentaries and stand-up specials.
- **Holiday Season is Key**: December sees a spike in content additions — opportunity for family-friendly, binge-worthy content.
- **Director & Actor Repeatability**: Content with recurring actors/directors tends to align with regional success. Reuse of talent works.

---

## 🧭 Recommendations

1. **Increase Investment in Regional Content**:
   - Countries like South Korea, India, and Brazil are growing content hubs.
   - Invest in localized content production for these regions.

2. **Leverage Release Timing**:
   - Capitalize on holiday periods, especially November–December, for new launches.

3. **Double Down on TV Shows**:
   - Audiences are showing higher retention with episodic content. More original series = more stickiness.

4. **Use Actor & Director Popularity Data**:
   - Collaborate with frequently featured and well-received artists across regions.
