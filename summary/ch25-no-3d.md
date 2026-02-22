# Chapter 25 — Don't Go 3D

**Source file:** `no_3d.Rmd`  
**Part II: Principles of Figure Design**

---

## Overview

Three-dimensional visualizations are seductive — they look impressive and modern. This chapter makes the case that gratuitous 3D (adding a third dimension that does not encode additional data) almost always distorts perception, misleads the reader, and reduces accuracy. Legitimate uses of 3D are discussed.

---

## Learning Objectives

1. Identify gratuitous 3D effects (3D bar charts, 3D pie charts, extruded shapes) and explain why they distort data perception.
2. Redesign a 3D visualization as an effective 2D alternative that communicates the same information more accurately.
3. Recognize the limited legitimate uses of 3D — actual three-dimensional data, physical surfaces, and interactive/animated displays.

---

## Key Takeaways

- **Gratuitous 3D distorts perception:** Adding a third dimension to a bar chart, pie chart, or line chart that doesn't encode any additional data variable creates perspective distortions. Bars at the back of a 3D chart appear shorter than equally-sized bars at the front.
- **3D projection is a non-invertible transformation:** Converting 3D coordinates to a 2D image projection destroys spatial information. Readers cannot accurately invert the perspective to recover original data values, making 3D charts inherently less accurate than 2D equivalents.
- **3D pie charts are particularly bad:** The perspective tilt makes front slices appear larger than back slices, distorting perceived proportions. A simple pie chart or bar chart is always preferable.
- **Two 2D plots beat one 3D plot:** When data has three variables, encode two in a scatter plot's x-y axes and the third via color, size, or shape. Alternatively, use faceting. Both approaches are more readable than a 3D scatter plot.
- **Legitimate uses of 3D:** Actual three-dimensional phenomena (terrain maps, molecular structures, architectural models) may genuinely require 3D representation. Interactive or animated 3D allows rotation, which partially overcomes the perception problems of static 3D.
- **Log-log scatter plots remove the need for 3D:** When two variables vary multiplicatively over a wide range, a log-log scatter plot reveals the structure that a 3D plot might attempt (and fail) to show simultaneously.
