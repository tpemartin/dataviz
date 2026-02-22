# Chapter 1 — Visualizing Data: Mapping Data onto Aesthetics

**Source file:** `aesthetic_mapping.Rmd`  
**Part I: From Data to Visualization**

---

## Overview

This chapter introduces the foundational concept underlying all data visualizations: mapping data values onto visual (aesthetic) properties. It presents a common language for describing any visualization — from scatter plots to pie charts — in terms of aesthetics such as position, shape, size, color, line width, and line type.

---

## Learning Objectives

1. Understand that all visualizations are systematic mappings from data values to quantifiable graphical features called *aesthetics*.
2. Distinguish between the five main data types (continuous quantitative, discrete quantitative, categorical/qualitative, date/time, text) and know which aesthetics are appropriate for each.
3. Understand the role of *scales* as the one-to-one mapping between a data dimension and an aesthetic dimension.

---

## Key Takeaways

- **All visualizations share a common language:** Every graphical element in a figure — whether in a bar chart, scatter plot, or heatmap — can be described by the same set of aesthetic properties: position (x, y), shape, size, color, line width, and line type.
- **Continuous vs. discrete aesthetics:** Position, size, color, and line width can represent continuous data. Shape and line type can only represent discrete data.
- **Five data types to know:**
  | Type | Example | Notes |
  |------|---------|-------|
  | Continuous quantitative | temperature, weight | Arbitrarily fine intermediates exist |
  | Discrete quantitative | number of people | Only integer values |
  | Categorical (qualitative) | dog, cat, fish | Unordered or ordered (factor) levels |
  | Date/time | Jan 5, 2018 | Ordered, but calendar-specific |
  | Text | "hello" | Free-form, usually not mapped to aesthetics |
- **Scales define the mapping:** A scale converts data values into aesthetic values (e.g., a color scale maps temperature to a color gradient). Each aesthetic in a figure has exactly one scale.
- **Not all aesthetics suit all data types:** Using shape to encode a continuous variable is ineffective; use position or color instead.
