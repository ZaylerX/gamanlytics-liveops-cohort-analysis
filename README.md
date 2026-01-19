# 🎮 Gaming LiveOps Analysis — Retention, LTV & A/B Testing

This project analyzes user behavior and monetization performance in a free-to-play gaming context using cohort analysis, monetization KPIs and A/B test evaluation.

The goal is to simulate a typical **LiveOps / Product Analytics workflow** used in mobile and online games to support data-driven decisions on player engagement and monetization strategies.

---

## 🎯 Business Questions

The analysis focuses on answering the following questions:

- How does user retention evolve during the first 30 days after installation?
- How much value does each cohort generate over time (LTV)?
- What drives monetization: payer conversion or spending intensity?
- Did an A/B test variant improve monetization performance?
- Is early retention correlated with long-term value?

---

## 📊 Analysis Workflow

### 1. Data Cleaning & Preparation (Python)
- Timestamp conversion from Unix time
- Creation of registration, login and revenue event tables
- Export of clean datasets and SQLite database

### 2. Cohort Construction (SQL)
- Daily install cohorts
- Days since install calculation
- Retention curves (D0–D30)

### 3. Monetization Analysis (SQL)
- ARPU, ARPPU and payer rate by cohort
- Lifetime Value (LTV) calculation
- Monetization funnel evaluation

### 4. A/B Test Evaluation (SQL)
- Monetization KPIs by test group
- Uplift calculation for ARPU, payer rate and ARPPU

### 5. Retention vs Monetization Relationship
- Cumulative LTV curves by cohort
- Scatter analysis between D7 retention and D30 LTV
- Correlation analysis to evaluate engagement–value relationship

### 6. Visualization & Storytelling (Tableau Public)
- Interactive dashboards for business interpretation
- KPI summaries and experiment insights

---

## 📈 Dashboards (Tableau Public)

Interactive dashboards are available here:

👉 **https://public.tableau.com/app/profile/federico.mistretta/viz/GamingLiveOpsAnalysisRetentionLTVABTesting/UserRetentionCurveD0-D30#2**

Dashboards included:
1. Retention curves (D0–D30)
2. Monetization KPIs and LTV by cohort
3. A/B test monetization comparison
4. Retention vs LTV relationship analysis

---

## 📦 Dataset Source & Notes

The dataset used in this project comes from the Kaggle competition:

👉 **Gamelytics Mobile Analytics Challenge**  
https://www.kaggle.com/datasets/debs2x/gamelytics-mobile-analytics-challenge/data

It contains:
- user registrations
- authentication (login) events
- in-app purchase revenue
- A/B test group assignments

### Data availability in this repository

Due to GitHub file size limits, **full raw authentication logs are not included in this repository**.

### Included in this repository:
- Cleaned and processed datasets used for analysis
- SQLite database containing all analysis views
- A small sample of raw authentication logs (for structure reference)

### Full dataset:
The complete raw dataset is available on Kaggle:

👉 https://www.kaggle.com/datasets/debs2x/gamelytics-mobile-analytics-challenge/data

This setup reflects common industry practices where:
- raw logs are stored in data warehouses
- analysts work on processed and aggregated datasets
- 
---

## 🛠 Tools Used

- **Python (pandas)** — data cleaning and preprocessing
- **SQLite** — cohort analysis, monetization metrics and A/B testing
- **Tableau Public** — dashboard creation and business storytelling

---

## 📌 Key Insights

- Retention drops significantly after Day 1 and stabilizes after Day 7
- Monetization is driven mainly by a small subset of high-spending users
- A/B test variant increased ARPPU but reduced payer rate, resulting in no ARPU improvement
- D7 retention shows almost no correlation with D30 LTV across cohorts, suggesting that early engagement alone does not predict long-term value

---

## 🎯 Why This Project

This project was built to demonstrate skills required for **Junior Data Analyst / LiveOps Analyst roles in the gaming and esports industry**, including:

- Cohort-based behavioral analysis
- Monetization KPI evaluation
- Experiment analysis
- Business-oriented data storytelling

---

## 👤 Author

Federico Mistretta 
Aspiring Junior Data Analyst / LiveOps Analyst (Gaming & Esports)

LinkedIn: https://www.linkedin.com/in/federico-mistretta/  
GitHub: https://github.com/your-username
