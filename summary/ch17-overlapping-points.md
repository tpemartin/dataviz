# Chapter 17 — Handling Overlapping Points

**Source file:** `overlapping_points.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

When plotting many data points, individual points frequently overlap, hiding the true density of the data. This chapter surveys techniques for dealing with overplotting: partial transparency, jittering, 2D binning (histograms and hexbins), contour lines, and faceting.

---

## Learning Objectives

1. Identify overplotting in a scatter plot and select an appropriate remedy based on the size and structure of the dataset.
2. Apply transparency, jittering, 2D histograms, hexagonal binning, and contour lines appropriately, understanding the tradeoffs of each.
3. Use faceting to separate overlapping groups and reduce clutter in complex multi-group datasets.

---

## Key Takeaways

- **Overplotting hides data density:** When many points share the same (or very similar) position, the resulting solid blob misrepresents the actual distribution. The first step is to recognize that overplotting is occurring.
- **Partial transparency (alpha blending):** Making points semi-transparent so that overlapping points appear darker than isolated points is the simplest remedy for moderate overplotting. The correct alpha level depends on point size and data density and usually requires trial and error.
- **Jittering adds small random offsets:** Displacing points by a small random amount (jitter) spreads them apart enough to see overlapping values. Jitter is most appropriate for discrete data where many observations share the exact same value. Avoid large jitter that moves points far from their true positions.
- **2D histograms bin the plotting area into rectangles:** Instead of drawing individual points, a 2D histogram divides the x-y space into a grid and colors each cell by point count. This is effective for very large datasets but loses individual-point information.
- **Hexagonal binning:** Like a 2D histogram but using hexagonal cells, which tile the plane more efficiently and reduce visual artifacts from axis-aligned binning. Preferred over rectangular binning for large datasets.
- **Contour plots show density as isolines:** Drawing contour lines at density thresholds provides a smooth, continuous representation of point density. Combine with a scatter plot for the best of both worlds.
- **Faceting separates groups into panels:** If overplotting is caused by many overlapping groups, splitting each group into a separate panel eliminates inter-group overlap while preserving the within-group density pattern.
