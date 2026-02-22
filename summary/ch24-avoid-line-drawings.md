# Chapter 24 — Avoid Line Drawings

**Source file:** `avoid_line_drawings.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

Historically, scientific figures were prepared as line drawings because of printing constraints. Today, color printing is ubiquitous, yet many practitioners still default to outlines and hatching. This chapter argues for using solid filled shapes instead of line drawings, demonstrating that filled shapes are visually clearer and more perceptually distinct.

---

## Learning Objectives

1. Understand why line drawings (outlines, hatched fills) produce less visually distinct and harder-to-read figures than solid filled shapes.
2. Apply solid fills to bar charts, histograms, density plots, box plots, and scatter plots to improve clarity.
3. Recognize that the historical justification for line drawings (black-and-white printing) no longer applies to most modern publication contexts.

---

## Key Takeaways

- **Filled shapes are perceptually stronger than outlines:** Solid filled regions create clear, unambiguous visual boundaries. Outlined shapes — especially when overlapping — produce confusing tangles of lines where it is hard to determine which group is which.
- **Hatched fills are rarely a good solution:** Hatching (diagonal lines, cross-hatching) was used to differentiate groups in black-and-white printing. It produces distracting visual noise (the "Moiré effect") and is perceptually inferior to color fills.
- **Bar charts: filled > outlined:** Open (unfilled) bars in a grouped bar chart are much harder to read than filled bars because adjacent bars share edges that appear as single thicker lines.
- **Histograms: filled > outlined:** Overlapping outlined histograms create ambiguity about which outline belongs to which distribution. Filled, semi-transparent histograms (or offset density plots) are clearer.
- **Box plots: lighter filled boxes, not open:** A light fill in a box plot helps distinguish the box from whiskers and from other elements in the figure.
- **Scatter plots: filled symbols > open symbols:** Open circles create visual noise in dense scatter plots. Filled circles (or other filled symbols) are perceptually cleaner and easier to distinguish.
- **When black-and-white is required:** If color must be avoided, prefer grayscale fills (light gray, dark gray, black) over hatching or outlines.
