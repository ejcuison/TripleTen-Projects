# Ecommerce User Analysis

![image alt](https://github.com/ejcuison/TripleTen-Projects/blob/95c9c55bb7a9d31d06f9b384e6b5585e9942a8f1/Ecommerce%20User%20Analysis/Conversion%20Funnel.png)
![image alt](https://github.com/ejcuison/TripleTen-Projects/blob/93ee1631d0fbee9f9c8479b65a512ace35a6ec4b/Ecommerce%20User%20Analysis/Retention%20Rates.png)
![image alt](https://github.com/ejcuison/TripleTen-Projects/blob/4e53e1f353cf3c010356556db5a08dac59661f8b/Ecommerce%20User%20Analysis/Cohort%20Analysis.png)

This project analyzes user behavior on an ecommerce website using funnel analysis and cohort retention modeling in Excel/Google Sheets. The goal is to understand user engagement, retention trends, and overall conversion performance.

## 📊 Project Overview

**Objectives:**
- Create a conversion funnel to understand user behavior
- Build acquisition cohorts based on users' first purchase month
- Calculate retention rates by cohort and analyze patterns
- Provide a clear, executive-level summary of findings

**Data Source:**  
`BusinessAnalyticsProject.xls` – raw user activity data

**Tools Used:**  
Google Sheets / Microsoft Excel

---

## ⚙️ Steps & Methodology

1. **Conversion Funnel Creation**
   - Built a pivot table using `raw_user_activity`
   - Added columns for overall and step-by-step conversion rates

2. **Purchase Filtering**
   - Filtered only "purchase" events
   - Created a `purchase_activity` sheet with relevant data

3. **First Purchase Identification**
   - Pivot table to find each user's first purchase date
   - Used `VLOOKUP()` to add `first_purchase_date` to user rows

4. **Cohort Grouping**
   - Added `event_month`, `first_purchase_month`, and `cohort_age` columns
   - Used `TEXT()` and `DATEDIF()` for time transformations

5. **Cohort Analysis**
   - Built a pivot table grouped by `first_purchase_month`
   - Counted unique users per `cohort_age`

6. **Retention Rate Calculation**
   - Created a `retention_rates` sheet
   - Used formulas to calculate month-over-month retention by cohort

7. **Executive Summary & Organization**
   - Added insights and visuals to an `Executive Summary` sheet
   - Ordered tabs logically for easy navigation
   - Cleaned up formatting for readability

---

## 📈 Key Results & Insights

- **Conversion Funnel:**
  - ~30% of users reach the shopping cart page
  - ~36% of those users complete a purchase

- **Retention Trends:**
  - Highest retention seen in the September 2020 cohort
  - Retention rates declined for cohorts from Oct–Dec 2020
  - Starting January 2021, Month 1 retention showed slight improvement

---

## 🧠 Conclusion & Recommendations

- Focus on replicating elements of the September 2020 user experience to improve retention.
- Investigate what changed in Jan 2021 that led to a rise in Month 1 retention—could inform future strategy.
- Continue monitoring retention trends using updated cohort models to guide marketing and product decisions.

---


