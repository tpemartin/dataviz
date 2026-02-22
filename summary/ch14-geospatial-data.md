# Chapter 14 — Visualizing Geospatial Data

**Source file:** `geospatial_data.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

Geospatial data requires specialized visualization techniques because the underlying space is curved, irregularly shaped, and must be projected onto a flat surface. This chapter covers map projections, choropleth maps, cartograms, and the use of color in maps. It discusses common pitfalls such as area bias in choropleth maps.

---

## Learning Objectives

1. Understand the concept of map projections and how different projections trade off distortions of area, shape, distance, and direction.
2. Design choropleth maps that accurately convey geographic data, choosing appropriate color scales and projection systems.
3. Recognize the limitations of standard choropleth maps (area bias) and know when alternative approaches such as cartograms or point maps are more appropriate.

---

## Key Takeaways

- **All maps distort:** Projecting the spherical Earth onto a flat surface inevitably distorts at least one of area, shape, distance, or direction. Choose a projection appropriate for your region and purpose: equal-area projections preserve relative areas; conformal projections preserve local shape.
- **Choropleth maps color geographic regions by a data value:** They are intuitive and widely used but have a critical flaw — large regions dominate visually regardless of their data value. This area bias can mislead readers if large and small regions have very different values.
- **Sequential color scales for choropleth maps:** Quantitative data on a map should use a perceptually uniform sequential (or diverging) color scale. Avoid the rainbow/jet palette, which creates false boundaries and is not colorblind-safe.
- **Cartograms correct for area bias:** A cartogram rescales geographic regions so their area is proportional to a data variable (e.g., population). This removes area bias at the cost of geographic familiarity — distorted shapes can be hard to recognize.
- **Point maps for precise locations:** When data is point-referenced (events at specific coordinates), map the points directly rather than aggregating to regions. This preserves spatial precision and avoids artificial regional boundaries.
- **Use an appropriate level of geographic detail:** For country-level data, a simple country outline is sufficient. For county- or neighborhood-level data, fine-resolution boundaries are needed. Don't add more geographic detail than the data supports.
