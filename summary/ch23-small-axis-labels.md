# Chapter 23 — Use Larger Axis Labels

**Source file:** `small_axis_labels.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

One of the most pervasive and easily corrected visualization problems is text that is too small to read comfortably. This chapter argues strongly for using larger axis labels and text throughout figures, explains why default software settings often produce text that is too small, and provides guidance on calibrating text size relative to the final figure size.

---

## Learning Objectives

1. Recognize that axis labels and tick mark labels in most default plots are too small for comfortable reading, especially at final print or display size.
2. Calibrate text sizes by previewing figures at their actual output size before finalizing.
3. Balance text size with other figure elements (point size, line width) to produce a visually harmonious, readable figure.

---

## Key Takeaways

- **Default axis label sizes are almost always too small:** Plotting software defaults are calibrated for large on-screen previews, not for the small final sizes typical of journal figures (single column ≈ 3.5 inches wide) or slide panels. At print size, default labels become illegible.
- **Always preview at actual output size:** Resize the figure to its intended final dimensions before judging whether text is legible. What looks fine at full-screen size may become unreadable at 3.5 × 2.5 inches.
- **Rule of thumb:** Axis labels should be readable without a magnifying glass by someone with normal vision at normal reading distance. If you cannot read the axis labels easily, they are too small.
- **Scale up text when scaling down figures:** If a figure will be printed at half the size it was created at, all text must be doubled in size during figure preparation to appear at the intended final size.
- **Balance text with other elements:** Larger text must be balanced with appropriately sized data marks (larger points, wider lines) and margins. A figure with large text but tiny points looks as unbalanced as one with tiny text.
- **Rotated axis labels are a symptom of too-small text:** Long category labels are often rotated 45° or 90° to fit on the axis, which is harder to read. The better solution is to increase figure width, reduce label count, abbreviate labels, or switch to a horizontal bar chart.
