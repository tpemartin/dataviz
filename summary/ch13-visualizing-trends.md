# Chapter 13 — Visualizing Trends

**Source file:** `visualizing_trends.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Many datasets are noisy, making it hard to see underlying patterns. This chapter covers techniques for extracting and displaying trends, including smoothing methods (moving averages, LOESS, splines), explicit regression models, and seasonal decomposition.

---

## Learning Objectives

1. Apply appropriate smoothing techniques (moving average, LOESS, regression lines) to reduce noise and highlight trends in scatter plots and time series.
2. Distinguish between descriptive smoothers that reveal patterns and model-based fits that test explicit hypotheses.
3. Use log transformations to linearize exponential trends and seasonal decomposition to separate trend, seasonality, and residuals.

---

## Key Takeaways

- **Smoothing separates signal from noise:** A smoother draws a line through scattered data points to reveal the underlying trend. Common choices are: moving average (simple, interpretable), LOESS (locally weighted regression, flexible), and parametric regression lines (interpretable coefficients).
- **LOESS is the default general-purpose smoother:** LOESS (locally estimated scatterplot smoothing) adapts to local data density and does not assume a global functional form. Its bandwidth parameter controls smoothness — wider bandwidth = smoother, less responsive curve.
- **Regression lines communicate model-based trends:** When you have a specific functional model in mind (linear, exponential, power-law), fit and display that model explicitly. The slope and intercept carry interpretable meaning.
- **Log transformation linearizes exponential growth:** If a quantity grows multiplicatively over time (e.g., compound interest, population growth), plotting it on a log y-axis converts the exponential curve to a straight line with slope = growth rate.
- **Show uncertainty around trends:** Always display confidence bands around smoothed lines and regression fits. A trend without uncertainty information is incomplete.
- **Seasonal decomposition separates trend from seasonality:** Many time series combine a long-term trend, a repeating seasonal component, and irregular residuals. Decomposition methods (e.g., STL) separate these components so each can be visualized and interpreted independently.
