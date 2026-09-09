---
layout: page
title: Automated Detection of Planets
description: Computer vision & image processing pipeline for detecting and classifying planets in NASA/ESA astronomical imagery (2020–2021).
img: assets/img/12.jpg
importance: 1
category: Applied AI
related_publications: false
---

### Research & Thesis Overview
Bachelor's Internship & Research Project completed at Azad University, North Tehran Branch (2020–2021).

Designed and implemented an automated computer vision pipeline for detecting, segmenting, and classifying celestial bodies and planets in scientific astronomical imagery obtained from NASA and ESA public archives.

### Methodology & Pipeline
- **Preprocessing:** Gaussian and median spatial filtering, global histogram equalization, Contrast Limited Adaptive Histogram Equalization (CLAHE), and background subtraction.
- **Segmentation & Detection:** Canny edge detection, morphological opening/closing operations, and OpenCV contour analysis for region-of-interest localization.
- **Feature Extraction:** Extracted multi-dimensional feature vectors including morphological descriptors, photometric intensity moments, RGB/HSV color histograms, and Gray-Level Co-occurrence Matrix (GLCM) texture statistics.
- **Classification & Evaluation:** Trained and rigorously benchmarked Support Vector Machines (SVM) and K-Nearest Neighbors (KNN) classifiers for multi-class planetary identification.

### Tech Stack
`Python` `OpenCV` `scikit-learn` `NumPy` `SciPy` `Matplotlib`
