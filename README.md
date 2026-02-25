# 🏗 Operational Mining Monitoring Dashboard (H+1 Reporting)

## 📖 Background

This project is a recreation inspired by the first operational dashboard I built during my time in the mining industry.

At that time, daily operational reporting was largely spreadsheet-based and structured for manual reading. I was given the opportunity to help translate that reporting process into a centralized monitoring dashboard used for daily H+1 operational briefings.

This project marked the point where I shifted from thinking in spreadsheets to thinking in systems.

---

## 🎯 Objective

To transform manual operational reporting into a structured monitoring dashboard that answers critical daily questions:

- Are we building or depleting stock?
- Is dispatch exceeding production?
- Is ore quality within marketable thresholds?
- Which pit contributes most to stock movement?

The dashboard is designed for **H+1 reporting**, meaning it presents yesterday’s operational performance.

---
## 📷 Dashboard Preview
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/05246fa3-7440-48da-99ff-b7a17ee90c82" />

https://lookerstudio.google.com/reporting/fa39fa1f-57a2-430a-a044-fd883f47d707

---
## 📊 Key KPIs

### 🔹 Net Stock Change  
`Production − Stock Out`  
Primary indicator of daily stock movement.

---

### 🔹 Stock Flow Ratio  
`Stock Out / Production`

- > 100% → stock depletion  
- < 100% → stock build-up  

Provides quick visibility into stock flow balance.

---

### 🔹 Marketable %  
`(Medium + High Grade Stock) / Total Stock`

Measures proportion of commercially viable material.

---

### 🔹 Marketable Ton  
Total tonnage of Medium and High grade stock.

---

### 🔹 Weighted Average Ni  
`SUM(tonnage × Ni) / SUM(tonnage)`

Ensures ore grade is evaluated using tonnage-weighted logic.

---

## ⚙️ Technical Implementation

- Data structured and normalized in Google Sheets  
- Pivot-style operational report transformed into analyzable format  
- Blended data source (Production + Barging)  
- Join keys: `date` and `pit`  
- Calculated metrics created at chart level  
- Default dashboard mode: **Yesterday (H+1)**  
- Comparison mode: **Previous Period**

---

## 🎨 Design Principles

- Clean industrial theme
- KPI-first hierarchy
- Minimal color usage
- Clear operational focus
- Reduced visual noise

This dashboard prioritizes clarity and decision-support over visual complexity.

---

## ⚠️ Important Notes

- This project is a **recreation inspired by the original operational dashboard** I developed during my time at the company.
- It does **not fully replicate the original system**.
- Some components have been simplified or omitted, including:
  - Fleet monitoring
  - Loading tracking
  - Additional operational breakdowns
- The KPI logic reflects real operational concepts, but the implementation has been streamlined for portfolio purposes.
- All data used in this repository is **dummy data generated for demonstration purposes** and does not represent actual company figures.

---

## 🧠 Key Learnings

This project taught me:

- The difference between reporting and analytics
- Why structured data matters more than formatted spreadsheets
- How blending and aggregation errors can distort business insight
- The importance of defining KPI logic before building visuals

It shaped how I approach data today: structured, contextual, and decision-oriented.

---

## 🔄 If Rebuilt Today

- Move from spreadsheet to structured database (e.g., PostgreSQL)
- Automate ETL pipeline
- Add anomaly detection
- Implement alert-based monitoring
- Introduce role-based dashboard views

---

## 📌 Why This Project Matters

This was not just a dashboard.  
It was the starting point of my journey into building structured, reliable, and business-aligned data solutions.
