# 📦 Kaizen Gaming Case Study – Technical Assessment

This repository contains the complete analysis for the **Kaizen Gaming Data Challenge**, structured in two independent parts:

* **Task 1:** Sportsbook Performance + CRM Level Analysis
* **Task 2:** Impact of Real-Time Validation in the Registration Form (Mexico)

All analyses were performed using **Python (Google Colab)**. Outputs are delivered in both **CSV** and **Excel (.xlsx)** formats with cleaned, typed, and formatted datasets ready for stakeholder review.

---

## 📊 Task 1 – Betting Performance and Customer CRM Insights

### Overview

The first part of the challenge analyzes **sports betting performance** across competitions and correlates that with **CRM level evolution** and **new customer behavior**.

The goals were to:

* Understand which competitions generate the most value
* Track CRM level distribution by month
* Analyze CRM levels among newly acquired customers

### Methodology

1. Imported and cleaned the following data:

   * `Sportbook.txt`: Betting transactions
   * `CRM Level.csv`: Monthly CRM levels
   * `Registrations.csv`: Customer registration date

2. Built 3 main analytical tables:

   * KPIs per competition
   * CRM levels per month
   * CRM levels of newly registered customers

3. Created one strategic visualization:

   * **Top 10 Competitions by Avg. Customer Value**

### Key Insights

* 🥇 Competitions like *Germany* and *EURO 2020* drive the highest average value per customer
* 🧱 CRM level data reveals structural changes over time in customer segmentation
* 🧲 Most new customers start in lower CRM levels, suggesting room for growth

### Files (Task 1)

* `task1_analysis.ipynb`: Google Colab Python notebook
* `avg_customer_value_chart.png`: Strategic line chart

#### Generated KPIs and tables in both CSV and XLSX

| Filename                             | Description                               |
| ------------------------------------ | ----------------------------------------- |
| `kpi_by_competition.*`               | Summary of betting metrics by competition |
| `crm_level_by_month.*`               | Unique customers by CRM level and month   |
| `crm_level_by_month_new_customers.*` | New customers by CRM level and month      |

All datasets:

* Dates formatted as `yyyy-mm`
* Currency in euros (EUR)
* Customer counts as integers

---

## 🧪 Task 2 – Registration Form Change Impact (Mexico)

### Overview

This analysis was based on a stakeholder request from the **Mexico Country Manager**, following a **drop in email registrations** after the addition of a **real-time validation field** on the registration form (16/09).

Objectives:

1. Determine if drop-off increased after the change (Google Analytics)
2. Assess whether the **quality** of registered users improved (Deposits)
3. Estimate the **impact and potential losses** (Customer value vs drop)

### Methodology

1. Cleaned and joined the following tables:

   * `Customer.txt`, `Acquisition Channel.txt`
   * `Deposits.csv`, `Google_Analytics_data_202209.csv`

2. Segmented users into:

   * `before`: Registered prior to 16/09
   * `after`: Registered after the change

3. Three-step investigation:

   * Funnel analysis of **Registration Steps 1-4** via Google Analytics
   * First-time deposit comparison (FTD) across groups
   * Estimation of potential lost revenue

### Key Insights

* 📉 **Conversion rate** dropped from 130% to 110%, suggesting increased friction
* 💸 Average deposit **increased** post-change, indicating higher quality
* 📊 Potential **lost revenue is non-trivial**, but may be offset by better retention

### Files (Task 2)

| Filename                       | Description                                     |
| ------------------------------ | ----------------------------------------------- |
| `task2_analysis.ipynb`         | Python notebook for Task 2 analysis             |
| `pivot_registration_steps.csv` | Drop-off data by GA registration steps          |
| `ftd_summary_by_group.csv`     | Deposit quality metrics before vs after         |
| `impact_estimation.csv`        | Modeled revenue loss due to fewer registrations |

---

## 🔧 Tools Used

* Python 3 (pandas, matplotlib, xlsxwriter)
* Google Colab (for processing and delivery)
* Google Analytics (behavioral funnel data)

---

## ✅ Delivery Notes

All datasets are:

* Cleaned and deduplicated
* Typed and formatted (dates, currency, integers)
* Exported in both `.csv` and `.xlsx` where relevant

All visuals and analyses are reproducible within the provided `.ipynb` notebooks.

Feel free to reach out if you would like dashboard versions in **Looker Studio**, which can be built using the same CSVs.

---

Prepared by: **Felipe Corrêa**
Assessment for: **Kaizen Gaming** – Data Challenge (2025)
