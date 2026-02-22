# Chapter 27 — Choosing the Right Visualization Software

**Source file:** `choosing_visualization_software.Rmd`  
**Part III: Miscellaneous Topics**

---

## Overview

The choice of visualization software profoundly affects reproducibility, workflow efficiency, and the range of figures that can be produced. This chapter discusses the key dimensions along which to evaluate software: reproducibility vs. interactivity, exploration vs. presentation, and the separation of content from design.

---

## Learning Objectives

1. Evaluate visualization software along the dimensions of reproducibility, repeatability, interactivity, and scope (exploration vs. presentation-quality output).
2. Understand why programmatic figure generation (code-based) is strongly preferable to interactive point-and-click tools for scientific publications.
3. Appreciate the role of themes/styles in separating the content of a visualization from its aesthetic presentation.

---

## Key Takeaways

- **Reproducibility is essential for science:** A figure is reproducible if running the same code on the same data produces the same output. Interactive, point-and-click tools (Excel, PowerPoint chart editors) make figures irreproducible because no code records the exact steps taken.
- **Programmatic tools (R/ggplot2, Python/matplotlib, Vega-Lite) are strongly preferred:** Code is a precise, rerunnable record of every decision made to produce a figure. Code-based figures can be regenerated automatically when data changes.
- **Exploration ≠ presentation:** During data exploration, speed and interactivity matter more than polish. During preparation of final figures for publication, reproducibility and fine control over appearance matter most. Some workflows use interactive tools for exploration and code for final figures.
- **Separation of content and design via themes:** Good visualization software supports *themes* (or styles) that control the appearance of a figure (colors, font sizes, background) independently of the data mapping. This allows consistent styling across all figures with minimal per-figure effort.
- **Avoid manual post-processing:** Importing a programmatically generated figure into Illustrator for "touch-ups" makes the final figure irreproducible and ties you to a slow, error-prone workflow. Invest time in learning to produce publication-ready output directly from code.
- **Pick the right tool for your context:** A journalist needing one-off interactive charts has different needs from a scientist producing reproducible publication figures. No single tool is best for all contexts; choose deliberately based on your actual needs.
