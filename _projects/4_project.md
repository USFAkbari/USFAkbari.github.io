---
layout: page
title: Automated Detection of Planets
description: Computer vision & image processing pipeline for detecting and classifying planets in NASA/ESA astronomical imagery (2020–2021).
img: assets/img/12.jpg
importance: 4
category: Research & AI
related_publications: false
---

### Project Overview
Bachelor's Internship Project completed at Azad University, North Tehran Branch (2020–2021).

Designed and implemented an automated computer vision pipeline for detecting and classifying celestial bodies and planets in astronomical imagery obtained from NASA and ESA archives.

### Methodology & Pipeline
- **Preprocessing:** Gaussian and median filtering, histogram equalization, CLAHE (Contrast Limited Adaptive Histogram Equalization), and background subtraction.
- **Segmentation & Detection:** Canny edge detection, morphological transforms, and OpenCV contour analysis.
- **Feature Extraction:** Extracted morphological descriptors, photometric stats, color histograms, and Gray-Level Co-occurrence Matrix (GLCM) texture features.
- **Classification:** Evaluated SVM (Support Vector Machines) and KNN (K-Nearest Neighbors) classifiers for multi-class planetary identification.

### Tech Stack
`Python` `OpenCV` `NumPy` `scikit-learn` `Matplotlib`
