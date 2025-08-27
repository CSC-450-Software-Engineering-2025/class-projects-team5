# Kittelson Financial Forecasting Tool

## Purpose
The **Kittelson Financial Forecasting Tool** is a **web-based, interactive financial planning and forecasting platform**.  
It provides a **rolling 12-month projection** and a **year-end projection** with outputs including:

- Accrual Operating Income  
- Audited Overhead Rate  
- Available Bonus Pool  
- Year-End Cash Balance  
- Estimated Taxable Income  
- Shareholder Book & Goodwill Balances  

The tool is designed as a **decision support system** that enables leadership to manage the complex and sometimes conflicting priorities of financial stewardship, regulatory compliance, and employee rewards.

---

## Strategic Objectives
- **Cash Reserve Protection** – Maintain at least breakeven cash.  
- **Overhead Rate Management** – Balance cost recovery with DOT expectations of “reasonableness.”  
- **Tax Efficiency** – Minimize firm-wide tax burden through shareholder tax dividends.  
- **Staff Recognition** – Provide a performance-based bonus pool that reflects firm success.  
- **Shareholder Valuation Growth** – Support long-term increases in book and goodwill balances.  

---

## System Context Overview

**Components**
- **Accounting ERP (Deltek Vantagepoint):** Source for actuals (income, overhead, cash, etc.).  
- **Data Storage & Processing (Power BI Dataflows, Azure SQL, or similar):** Repository for data, aggregation, and forecasting logic.  
- **Accounting Interface (Web-based in-house tool):** Inputs, comparisons, and visualizations.  
- **End User Visualization Platform (Web + Power BI integration):** Dashboards for summarized outputs and scenario analysis.  

**Data Flow**
1. Ingestion of actuals from Deltek to BI database.  
2. User inputs:  
   - **Accounting:** Full variable access via entry tool.  
   - **Pulse:** Limited variable access via dashboards.  
3. Processing through the forecast engine.  
4. Outputs visualized via dashboards (interactive, export-ready).  

**User Roles**
- **Accounting/Data Analyst:** Full access and transparency.  
- **Pulse:** Summary-level access with limited control (utilization, multiplier, staff adds).  
- **Board:** Read-only summaries without scenario control.  

---

## Functional Requirements

**Data Ingestion**
- Extract actuals from ERP into BI database (ETL).  
- Manual entry forms for assumptions.  
- Scenario “locking” for historical comparison.  

**Forecast Modules**
- Rolling 12-month and year-end forecasts.  
- Scenario management (Base, Optimistic, Pessimistic).  
- Key outputs: Accrual Operating Income, Bonus Pool, Overhead Rate, Taxable Income, Dividends, Book & Goodwill, Ending Cash Balance.  

**Reporting**
- Outputs include accrual income, cash balance, bonus pool, dividends, and valuations.  
- Historical and forecasted trend analysis.  

---

## Approach & Timeline (Agile)

1. **Planning & Requirements** – Functional spec, ETL plan, Power BI capabilities, alignment with financial model.  
2. **Accrual Operating Income Modeling** – Baseline rolling forecast, driver-based methodology, historical datasets.  
3. **Overhead Rate Forecasting** – Forecasting tied to income scenarios, eventual integration with bonus inputs, visuals.  
4. **Accrual-to-Cash + Taxable Income + Bonus Modeling** – Cash conversion, forecasted taxable income/dividends, bonus pool levels.  
5. **Book & Goodwill Valuation + Ending Cash** – Forecasted valuations, ending cash balance, scenario visualizations.  
6. **Testing & Refinement** – Dual-run manual vs. system, alignment with Kittelson’s financial model, feedback, and enhancements.  

---

## Security & Access
- Initial access limited to 3 roles (Accounting, Pulse, Board).  
- Future: Role-based access controls.  

---

## Summary
This tool will enable **self-service forecasting** with both detailed and high-level controls.  
By combining **driver-based modeling, AI/ML forecasting logic, and scenario analysis**, it will help leadership and staff balance **financial sustainability, compliance, and performance recognition**.  
