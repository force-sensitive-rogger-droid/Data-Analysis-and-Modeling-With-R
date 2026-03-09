# Bayesian Linear Regression & Predictive Inference using Stan

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Stan](https://img.shields.io/badge/Stan-MCMC-red?style=for-the-badge)
![Bayesian](https://img.shields.io/badge/Statistics-Probabilistic-blue?style=for-the-badge)

## 📌 Project Overview
This project implements **Bayesian Linear Regression** using **Stan**, a state-of-the-art platform for statistical modeling and high-performance statistical computation. The analysis focuses on estimating parameters for food expenditure data, utilizing **Markov Chain Monte Carlo (MCMC)** algorithms to sample from the posterior distribution.

By moving beyond simple point estimates, this project provides a full probabilistic view of regression coefficients, allowing for robust uncertainty quantification in economic forecasting.

---

## ⚙️ Bayesian Modeling with Stan
The project utilizes the `rstan` or `brms` interface to define and fit Bayesian models.

* **NUTS Sampler:** Leveraging the No-U-Turn Sampler (an advanced HMC algorithm) for efficient posterior sampling.
* **Convergence Diagnostics:** Evaluation of model fit using **R-hat** (Gelman-Rubin diagnostic), **Trace plots**, and **Effective Sample Size (ESS)**.
* **Prior Specification:** Defining weakly informative priors to regularize the model and improve convergence.



---

## 📈 Analytical Workflow
1. **Data Pre-processing:** Cleaning and scaling economic variables (Income, Household size).
2. **Model Definition:** Writing the Stan probabilistic program to relate Income to Food Expenditure.
3. **Posterior Analysis:** Extracting and visualizing the marginal posterior distributions for $\beta$ coefficients.
4. **Predictive Inference:** Generating **Posterior Predictive Checks (PPC)** to validate if the model's simulated data matches the observed data.

---

## 🛠️ Technical Stack
* **Language:** R
* **Probabilistic Programming:** **Stan** (via `rstan` or `brms` library).
* **Visualization:** `bayesplot` and `ggplot2` for diagnostic and result plots.
* **Reporting:** Quarto/RMarkdown for reproducible research.

---

## 📊 Business Insights
* **Reliability:** Unlike traditional regression, the Stan model provides a range of probable values for the impact of income, which is crucial for risk-averse financial planning.
* **Outlier Robustness:** Bayesian methods, particularly with appropriate priors, showed better stability against extreme values in the household expenditure dataset.

---

## 🚀 How to Run
1. Install Stan and the R interface:
   ```r
   install.packages("rstan")
