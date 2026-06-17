# optimization-of-finance-and-marketing-expenses
Showz, an event ticketing platform, is experiencing optimization challenges within its marketing department.
# Showz: Marketing Expenditure Optimization & Cohort Analysis

## 📌 Project Overview

### 🔍 Problem
Showz, an event ticketing platform, is experiencing optimization challenges within its marketing department. While acquiring users across multiple advertising channels, the company lacks clear visibility into the return on investment of its marketing spend. The primary challenge is to analyze server logs, order history, and marketing costs from January 2017 to December 2018 to pinpoint exactly which user acquisition channels are highly profitable, how long users take to convert, and when the company recovers its customer acquisition costs.

### 🛠️ What I Did (Step-by-Step)

1. **Data Optimization & Cleaning (Data Wrangling):**
   * Imported web visits, user orders, and marketing expenditure datasets using **Pandas**.
   * Converted date-time strings into proper `datetime64` structures and validated the integrity of unique identifiers (`Uid`, `Source Id`) to avoid calculation biases.

2. **User Engagement & Cohort Analysis (EDA):**
   * Calculated core product metrics including **DAU, WAU, and MAU** to analyze platform traffic stability.
   * Monitored **Average Session Length (ASL)** and mapped user retention dynamics (**Retention Rate**) across different cohorts.

3. **Conversion Tracking & Customer Lifetime Value (LTV):**
   * Grouped users into monthly cohorts based on registration dates to calculate the exact conversion window (e.g., `Conversion 0d`, `1d`) from registration to purchase.
   * Calculated purchase frequency, average purchase size (ticket price), and cumulative **Lifetime Value (LTV)** per cohort over time.

4. **Marketing Spend & Profitability Analysis:**
   * Calculated **Customer Acquisition Cost (CAC)** for each specific marketing channel (`Source Id`).
   * Evaluated marketing channel efficiency by computing the **Return on Marketing Investment (ROMI)** to locate the exact month a cohort reaches its financial breakeven point.
   * Segmented behavioral and financial performance by **Device type** (Desktop/Mobile) and ad sources using **Matplotlib/Seaborn** visualizations.

### 📋 Operational Impact & Decision Matrix

This analysis transitions raw server data into an executive decision framework for marketing leadership:
* **Resource Allocation Matrix:** Ranks marketing platforms by comparing their **CAC vs. LTV**. This allows the marketing team to immediately see which channels yield long-term valuable clients and which ones drain resources.
* **Device-Based Strategy:** Identifies whether desktop or mobile user segments yield a higher conversion velocity, preventing waste on underperforming responsive interfaces.
* **Breakeven Timeline:** Gives stakeholders a predictable timeline of when a specific ad-dollar investment turns profitable, safeguarding the company's monthly cash flow.

### 🚀 Key Results

* **Optimized Marketing Spend:** Identified high-CAC, low-ROMI acquisition channels, allowing a data-driven recommendation to reallocate budget toward top-performing ad sources.
* **Cohort Conversion Insights:** Pinpointed the exact behavioral timeline of the highest-converting user cohorts, streamlining customer retention strategies.
* **Data-Backed Recommendations:** Delivered an end-to-end Jupyter Notebook utilizing business metrics (**LTV, CAC, ROMI**) that serves as an executive playbook for future marketing investment strategy.
