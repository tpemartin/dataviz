# Chapter 16 — The Principle of Proportional Ink

**Source file:** `proportional_ink.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

The proportional ink principle states that the amount of ink (or colored area) used to represent a data value should be proportional to that value. This chapter explains when this principle applies, identifies common violations, and discusses cases where the principle must be adapted (e.g., log scales, area charts).

---

## Learning Objectives

1. Define the proportional ink principle and recognize violations in bar charts, filled area plots, and other ink-based visualizations.
2. Understand why bars in a bar chart must always start at zero on a linear scale, and why this rule changes on a logarithmic scale.
3. Apply proportional ink reasoning to area-based visualizations (pie charts, treemaps, bubble charts) and understand their inherent perceptual limitations.

---

## Key Takeaways

- **Proportional ink principle:** "The sizes of shaded areas in a visualization need to be proportional to the data values they represent." — Edward Tufte.
- **Bar charts must start at zero (linear scale):** Because a bar's visual quantity is its length/area, truncating the y-axis to start above zero inflates perceived differences between bars. This is one of the most common visualization errors.
- **The rule changes on a log scale:** On a logarithmic axis, a bar starting at 1 (not 0) satisfies the proportional ink principle because the log scale maps equal ratios to equal distances — bars represent multiplicative factors, not absolute differences.
- **Filled area charts require a zero baseline:** Filling the area under a line (an area chart) implies the area encodes magnitude. The baseline must be zero or the chart violates proportional ink.
- **Area encodings are less accurate than length encodings:** Humans judge linear distances more accurately than areas or volumes. Pie charts and bubble charts satisfy proportional ink mathematically but are perceptually inferior to bar charts because area judgments are less precise.
- **Treemaps face the same area perception challenge:** Each tile's area represents a data value, which is harder to compare accurately than bar lengths on a common axis.
