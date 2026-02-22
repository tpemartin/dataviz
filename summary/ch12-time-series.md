# Chapter 12 — Visualizing Time Series and Other Functions of an Independent Variable

**Source file:** `time_series.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Time series are a ubiquitous data type in which observations are recorded at successive time points. This chapter covers line graphs as the primary tool for time series, strategies for comparing multiple time series, connected scatter plots for bivariate time-dependent data, and approaches for high-dimensional time series.

---

## Learning Objectives

1. Design clear, effective line graphs for single and multiple time series, including choices about axis scaling, filling, and labeling.
2. Understand when to use a connected scatter plot (phase portrait) instead of separate time series lines to reveal cyclic or lagged relationships.
3. Handle high-dimensional time series using smoothing, dimensionality reduction, or faceting.

---

## Key Takeaways

- **Line graphs emphasize temporal order:** Connecting points with lines signals that observations are ordered and that interpolation between consecutive points is meaningful. Use lines only when the x-axis represents a truly ordered, continuous variable.
- **Fill area under curves with care:** Shading the area between the line and the zero baseline emphasizes magnitude and cumulative quantities, but is only meaningful when zero is a natural baseline. Filling to a non-zero baseline can be misleading.
- **Multiple time series need careful separation:** For 2–3 series, overlapping lines with different colors work well. For more series, direct labeling (text at the end of each line) is better than a legend. For many series, faceting into separate panels prevents overplotting.
- **Direct labeling over legends:** In time series charts, labeling each line at its end or at a prominent point is more readable than a separate legend, which forces readers to match colors.
- **Connected scatter plots reveal relationships over time:** By plotting two variables against each other and connecting observations chronologically, a connected scatter plot shows how the relationship between the variables evolves — revealing cycles, loops, and lead-lag patterns invisible in separate line graphs.
- **Smoothing for noisy series:** A LOESS smoother or rolling average reduces noise and highlights the underlying trend, though it removes information about short-term variation. Show both the raw data and the smooth when both matter.
