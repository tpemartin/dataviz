# Chapter 2 — Coordinate Systems and Axes

**Source file:** `coordinate_systems_axes.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

This chapter examines the various coordinate systems used in data visualization and how the choice of coordinate system fundamentally shapes how data is perceived. It covers Cartesian coordinates, non-linear axes (log scale), curved coordinates (polar, geographic projections), and the importance of axis labeling and aspect ratios.

---

## Learning Objectives

1. Understand how different coordinate systems — Cartesian, log-scale, polar, and geographic — transform the perception of data relationships.
2. Know when to use linear vs. logarithmic axes and how to interpret each correctly.
3. Recognize how aspect ratio and axis labeling affect the accuracy of a reader's interpretation.

---

## Key Takeaways

- **Cartesian coordinates are the default:** Most visualizations use two perpendicular linear axes (x and y). The same data values always map to the same positions regardless of context, making Cartesian plots highly interpretable.
- **Aspect ratio matters:** Stretching or compressing a figure can make relationships appear steeper or flatter. Choose an aspect ratio that faithfully represents the data's structure (e.g., use equal axes when plotting spatial data to avoid distortion).
- **Log scales reveal multiplicative relationships:** Use a logarithmic axis when data spans several orders of magnitude or when multiplicative/ratio relationships are more meaningful than additive ones. On a log scale, equal distances represent equal ratios, not equal differences.
- **Polar coordinates suit cyclic data:** Polar coordinates map data onto angles and radii, making them natural for cyclical phenomena (e.g., time of day, compass direction). They underlie pie charts (angle encodes proportion) and wind roses.
- **Geographic projections are coordinate systems too:** Projecting the curved Earth onto a flat map requires choosing a projection, each of which distorts area, shape, distance, or direction. No single projection preserves all properties simultaneously.
- **Always label axes with units:** Every quantitative axis must include both a descriptive title and measurement units so readers can interpret actual data values.
