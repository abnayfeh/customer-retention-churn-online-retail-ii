# Customer Retention & Churn Analysis — Online Retail II

This project analyzes **customer churn, retention, and revenue dynamics** using transactional e-commerce data from the **Online Retail II** dataset.  
The goal is to understand **how customer retention evolves over time**, how it differs from **revenue retention**, and where churn risk is highest in the customer lifecycle.

The analysis follows an end-to-end analytics workflow using **Python, SQLite, and Tableau**, resulting in an executive-style dashboard suitable for business stakeholders.

**Dataset Used:** https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci
---

## 🔍 Project Overview

**Key questions addressed:**
- How quickly do customers churn after their first purchase?
- How does customer retention differ from revenue retention over time?
- When in the customer lifecycle is retention most critical?
- Do retained customers expand revenue even as customer counts decline?

**Churn definition:**  
A customer is considered **churned** if they are inactive for **90 consecutive days**.


---

## 📊 Dashboard

**Tableau Public:**  
👉 https://public.tableau.com/app/profile/abdo.nayfeh/viz/OnlineRetailII-ChurnAnalysis/Dashboard

**Dashboard features:**
- Customer retention heatmap (monthly cohorts)
- Revenue retention heatmap (normalized to first purchase month)
- Monthly churn rate over time
- Executive KPIs (3-, 6-, 12-month retention; repeat customer rate)
- Business insight annotations

<img width="1221" height="697" alt="Screenshot 2026-01-07 at 1 07 50 PM" src="https://github.com/user-attachments/assets/e22b5c0e-3aa4-4ce5-b17f-4458c97065be" />

---

## 🧠 Analytical Approach

### 1️⃣ Data Preparation (Python)
- Cleaned raw transactional data (Online Retail II Dataset Link at -> https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci
- Filtered invalid transactions and cancellations
- Parsed dates and computed revenue fields
- Exported a clean, analysis-ready transactions table

### 2️⃣ Customer & Cohort Modeling (SQLite)
- Aggregated invoice-level records into **customer-level features**
- Defined churn windows (90-day inactivity rule)
- Built monthly **cohort retention tables**
- Computed **customer retention** and **revenue retention** metrics
- Generated churn-over-time tables

### 3️⃣ Visualization & Insights (Tableau)
- Built cohort heatmaps for customer and revenue retention
- Created churn trend line and executive KPIs
- Compared customer vs revenue retention behavior
- Added business-oriented insights and annotations

---

## Key Insights

- 📉 **Customer churn is highest in the first 3–6 months** after acquisition, after which retention stabilizes.
- 💰 **Revenue retention consistently outperforms customer retention**, indicating higher spend among retained customers.
- 🔁 **Repeat customers contribute disproportionate revenue**, offsetting losses from early churn.
- 📊 **Monthly churn rates decline over time**, suggesting improving customer quality or engagement.


