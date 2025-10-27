# EV Market Analysis for AtliQ Motors India
<img width="1015" height="561" alt="image" src="https://github.com/user-attachments/assets/400d7e61-6ca4-4f96-a0ec-9c3ab7f7b3ce" />


## Project Overview

This project presents a **Business Intelligence (BI) dashboard** designed to analyze the Electric Vehicle (EV) market in India for AtliQ Motors, a US-based automotive company planning expansion into the Indian market. The dashboard provides insights into sales growth, top-performing states and manufacturers, EV penetration, and market trends to support data-driven strategic planning for AtliQ's market entry.

---

## Objectives

The main objectives of this BI project were to:

* Analyze EV sales growth in India from 2021 to 2024.
* Identify the top-performing states and manufacturers in the EV segment.
* Measure EV penetration and CAGR across vehicle categories.
* Project potential future EV sales (2030) based on historical trends.
* Provide actionable insights and recommendations for AtliQ Motors' market entry strategy.

---

## Problem Statement

AtliQ Motors, holding a significant market share (25%) in North America's EV segment, sought to expand into India where their share is currently less than 2%. Before launching models, the company required a detailed market study to understand the existing EV/Hybrid landscape, growth trends, key players, and regional performance in India.

---

## Dataset Information

The analysis utilized datasets covering EV and total vehicle sales, along with dimension tables for time and vehicle category:

| Table Name                          | Description                                                                 | Key Fields Used                          |
| :---------------------------------- | :-------------------------------------------------------------------------- | :--------------------------------------- |
| `electric_vehicle_sales_by_state`   | Tracks EV and total vehicle sales across states, dates, and categories.     | date, state, electric\_vehicles\_sold, total\_vehicles\_sold, vehicle\_category |
| `electric_vehicle_sales_by_makers`  | Captures sales performance by manufacturer, vehicle type, and time.         | date, maker, electric\_vehicles\_sold, vehicle\_category |
| `dim_date`                          | Date dimension enabling time-based filtering (fiscal year, quarter).        | date, fiscal\_year, quarter              |
| `Vehicle_Category_Table`            | Defines vehicle categories (2-Wheeler, 4-Wheeler) for consistent filtering. | vehicle\_category                        |

**Data Cleaning:** The data was validated for consistency, positive sales figures, correct date mapping, and absence of missing values or duplicates.

---

## Technology Stack

| Component                  | Tool / Language               |
| :------------------------- | :---------------------------- |
| Data Cleaning & Processing | Power Query                   |
| Calculations               | DAX (Power BI)                |
| Visualization / Dashboard  | Power BI                      |
| Documentation              | Markdown (README), Word       |

---

## Power BI Data Model Overview

<img width="932" height="485" alt="image" src="https://github.com/user-attachments/assets/b15df098-e26e-4e4a-beb7-3b38cd3ec445" />


The model uses a star schema linking the two fact tables (`sales_by_state`, `sales_by_makers`) to the dimension tables (`dim_date`, `Vehicle_Category_Table`). This structure enables efficient slicing and dicing of data by time, geography, vehicle type, and manufacturer.

---

## Key DAX Measures

Several DAX measures were created to drive the analysis:

* **EV Penetration Rate:** Calculates the percentage of total vehicle sales that are electric.
* **CAGR (Compound Annual Growth Rate):** Shows the average annual growth rate of EV sales.
* **Projected EV Sales (2030):** Uses current sales and CAGR to forecast future potential.

---

## Key Insights (from Dashboard)

* **Market Size & Growth:** India's EV market penetration is currently low (**3.61%**) but growing rapidly. Projected sales could reach **80M by 2030**.
* **Category Dominance:** **2-Wheelers** account for **92.6%** of all EV sales, highlighting strong demand for affordable electric mobility.
* **Geographical Concentration:** The top 3 states (**Maharashtra, Karnataka, Tamil Nadu**) contribute over **50%** of total EV sales.
* **Top Manufacturers:** **Ola Electric** leads the market (**23.7%** share), followed by TVS and Ather, primarily in the 2-wheeler segment. There is a noticeable gap in major 4-wheeler manufacturers among the top players.
* **Seasonality:** EV sales peak in **Q1 (Jan-Mar)** and **Q4 (Oct-Dec)**, potentially linked to festive seasons and financial year-end activities.

### Executive Summary
<img width="1017" height="556" alt="image" src="https://github.com/user-attachments/assets/448788c5-a9f1-4695-bbc3-a5a9f8b85a6b" />

### Market analysis by state
<img width="1013" height="560" alt="image" src="https://github.com/user-attachments/assets/f825f50f-50aa-4a79-ad2f-c52b258ce36d" />

Market analysis by manufacture
<img width="1002" height="556" alt="image" src="https://github.com/user-attachments/assets/b5d2e819-5d25-4679-babf-7e0e4d33bbf6" />

Detailed analysis by vehicle category
<img width="1010" height="561" alt="image" src="https://github.com/user-attachments/assets/9e2a0776-ce82-4354-a4e6-0d757d8d55d3" />

Detailed sales analysis
<img width="1029" height="562" alt="image" src="https://github.com/user-attachments/assets/2eba3575-c307-4c48-9a1b-71862ffa0d5b" />

---

## Recommendations for AtliQ Motors

1.  **Prioritize 2-Wheelers:** Launch affordable, high-range 2-wheeler models first to compete directly with market leaders like Ola and TVS.
2.  **Target Key States:** Focus initial market entry efforts on Maharashtra, Karnataka, and Tamil Nadu due to their high EV adoption rates.
3.  **Address the 4-Wheeler Gap:** Plan a subsequent launch of premium 4-wheeler EVs (SUVs/sedans) to capture the less competitive, but growing, segment.
4.  **Strategic Timing:** Align product launches and marketing campaigns with peak sales seasons (Q1 and Q4).
5.  **Competitive Edge:** Leverage AtliQ's US reputation and focus on differentiating factors like battery life, charging speed, or pricing.

---

## Conclusion

India's EV market offers a significant growth opportunity for AtliQ Motors. A phased approach, starting with competitive 2-wheelers in key regions and followed by strategic entry into the 4-wheeler segment, positions AtliQ for success in capturing market share in this rapidly expanding sector.
