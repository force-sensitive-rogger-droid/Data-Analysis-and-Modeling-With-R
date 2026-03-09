# Multi-Source Data Analysis & Predictive Modeling with R

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Tidyverse](https://img.shields.io/badge/Tidyverse-v2.0.0-blue?style=for-the-badge)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-Random_Forest-green?style=for-the-badge)

## 📌 Project Overview
This project presents a comprehensive data analysis and predictive modeling workflow, divided into two distinct parts using different data sources (Open Data and Kaggle). 

The goal is to demonstrate proficiency in **Data Cleaning**, **Exploratory Data Analysis (EDA)**, and building **Machine Learning** models to derive actionable insights.

---

## 🚦 Part 1: Traffic Volume Analysis (SCATS)
Analysis of traffic flow data from the SCATS (Sydney Coordinated Adaptive Traffic System) in Dun Laoghaire-Rathdown, Ireland, for November 2022.

* **Source:** [data.gov.ie](https://data.gov.ie/dataset/traffic-volumes-from-scats-traffic-management-system-2022)
* **Key Features:** Analysis of hourly traffic volume, identification of peak hours, and geographical distribution across detectors.
* **Techniques:** Data transformation with `dplyr`, time-series manipulation, and trend visualization using `ggplot2`.

---

## 🎮 Part 2: Twitch Streamer Trend Prediction
Predictive modeling on the "Top 1000 Twitch Streamers" dataset (May 2024).

* **Source:** [Kaggle](https://www.kaggle.com/datasets/hibrahimag1/top-1000-twitch-streamers-data-may-2024)
* **Modeling Objectives:**
    1.  **Classification:** Predicting the Streamer Type (Esports vs. Personality).
    2.  **Regression:** Predicting the `Average Stream Duration`.
* **Algorithm:** Random Forest (via the `caret` package).
* **Highlights:** Variable Importance analysis, Confusion Matrix evaluation, and hyperparameter tuning (`ntree` optimization).

---

## 🛠️ Tools & Technologies
* **Language:** R
* **Core Packages:** * `tidyverse` (ggplot2, dplyr, tidyr) for processing and visualization.
    * `caret` & `randomForest` for machine learning.
    * `scales` for professional data formatting.
* **Environment:** Quarto (.qmd) for reproducible reporting and PDF generation.

---

## 📊 Key Insights
* **Traffic Flow:** Identified distinct morning and afternoon rush hour patterns consistent with local commuting behaviors.
* **Twitch ML:** * `Followers Gained` and `Total Views` were identified as the strongest predictors for streamer classification.
    * A Random Forest model with 50 trees provided the best balance between accuracy and generalization, effectively handling categorical noise.

---

## 🚀 How to Run
1. Ensure you have R and RStudio installed.
2. Install the required packages:
   ```r
   install.packages(c("tidyverse", "caret", "randomForest", "mlbench"))
