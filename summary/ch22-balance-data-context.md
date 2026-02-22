# Chapter 22 — Balance the Data and the Context

**Source file:** `balance_data_context.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

Every visualization contains both data elements (the marks that represent data values) and non-data elements (axes, grid lines, labels, backgrounds). This chapter discusses how to balance these two types of elements, drawing on Tufte's concept of the "data-ink ratio" while avoiding the extreme of "chartjunk minimalism" that removes useful contextual elements.

---

## Learning Objectives

1. Understand the data-ink ratio concept and how it guides decisions about what elements to include or remove from a figure.
2. Recognize the difference between useful contextual elements (axis labels, reference lines, grid lines) and decorative elements that add visual noise without information.
3. Apply the principle of balance: neither overloaded figures full of chartjunk nor stripped-down figures lacking necessary context.

---

## Key Takeaways

- **Data-ink ratio (Tufte):** Maximize the proportion of a figure's ink devoted to displaying data. Remove or de-emphasize non-data ink that does not contribute to understanding.
- **Balance, not minimalism:** While the data-ink ratio is a useful guide, removing *all* non-data elements produces sterile, hard-to-read figures. Axis lines, tick marks, grid lines, and background fill can all serve useful contextual roles when used thoughtfully.
- **Grid lines: use sparingly, make subtle:** Horizontal grid lines help readers estimate values from bar or line charts. However, heavy, closely spaced grids dominate the figure and obscure the data. Use light, widely spaced major gridlines only when they add value.
- **Background fills: neutral, not white:** A very light gray background (as in the ggplot2 default gray theme) can help the figure stand out from surrounding white text. Pure white backgrounds can sometimes make figures float.
- **Avoid chartjunk:** Decorative 3D effects, unnecessary borders, patterned fills, clip art, and excessive gridlines add visual noise without improving comprehension. Every element should earn its place.
- **Context enables interpretation:** Reference lines (e.g., a threshold line, a national average), annotations, and shaded regions provide essential context that helps readers interpret data values. These are non-data elements that genuinely add informational value.
