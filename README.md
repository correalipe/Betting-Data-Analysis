# 📊 Task 1 – Betting Performance and Customer CRM Insights

## Overview

This project analyzes **sportsbook betting performance** across different competitions, correlating it with **customer CRM levels** and registration cohorts.

The goals were to:
- Understand which competitions generate the most value
- Track CRM level evolution over time
- Evaluate CRM levels among newly acquired customers

All calculations were performed using **Python (Colab)**, and outputs are delivered in both **CSV** and **formatted Excel (.xlsx)** files for stakeholder use.

---

## Methodology

1. Cleaned and transformed the following input files:
   - `Sportbook.txt`: Betting transactions
   - `CRM Level.csv`: Monthly CRM levels per customer
   - `Registrations.csv`: Customer registration dates

2. Generated 3 core analytical tables:
   - KPIs by competition
   - Monthly CRM level distribution
   - CRM levels among new customers (by registration month)

3. Created a strategic chart:  
   - **Top 10 competitions by average value per customer**

---

## Key Insights

- 💶 Certain competitions (e.g., Germany, EURO 2020) stand out for high **average customer value**.
- 📈 The CRM level distribution reveals the **evolution of user engagement** across months.
- 🧲 Most **new customers** start in lower CRM levels, providing a benchmark for growth and nurturing.

---

## Files

- `task1_analysis.ipynb`: Full Python notebook (Google Colab-compatible)
- `avg_customer_value_chart.png`: Optional visualization (top 10 competitions)

### Generated KPIs and analytics tables in both **CSV** and formatted **Excel (.xlsx)**:

All datasets are clean and structured. Dates are formatted as `yyyy-mm`, monetary values as euros, and customer counts are treated as integers.

| Filename | Description |
|----------|-------------|
| `kpi_by_competition.*` | Summary of key betting metrics by competition |
| `crm_level_by_month.*` | Unique customers by CRM level and month |
| `crm_level_by_month_new_customers.*` | New customers by CRM level and month |

---

## Tools Used

- **Python** (pandas, matplotlib, xlsxwriter)
- **Google Colab** for collaborative and cloud-based development
- Optional integration with **Looker Studio** for dashboards (not included here)
