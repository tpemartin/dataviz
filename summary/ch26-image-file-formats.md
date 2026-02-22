# Chapter 26 — Understanding the Most Commonly Used Image File Formats

**Source file:** `image_file_formats.Rmd`  
**Part III: Miscellaneous Topics**

---

## Overview

Choosing the wrong file format can degrade figure quality, produce unnecessarily large files, or introduce artifacts. This chapter explains the fundamental distinction between bitmap (raster) and vector graphics, describes the most common formats (PDF, PNG, JPEG, SVG, TIFF), and provides guidance on when to use each.

---

## Learning Objectives

1. Explain the difference between bitmap (raster) and vector graphics and understand the implications for resolution, file size, and quality at different output sizes.
2. Select the appropriate file format for a given figure type and output context (publication, web, presentation).
3. Avoid quality loss by understanding lossless vs. lossy compression and the consequences of format conversion.

---

## Key Takeaways

- **Bitmap (raster) vs. vector:** Bitmap images store color information for each pixel in a fixed grid; they become pixelated ("blurry") when enlarged beyond their native resolution. Vector images store geometric descriptions (lines, curves, shapes); they scale to any size without loss of quality.
- **Use vector formats for figures with lines and text:** Data visualizations made of lines, shapes, and text should be saved as PDF or SVG so they remain sharp at any print or screen size.
- **Use bitmap formats for photographs and complex images:** Images with millions of colors and smooth gradients (photographs) are impractical as vectors and are best stored as PNG (lossless) or JPEG (lossy).
- **PNG: lossless, for figures with sharp edges and text:** PNG compression preserves every pixel exactly, making it ideal for line charts, bar charts, and any figure with text. PNG files are larger than JPEG but have no quality loss.
- **JPEG: lossy, for photographs:** JPEG compression discards fine detail to achieve small file sizes. Artifacts become visible in images with sharp edges or text. Never save a data visualization as JPEG.
- **PDF: the preferred format for publications:** PDF is a vector format that also embeds fonts, making it ideal for publication-quality figures. Most journals accept PDF for figures.
- **Never re-compress a JPEG:** Each save in JPEG format introduces additional lossy compression. Always work from an original high-quality source and export to the final format once.
