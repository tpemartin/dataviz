# Chapter 20 — Multi-Panel Figures

**Source file:** `multi-panel_figures.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

Complex datasets often require showing multiple related plots side by side. This chapter distinguishes between small multiples (trellis/facet plots, where panels show the same type of visualization for different data subsets) and compound figures (panels showing different types of visualizations assembled into a single figure). It covers layout, alignment, and labeling conventions.

---

## Learning Objectives

1. Distinguish between small multiples (faceted panels of the same plot type) and compound figures (panels of different plot types) and know when each is appropriate.
2. Design small multiples with consistent scales and minimal redundancy so that differences between panels are immediately apparent.
3. Assemble compound figures with proper panel labeling (a, b, c…), aligned axes, and a coherent narrative.

---

## Key Takeaways

- **Small multiples (faceting) for the same visualization across subgroups:** Placing the same chart type side by side for different subsets of data (e.g., one panel per country, one per year) allows direct visual comparison with minimal cognitive load. The key requirement is that all panels share the same axis scales.
- **Consistent scales are critical in small multiples:** Different scales in each panel prevent valid visual comparisons. Use a shared, consistent scale even if it means some panels have lots of white space.
- **Compound figures assemble different chart types:** When presenting results from multiple related analyses, arranging different plots (e.g., a map, a bar chart, and a scatter plot) as labeled panels (a, b, c) in a single figure helps readers see the full picture.
- **Label panels with (a), (b), (c):** Use letter labels in the top-left corner of each panel, referenced in the figure caption. This allows the caption to describe each panel separately.
- **Align axes across panels where meaningful:** When panels share a common axis (e.g., the same time range or the same x variable), aligning that axis across panels makes comparisons easier. Use a shared axis strip to avoid repeating axis labels.
- **Minimize redundancy:** Avoid repeating the same axis labels, titles, or legends in every panel. Shared axes and a single shared legend reduce ink and visual clutter.
