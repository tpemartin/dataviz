# Chapter 8 — Visualizing Many Distributions at Once

**Source file:** `boxplots_violins.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

When distributions must be compared across many groups, individual histograms or density plots become unwieldy. This chapter presents techniques — box plots, violin plots, strip charts, sina plots, and ridgeline plots — designed for simultaneously displaying and comparing the shapes of multiple distributions.

---

## Learning Objectives

1. Select an appropriate technique (box plot, violin plot, strip chart, sina plot, or ridgeline plot) based on the number of observations per group and the need to show individual data points vs. distributional summaries.
2. Understand what a box plot's components (median, IQR, whiskers, outliers) represent and when box plots are and are not appropriate.
3. Recognize when more informative alternatives to box plots — violin plots and sina plots — better reveal distributional shape.

---

## Key Takeaways

- **Box plots are compact but can hide shape:** A box plot shows the median, interquartile range (IQR), whiskers (typically 1.5 × IQR), and outliers. Two very different distributions (e.g., unimodal vs. bimodal) can produce identical box plots. Use box plots only when you are confident the distribution shape is not critical to your message.
- **Violin plots reveal distributional shape:** A violin plot mirrors a kernel density estimate on both sides of a center line. This reveals multimodality and the full shape of the distribution, at the cost of requiring enough data to produce a meaningful density estimate.
- **Strip charts for small datasets:** When there are few observations per group (roughly < 50), showing individual points directly (a strip chart) is more honest than a summary. Add jitter to separate overplotted points.
- **Sina plots combine individual points with density:** A sina plot jitters each point horizontally in proportion to the local density, combining the benefits of strip charts and violin plots. It works well for moderate sample sizes.
- **Ridgeline plots for trends across many groups:** Ridgeline (joy) plots stack horizontally offset density plots, making them ideal for showing how a distribution changes across many ordered groups (e.g., years, income brackets).
- **Avoid bar charts with error bars for distributions:** A bar showing mean ± standard deviation or standard error conveys very little about the true distribution shape and can be misleading.
