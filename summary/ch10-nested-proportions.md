# Chapter 10 — Visualizing Nested Proportions

**Source file:** `nested_proportions.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Some datasets have proportions that are themselves subdivided into further proportions, creating hierarchical (nested) structures. This chapter explores visualization methods for such nested data, including mosaic plots, treemaps, parallel sets (Sankey diagrams), and nested pie/donut charts.

---

## Learning Objectives

1. Recognize when proportional data has a nested or hierarchical structure that requires a visualization beyond a simple pie or stacked bar chart.
2. Understand the strengths and weaknesses of mosaic plots, treemaps, and parallel sets diagrams for nested proportions.
3. Apply the appropriate nested proportion visualization based on the depth of the hierarchy and the message to communicate.

---

## Key Takeaways

- **Nested proportions add a level of hierarchy:** Instead of a single set of parts summing to a whole, nested proportions have categories that are themselves divided into subcategories. For example, political party affiliation broken down by gender and age group.
- **Mosaic plots encode two proportional dimensions simultaneously:** The width of each column represents one categorical variable's proportion; within each column, subdivisions represent a second categorical variable. They work well for two-level hierarchies but become hard to read with more levels.
- **Treemaps tile a rectangle with area-proportional rectangles:** Each rectangle's area represents its proportion of the whole. Treemaps can show multiple levels of hierarchy via nested rectangles, but area is harder to judge accurately than length.
- **Parallel sets (Sankey) diagrams show flow between categories:** Flow widths are proportional to the frequencies they represent, making it easy to trace how a population is distributed across multiple categorical dimensions simultaneously.
- **Nested pie / donut charts:** An outer ring and inner ring can show two levels of a hierarchy, but they quickly become unreadable and are generally not recommended.
- **Prefer simpler charts when hierarchy is shallow:** For two-level hierarchies, a faceted stacked bar chart is often clearer than a mosaic plot or treemap.
