# Chapter 7 — Visualizing Distributions II: ECDFs and Q-Q Plots

**Source file:** `visualizing_distributions_II.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

This chapter covers more advanced approaches to distribution visualization: the empirical cumulative distribution function (ECDF) and the quantile–quantile (Q-Q) plot. These methods avoid the parameter-sensitivity problems of histograms and density plots and are particularly useful for assessing distributional assumptions or comparing groups.

---

## Learning Objectives

1. Construct and interpret empirical cumulative distribution functions (ECDFs) as a parameter-free alternative to histograms.
2. Use Q-Q plots to assess whether a dataset follows a specific theoretical distribution (e.g., normal) or to compare two empirical distributions.
3. Apply log transformations and log-log plots to reveal patterns in highly skewed or power-law distributed data.

---

## Key Takeaways

- **ECDFs require no parameter choice:** Unlike histograms or density plots, the ECDF plots each data point's value against the fraction of data at or below that value. Every data point is represented exactly. The tradeoff is that ECDFs are less intuitive to read than histograms for non-statistician audiences.
- **Reading an ECDF:** The y-axis value at any x gives the proportion of data ≤ x. Steep segments indicate high data density; flat segments indicate sparse data in that range. Comparing two ECDFs directly shows which distribution has higher values.
- **Q-Q plots test distributional assumptions:** A Q-Q plot compares the quantiles of observed data against the theoretical quantiles of a target distribution (e.g., normal). Points falling on the diagonal line indicate a good fit. Systematic curvature reveals skewness or heavy tails.
- **Q-Q plots can compare two datasets:** By plotting quantiles of one empirical distribution against another, you can check whether two groups have the same distribution regardless of what that distribution is.
- **Use log scales for skewed/power-law data:** Multiplicative processes and power-law distributions appear as straight lines on log-log plots, making patterns visible that are invisible on linear scales. Log transformation also stabilizes variance for data spanning multiple orders of magnitude.
- **Highly skewed distributions need careful handling:** The appropriate visualization — log-transformed histogram, log-log ECDF, or log-scale density plot — depends on whether you want to emphasize the body or the tail of the distribution.
