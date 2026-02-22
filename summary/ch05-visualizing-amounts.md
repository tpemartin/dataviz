# Chapter 5 — Visualizing Amounts

**Source file:** `visualizing_amounts.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

This chapter focuses on visualizing a single quantitative value for each of several categories — "amounts." It compares bar plots, dot plots, and heatmaps, and explores design choices such as bar orientation, ordering, and grouping that affect how clearly the data's message comes through.

---

## Learning Objectives

1. Choose between bar plots, dot plots, and other chart types when visualizing categorical amounts based on the number of categories and the nature of the data.
2. Apply ordering strategies (by value, alphabetical, natural) that help readers extract the key message from an amount visualization.
3. Design grouped and faceted bar charts to effectively compare amounts across multiple categorical dimensions.

---

## Key Takeaways

- **Bar plots are the default for amounts:** A bar plot encodes a quantity as the length of a bar. The bar's length is perceptually easy to judge, making bar charts highly effective for comparing values across categories.
- **Bars must start at zero:** Because bar length encodes the quantity, truncating the axis creates a misleading impression of differences. This is a violation of the proportional ink principle.
- **Order categories meaningfully:** Sort bars by value (descending or ascending) unless there is a natural order (e.g., months of the year). Alphabetical ordering rarely helps the reader see patterns.
- **Horizontal bars for long category names:** Rotate the chart so bars run horizontally when category labels are long text strings — this avoids cramped, rotated labels on a vertical bar chart.
- **Dot plots as an alternative:** Replacing bars with dots removes the need for a zero baseline (since dots encode position, not length). Dot plots work especially well when values are all of similar magnitude or when the baseline is not meaningful.
- **Grouped vs. stacked vs. faceted bars:** For two categorical dimensions, grouped bars (side by side) facilitate within-group comparisons; stacked bars show totals; faceting separates groups into panels and reduces clutter.
- **Heatmaps for many categories:** When both row and column dimensions have many categories, a heatmap (color-encoded matrix) is often clearer than a bar chart forest.
