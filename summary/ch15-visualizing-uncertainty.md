# Chapter 15 — Visualizing Uncertainty

**Source file:** `visualizing_uncertainty.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Communicating uncertainty is one of the most challenging aspects of data visualization, yet it is essential for honest and informative reporting of scientific results. This chapter surveys the major techniques for visualizing uncertainty: error bars, confidence bands, frequency framing, and probabilistic visualizations.

---

## Learning Objectives

1. Understand the different types of uncertainty estimates (standard deviation, standard error, confidence interval) and know what each communicates.
2. Choose appropriate visualizations for uncertainty depending on whether the audience is statistically trained or general-public.
3. Apply frequency-based framing and probabilistic plot types (e.g., hypothetical outcome plots, quantile dot plots) to communicate uncertainty to non-expert audiences.

---

## Key Takeaways

- **Error bars are often misunderstood:** An error bar can represent ±1 SD (describes the data spread), ±1 SE (precision of the mean estimate), or a 95% confidence interval (a range consistent with the data under a model). Always state explicitly what the error bar represents.
- **Graded uncertainty visualizations are more informative:** Rather than a single error bar, showing a gradient of confidence bands (e.g., 50%, 80%, 95% CI) communicates the full uncertainty distribution more completely.
- **Confidence intervals vs. credible intervals:** Frequentist confidence intervals (CIs) have a specific technical meaning that is often misinterpreted. Bayesian credible intervals have the more intuitive interpretation of "the parameter lies in this range with X% probability."
- **Frequency framing helps non-expert audiences:** Showing uncertainty as "X out of 100 people" or via icon arrays (each icon = one person) is often more intuitively understood by general audiences than probability statements.
- **Hypothetical outcome plots (HOPs) animate uncertainty:** By showing a rapid sequence of plausible outcomes drawn from the uncertainty distribution, HOPs can convey probabilistic concepts more intuitively than static displays — though they require animation.
- **Quantile dot plots:** Dot plots where the number of dots in each bin represents the probability of that outcome provide a discrete, count-based representation of a probability distribution that is accessible to non-expert audiences.
- **Never omit uncertainty:** A point estimate without any indication of uncertainty is an incomplete and potentially misleading representation of the data.
