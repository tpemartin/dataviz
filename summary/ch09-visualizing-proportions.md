# Chapter 9 — Visualizing Proportions

**Source file:** `visualizing_proportions.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Proportions (parts of a whole) are a special class of amounts that sum to a meaningful total. This chapter evaluates the primary chart types for displaying proportions — pie charts, stacked bar charts, and side-by-side bar charts — and discusses the conditions under which each succeeds or fails.

---

## Learning Objectives

1. Understand the part-to-whole constraint that defines proportional data and how it influences chart design.
2. Compare pie charts, stacked bar charts, and side-by-side bars in terms of their accuracy for conveying proportional information.
3. Choose the appropriate proportion visualization based on the number of categories and whether individual values or comparisons across groups are more important.

---

## Key Takeaways

- **Proportions must sum to 100%:** This constraint is fundamental. Every chart that shows proportions implicitly makes a claim about the whole, so any omitted category must be explained or labeled.
- **Pie charts are acceptable for a few categories:** When there are 2–3 parts and the goal is simply to show rough relative sizes, a well-designed pie chart is fine. Pie charts become hard to read with 5+ slices, especially when slices are similar in size, because humans judge angles and arc lengths poorly.
- **Stacked bar charts for multiple groups:** When proportions must be compared across several groups (e.g., survey responses by year), a stacked bar chart places all groups on a common axis, making the overall pattern visible. However, only the first and last categories (anchored to the two ends of the bars) are easy to compare precisely.
- **Side-by-side bars for direct comparisons:** Placing bars for each category next to each other rather than stacking them makes individual values easy to compare, but loses the visual impression of the whole.
- **100% stacked bars emphasize relative composition:** Scaling all bars to the same height forces a focus on proportional composition rather than absolute values, useful when comparing relative mix across groups.
- **Avoid pie charts when precision matters or there are many categories:** In those situations, a stacked bar chart or a dot plot of percentages communicates the same information more accurately.
