# Urban Mobility & Traffic Flow Analysis: Dublin City Insights

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Tidyverse](https://img.shields.io/badge/Tidyverse-v2.0.0-blue?style=for-the-badge)
![Data_Viz](https://img.shields.io/badge/Visualization-ggplot2-orange?style=for-the-badge)

## 📌 Project Overview
This project explores urban mobility patterns in Dublin, Ireland, by analyzing large-scale datasets from the **DublinBikes** sharing scheme and **SCATS** traffic management sensors. 

The analysis focuses on identifying temporal trends, peak usage periods, and the correlation between bike availability and city traffic flow, providing a data-driven perspective on urban transportation dynamics.

---

## 🚲 Part 1: DublinBikes Usage Patterns
A deep dive into the bike-sharing ecosystem to understand how citizens move through the city.

* **Dataset:** Historical DublinBikes occupancy and station data.
* **Analysis Focus:** * Identifying the busiest bike stations (e.g., Smithfield, Parnell Square).
    * Temporal analysis (Hourly, Daily, and Monthly trends).
    * Impact of weekdays vs. weekends on bike availability.
* **Key Visualizations:** Heatmaps of bike demand and interactive time-series plots.

---

## 🚗 Part 2: SCATS Traffic Flow Analysis
Analysis of traffic volumes captured by the SCATS system to map the "pulse" of the city.

* **Source:** [data.gov.ie](https://data.gov.ie/) (Dublin City Council Open Data).
* **Technical Workflow:**
    * Extensive data cleaning and merging of multiple sensor CSV files.
    * Aggregation of traffic counts by site and hour.
    * Identifying "Rush Hour" bottlenecks and traffic distribution across key junctions.

---

## 🛠️ Tech Stack & Methodology
* **Language:** R
* **Key Libraries:** * `tidyverse` (dplyr, ggplot2, tidyr) for robust data wrangling.
    * `lubridate` for complex date-time manipulations.
    * `scales` & `gridExtra` for professional-grade plotting.
* **Data Processing:** Handling large CSV files, managing missing values, and normalizing time-stamps for cross-dataset comparison.

---

## 📊 Key Findings
* **Mobility Peak:** Bike usage shows a strong "dual-peak" distribution (08:00-09:00 and 17:00-18:00), aligning perfectly with typical commuting hours.
* **Station Dynamics:** Certain stations act as "drains" (bikes are removed in the morning) while others act as "sources," highlighting the need for efficient bike redistribution strategies.
* **Traffic Correlation:** Traffic volume peaks slightly precede bike usage peaks, suggesting a shift in transport mode preference during heavy congestion periods.

---

## 🚀 How to Use
1. Clone this repository.
2. Ensure the raw data files (CSV) are placed in the `/data` directory.
3. Open the `Dublin_Mobility_Analysis.qmd` file in RStudio.
4. Run `Render` to generate the full PDF report.

---
**Author:** Charalampos Sarakatsanis  
**Context:** Data Programming with R - Assignment 2
