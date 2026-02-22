# Chapter 11 — Visualizing Associations Among Two or More Quantitative Variables

**Source file:** `visualizing_associations.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

This chapter examines how to reveal relationships (associations) between two or more quantitative variables. It covers scatter plots, bubble charts, correlograms, and dimension-reduction techniques, as well as paired-data plots such as slope graphs.

---

## Learning Objectives

1. Design effective scatter plots for exploring and communicating pairwise relationships between quantitative variables, including handling a third variable via size, color, or shape.
2. Use correlograms and paired scatter plot matrices to visualize associations among many variables at once.
3. Apply slope graphs and other paired-data techniques to highlight change or difference between two conditions.

---

## Key Takeaways

- **Scatter plots are the workhorse for associations:** Plotting one variable on the x-axis and another on the y-axis makes the strength and direction of their relationship immediately visible. Add a trend line (regression line or LOESS smoother) to guide the eye.
- **A third variable can be encoded via color, size, or shape:** Bubble charts add a size aesthetic; a color aesthetic can encode a categorical or continuous third variable. Avoid encoding more than 2–3 variables in a single scatter plot — beyond that, faceting is clearer.
- **Correlograms summarize many pairwise relationships:** A correlogram (matrix of correlation coefficients or scatter plots) is useful for a first-pass exploration of a multi-variable dataset. Color-coded correlation matrices and scatterplot matrices (pairs plots) are two common forms.
- **Slope graphs show paired or longitudinal comparisons:** A slope graph connects the same entity's value at two (or more) time points with a line, making changes and rank shifts immediately visible. They are particularly effective for showing before-vs-after comparisons across many entities.
- **Be wary of spurious correlations:** Correlation in a scatter plot does not imply causation. Always ask whether a confounding variable could explain the observed association.
- **Log-scale axes for multiplicative associations:** When the relationship between two variables is multiplicative (e.g., exponential growth), plotting both axes on a log scale linearizes the relationship and makes it easier to fit and interpret.
