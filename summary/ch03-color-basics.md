# Chapter 3 — Color Scales

**Source file:** `color_basics.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Color is one of the most powerful and most misused aesthetics in data visualization. This chapter introduces the three fundamental use cases for color — distinguishing groups, representing data values, and highlighting — and describes the appropriate type of color scale for each case. It also addresses color-vision deficiency and the importance of designing accessible figures.

---

## Learning Objectives

1. Identify the three use cases for color in visualization (qualitative/categorical distinction, sequential/quantitative encoding, highlighting) and select the correct color scale for each.
2. Understand the difference between qualitative, sequential, and diverging color scales and know when each is appropriate.
3. Design figures that remain interpretable for viewers with color-vision deficiency (CVD).

---

## Key Takeaways

- **Three use cases for color:**
  | Use Case | Scale Type | When to Use |
  |----------|-----------|-------------|
  | Distinguish unordered groups | Qualitative | Categorical variables with no inherent order |
  | Represent ordered/continuous values | Sequential | Data with a natural low-to-high progression |
  | Show deviation from a midpoint | Diverging | Data where both extremes and a neutral center matter |

- **Qualitative scales:** Contain a small set of clearly distinct colors that are perceptually equivalent (no color should stand out more than others). The Okabe-Ito palette and ColorBrewer qualitative palettes are reliable choices.

- **Sequential scales:** Progress from light to dark (or one hue to another) to indicate low-to-high data values. Avoid rainbow/jet color maps — they are not perceptually uniform and create false boundaries.

- **Diverging scales:** Combine two sequential scales meeting at a neutral midpoint (often white or light gray). Use when the midpoint (e.g., zero, average) has a meaningful interpretation distinct from both extremes.

- **Color-vision deficiency (CVD):** Approximately 8% of males and 0.5% of females have some form of CVD. Red–green contrasts are invisible to deuteranopes and protanopes; blue–green contrasts are invisible to tritanopes. The Okabe-Ito palette is designed to be safe for the most common CVD types.

- **Don't use color as the only encoding:** For categorical data, supplement color with shape, line type, or direct labels so that the figure remains readable in black-and-white and for CVD viewers.
