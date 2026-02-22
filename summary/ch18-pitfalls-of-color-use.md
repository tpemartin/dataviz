# Chapter 18 — Common Pitfalls of Color Use

**Source file:** `pitfalls_of_color_use.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

Color is easy to misuse. This chapter catalogs the most frequent color pitfalls: encoding too many categories, using non-monotonic scales (e.g., rainbow/jet), ignoring color-vision deficiency, and using color unnecessarily. It reinforces how to choose accessible, effective color palettes.

---

## Learning Objectives

1. Recognize and avoid the most common color mistakes: too many categories, non-monotonic scales, red–green contrasts, and decorative color use.
2. Select colorblind-safe palettes (Okabe-Ito, ColorBrewer) for both categorical and continuous data.
3. Understand how to test a figure for color-vision deficiency accessibility using simulation tools.

---

## Key Takeaways

- **Limit categorical color encoding to ~8 categories:** Human color perception struggles to distinguish more than about 8–10 distinct colors simultaneously, especially at small sizes or in low-contrast conditions. For more categories, use direct labeling, faceting, or a combination of color and shape.
- **Avoid the rainbow/jet color map:** The rainbow palette (red–orange–yellow–green–blue) is non-monotonic in luminance, creates artificial boundaries at color transitions, and is not interpretable by colorblind viewers. It remains popular but should be replaced by perceptually uniform sequential scales.
- **Red–green contrasts are invisible to the most common CVD types:** Deuteranomaly (reduced green sensitivity) and protanomaly (reduced red sensitivity) affect ~6% of males. Never use red and green as the only distinguishing colors for two critical categories.
- **Use CVD simulation software to test figures:** Tools such as the R package `colorblindr` or online simulators (Coblis, Sim Daltonism) render your figure as it appears to viewers with different types of CVD. Test figures before publication.
- **Color elements must be large enough to distinguish:** Small colored symbols, thin colored lines, or low-contrast backgrounds make color discrimination harder. Increase marker size, line width, or contrast when using color as a primary encoding.
- **Don't use color for decoration:** Adding rainbow stripes, multicolored bars that encode no data, or decorative gradients adds visual noise without information. Color should always encode something meaningful or should be a neutral, non-distracting background.
