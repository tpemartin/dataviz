# Chapter 6 — Visualizing Distributions I: Histograms and Density Plots

**Source file:** `visualizing_distributions_I.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

This chapter introduces techniques for showing the full distribution of a single continuous variable, beginning with histograms and kernel density plots. It examines how parameter choices (bin width, bandwidth) fundamentally affect what a distribution visualization reveals, and compares strategies for displaying multiple distributions simultaneously.

---

## Learning Objectives

1. Create and interpret histograms and kernel density estimates, understanding how bin width and bandwidth choices alter the appearance and interpretation of a distribution.
2. Compare the strengths and limitations of histograms vs. density plots and know when to prefer each.
3. Visualize and compare multiple distributions side by side using stacked histograms, overlapping density plots, or ridgeline plots.

---

## Key Takeaways

- **Histograms partition data into bins:** The y-axis shows either count or density (count per unit width). Appearance depends critically on bin width — too narrow produces spiky noise; too wide hides important structure. Always try multiple bin widths.
- **Density plots use kernel smoothing:** A kernel density estimate (KDE) draws a smooth curve over the data. The bandwidth parameter controls smoothness analogously to bin width. Density plots look cleaner than histograms but may extend into impossible ranges (e.g., negative values for non-negative data).
- **Histograms show actual counts; density plots show relative frequencies:** For communicating absolute numbers, histograms are preferable; for shape comparisons, density plots often work better.
- **Overlapping histograms are usually bad:** When comparing multiple groups, overlapping histograms become hard to read quickly. Overlay transparent density curves instead, or use a ridgeline plot.
- **Ridgeline (joy) plots for many groups:** Staggered density plots arranged vertically allow comparison of distributions across many groups or time periods in a compact space.
- **Faceting is often the safest option:** Placing each group's histogram or density plot in its own panel with a shared x-axis scale is less visually elegant but maximally clear.
