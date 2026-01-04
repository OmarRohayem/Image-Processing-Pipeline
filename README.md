# Image Processing & Analysis Pipeline

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green.svg)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

## 📌 Overview
This project implements a complete image processing pipeline using Python and OpenCV. The solver accepts an input image and performs a sequence of enhancement, analysis, and feature extraction tasks. 

This repository was designed to demonstrate fundamental Computer Vision concepts including Power-Law transformations, spatial filtering, and texture analysis.

## 🚀 Features

The pipeline is divided into three distinct tasks:

### Task 1: Image Enhancement
- **Gamma Correction:** Applies Power-Law transformation to adjust image luminance.
- **Histogram Analysis:** Generates and compares histograms before and after correction to visualize intensity shifts.

### Task 2: Noise Reduction & Edge Detection
- **Median Filtering:** Applied to remove salt-and-pepper noise while preserving edge data.
- **Laplacian Operator:** Calculates the second derivative of the image to highlight regions of rapid intensity change (edges).

### Task 3: Segmentation & Feature Extraction
- **Otsu's Thresholding:** Automatically calculates the optimal threshold value to binarize the image.
- **Morphological Operations:** Uses Closing (Dilation followed by Erosion) to fill gaps in detected objects.
- **Feature Extraction:** Calculates:
  - **Geometric:** Area, Perimeter, Aspect Ratio, Extent.
  - **Statistical:** Mean Intensity, Standard Deviation.
  - **Texture (GLCM):** Contrast, Energy, Homogeneity, Correlation.

## 🛠️ Dependencies

* Python 3.x
* OpenCV (`cv2`)
* NumPy
* Matplotlib
* Scikit-Image (`skimage`)

## 💻 Usage

**Note:** This notebook is optimized for **Google Colab** as it utilizes `google.colab.files` for image uploading.

1.  Open the notebook in Google Colab.
2.  Run the cells sequentially.
3.  When prompted, upload an image from your local machine.
4.  The system will output a series of comparison plots and a dictionary of extracted features.

## 📊 Example Output

The script generates 2x2 comparison grids for every stage of processing to allow for immediate visual verification of the algorithms applied.

---
*Created by [Omar Rohayem].
