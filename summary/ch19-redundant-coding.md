# Chapter 19 — Redundant Coding

**Source file:** `redundant_coding.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

Redundant coding means encoding the same data dimension using multiple aesthetics simultaneously (e.g., both color and shape for group membership). This chapter argues that redundant coding improves accessibility and robustness, especially for colorblind readers and black-and-white printing.

---

## Learning Objectives

1. Understand what redundant coding is and why using multiple aesthetics for the same variable improves accessibility and clarity.
2. Apply redundant coding by pairing color with shape, line type, or fill pattern to make figures legible in grayscale and for colorblind readers.
3. Design legends that exploit redundant coding, and recognize when direct labeling can replace a legend altogether.

---

## Key Takeaways

- **Redundant coding = same variable, multiple aesthetics:** Mapping group membership to both color and shape (e.g., circles vs. triangles) means readers can identify groups even if they cannot distinguish colors — essential for colorblind accessibility and black-and-white reproduction.
- **Color alone is insufficient for many audiences:** About 8% of males have color-vision deficiency. Additionally, printed figures are often photocopied in grayscale. Relying solely on color creates barriers for a significant fraction of potential readers.
- **Pair color with shape for scatter plots:** Use different point shapes (circle, triangle, square, diamond) together with different colors for each group. Both aesthetics convey the same grouping information redundantly.
- **Pair color with line type for line graphs:** Use different line styles (solid, dashed, dotted) in addition to different colors for each series in a multi-line plot.
- **Match legend order to visual ordering in the figure:** The legend should list groups in the same order they appear visually (e.g., top-to-bottom for a line chart where lines are ordered by their final values). Mismatched order forces unnecessary cognitive matching.
- **Direct labeling can replace legends:** When possible, label each group directly (e.g., at the end of a line, or adjacent to a cluster of points) instead of using a legend. This eliminates the need for the reader to visually look up colors.
