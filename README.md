
# 🚴‍♂️ Bike Buyers Analysis — Power BI Dashboard

## Executive Summary

This project delivers a **professional two-page Power BI dashboard** analyzing bike buyer demographics and purchasing behavior. Using a dataset of **1,000 customers**, the dashboard reveals **who buys bikes and why**, comparing **buyers vs non-buyers** across **income, age, education, region, commute distance, and family size**.

Key findings show that **middle-aged professionals with higher incomes and shorter commutes** are the most likely to purchase bikes, while purchase likelihood decreases with more children. These insights directly inform **marketing strategy, product targeting, and regional expansion opportunities**.

👉 This repository includes:

* The **Power BI `.pbix` file** (full dashboard).
* A **PowerPoint summary deck** prepared for **executive review**.
* Screenshots of the dashboards (`Overview` & `Demography`).

---

## Introduction

The dataset was obtained from the **Bike Buyers Dataset** on Kaggle. It is a **simulated dataset** that mirrors real-world sales and customer demographic information, commonly used for analytical and visualization practice.

This project forms part of my **professional Data Analyst portfolio** and demonstrates how to turn raw customer data into meaningful insights using **Power BI, DAX, and analytical storytelling**.

---

## Project Description

This project centers on building a **two-page interactive Power BI dashboard** that provides a clear picture of customer behavior in bike purchases. It identifies **key buyer segments** and helps businesses understand how **income, demographics, commute, and lifestyle** influence purchase decisions.

The dashboard is designed to be **management-ready**: visually intuitive, interactive, and structured to answer strategic business questions in seconds.

---

## Project Context

Organizations often struggle to understand **which customers are most likely to purchase bikes**. Without data-driven insights, marketing strategies remain broad, inefficient, and costly.

By applying **business intelligence techniques** to customer data, this project provides actionable insights that can:

* Reduce wasted marketing spend.
* Improve buyer targeting.
* Increase overall bike sales.

➡️ You can view the project here: **[Insert published Power BI report link once hosted]**

---

## Problem Statement

The company lacks **clear, data-backed insights** into who its bike customers are. Without this knowledge, resources are misallocated, and sales growth opportunities are missed.

Specifically:

* Which **age groups, income brackets, and occupations** are most likely to buy bikes?
* How do factors like **region, commute distance, and family size** affect purchases?
* What customer profiles should the company prioritize for **marketing and sales campaigns**?

This project addresses these questions by analyzing the dataset and creating a **comprehensive Power BI dashboard**.

---

## Aim of the Project

The project aims to:

* Identify **demographic and economic factors** influencing bike purchases.
* Compare **buyers vs non-buyers** on income, family size, and commute distance.
* Create an **interactive and professional Power BI dashboard** with executive-ready visuals.
* Provide **strategic recommendations** to increase sales and improve customer targeting.
* Showcase **technical, analytical, and storytelling skills** for my professional portfolio.

---

## My Approach

### 🔹 Data Cleaning Checklist

* Loaded the `Bike_Buyer` dataset with the following fields:
  `ID, Marital Status, Gender, Income, Children, Education, Occupation, Home Owner, Cars, Commute Distance, Region, Age, Purchase Bike`.
* Removed blank spaces and standardized categorical values (e.g., `M` → `Male`, `F` → `Female`).
* Checked and corrected **data types**.
* Created **age and income bins** for better segmentation.
* Removed duplicates and missing values.

**Context:**

* Rows before cleaning: **1,027**
* Rows after cleaning: **1,000**

---

### 🔹 Modelling & Engineering

Since this was a **flat table dataset**, advanced modeling was not required. Steps included:

1. Data load and transformation.
2. Normalization and categorical cleaning.
3. Exploratory Data Analysis (EDA).
4. Creation of **DAX measures** for KPIs.
5. Dashboard visualizations with custom theme.
6. Navigation buttons for a professional user experience.

---

## Analysis / Work Done

### 🔹 Key DAX Measures

```DAX
Total Buyers =
CALCULATE(COUNTROWS('BikeData'), 'BikeData'[Purchased Bike] = "Yes")

Total Non-Buyers =
CALCULATE(COUNTROWS('BikeData'), 'BikeData'[Purchased Bike] = "No")

Purchase Rate (%) =
DIVIDE([Total Buyers], [Total Buyers] + [Total Non-Buyers], 0) * 100

Avg Income Buyers =
CALCULATE(AVERAGE('BikeData'[Income]), 'BikeData'[Purchased Bike] = "Yes")

Avg Income Non-Buyers =
CALCULATE(AVERAGE('BikeData'[Income]), 'BikeData'[Purchased Bike] = "No")
```
These measures were critical for building **KPI cards** and comparative visuals.

---

## Analysis Processes

* **Data Collection & Cleaning** (Excel, Power BI).
* **Exploratory Data Analysis (EDA)** for trends.
* **KPI Calculation** (Buyers, Non-Buyers, Purchase Rate, Avg Income).
* **Visualization**: Two-page Power BI dashboard with interactive slicers.
* **Insight Extraction**: Interpreted visuals to address the problem statement.
* **Recommendations**: Business strategies drawn from the data.

---

## Skills & Tools Used

* **Excel** — Initial exploration and checks.
* **Power BI** — Dashboard creation, slicers, cross-filtering.
* **DAX** — Measures for KPIs and advanced calculations.
* **Business Knowledge** — Translating patterns into strategies.
* **Analytical Storytelling** — Communicating insights clearly.

---

## KPIs Tracked

* **Total Buyers**: 481
* **Total Non-Buyers**: 519
* **Purchase Rate (%)**: 48.1%
* **Avg Income (Buyers)**: 58K
* **Avg Income (Non-Buyers)**: 54.9K

---

## Key Features

* **Two-page interactive dashboard**: Overview & Demography.
* **Executive-friendly visuals**: KPI cards, donut charts, bar/line graphs.
* **Slicers & filters** for dynamic exploration.
* **Custom color theme** (blue = buyers, orange = non-buyers).
* **Navigation buttons** for seamless report flow.
* **Export-ready insights** for management presentations.

---

## Recommendations

1. **Target middle-aged professionals** — the largest buyer group.
2. **Expand marketing in the Pacific region**, which has higher buyer share.
3. **Highlight short-distance commuting** benefits (0–1 mile commuters show higher adoption).
4. **Segment by income**:

   * Affordable models for 10–50k earners.
   * Premium options for 60–100k+ customers.
5. **Offer family packages or promotions** to offset declining purchases in larger families.

---

## Final Note

This project highlights the **power of BI dashboards** in delivering business-critical insights.

The repository includes:

* **Power BI `.pbix` file** (full interactive dashboard).
* **PowerPoint summary deck** created for **executive review**.
* Dashboard screenshots (Overview & Demography).

These files demonstrate both **technical skills (data cleaning, DAX, visualization)** and **business acumen (recommendations, strategy alignment)**.

---

## Contact

👤 **Your Name** — Data Analyst
📧 Email: [Your email here]
🔗 LinkedIn: [Your LinkedIn profile here]
🌐 Portfolio: [Your website here]

---

✅ Now this README is **executive-ready**, comprehensive, and polished.

Would you like me to also **draft the Executive PowerPoint deck outline** (like 5–7 slides: KPIs, key insights, recommendations) so it aligns perfectly with this README? That way your `.pbix`, README, and PowerPoint tell one consistent story.
