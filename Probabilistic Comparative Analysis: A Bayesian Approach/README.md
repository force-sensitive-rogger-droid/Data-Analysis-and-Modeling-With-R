# Probabilistic Comparative Analysis: A Bayesian Approach

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Bayesian](https://img.shields.io/badge/Statistics-Bayesian_Inference-red?style=for-the-badge)
![Probability](https://img.shields.io/badge/Analysis-Probabilistic-gold?style=for-the-badge)

## 📌 Project Overview
This project demonstrates the application of **Bayesian Statistical Methods** to compare probabilistic models and estimate parameters under uncertainty. Moving beyond frequentist p-values, this analysis utilizes **Prior distributions**, **Likelihood functions**, and **Posterior distributions** to make informed statistical inferences.

The project is structured into two main analytical parts:
1. **Beta-Binomial Conjugate Analysis:** Comparing success rates between different groups.
2. **Predictive Inference:** Using posterior distributions to forecast future outcomes.

---

## 📊 Part 1: Beta-Binomial Model Comparison
A comparative study of two groups (e.g., Treatment vs. Control or different user segments) using the Beta-Binomial conjugate prior framework.

* **Methodology:** * Assignment of non-informative and informative **Priors** ($\alpha, \beta$).
    * Computation of **Posterior distributions** after observing data.
    * Statistical comparison using the **Posterior Odds Ratio**.
* **Key Insight:** Determination of the probability that one group outperforms the other ($P(\theta_1 > \theta_2 | data)$), providing a more intuitive result than traditional significance testing.

---

## 📉 Part 2: Bayesian Parameter Estimation & Prediction
Focus on estimating unknown parameters and generating predictive distributions for future observations.

* **Core Tasks:**
    * Deriving Posterior Mean, Mode, and **Highest Posterior Density (HPD) Intervals**.
    * Sensitivity analysis of Prior selection on the final results.
    * Simulating predictive distributions to quantify uncertainty in future events.
* **Techniques:** Integration of prior knowledge with observed evidence to refine model accuracy.

---

## 🛠️ Mathematical & Technical Stack
* **Language:** R
* **Statistical Concepts:** * Conjugate Priors (Beta, Binomial).
    * Credible Intervals (vs. Confidence Intervals).
    * Posterior Predictive Checks.
* **Visualization:** Custom `ggplot2` plots to visualize the shift from Prior to Posterior distributions.

---

## 💡 Why Bayesian?
Unlike standard frequentist methods, this approach allows for:
1. **Incorporating Expert Knowledge:** Using Priors to inform the model before seeing data.
2. **Direct Probabilistic Statements:** Answering "What is the probability that X is true?" instead of "Can we reject the null hypothesis?".
3. **Better Handling of Small Samples:** More robust results when data is scarce.

---

## 🚀 How to Run
1. Open the `.qmd` file in RStudio.
2. Ensure you have the following libraries: `tidyverse`, `extraDistr`, and `knitr`.
3. Render the document to view the mathematical derivations and visual outputs.

---
**Author:** Charalampos Sarakatsanis  
**Course:** STAT40850 - Bayesian Analysis
