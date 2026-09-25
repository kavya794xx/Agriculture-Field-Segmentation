# Image Processing for Agriculture Field Segmentation

## Project Overview

This project focuses on agriculture field segmentation and crop percentage estimation using image processing and Support Vector Machine (SVM) classification.

The system works with four crop classes:

- Mirchi
- Cotton
- Paddy
- Sunflower

## Methodology

1. Agricultural image dataset collection
2. Image resizing to 64 × 64 pixels
3. BGR to RGB conversion
4. Pixel normalization
5. RGB feature extraction
6. SVM-based crop classification
7. RGB-based crop segmentation
8. Crop percentage estimation
9. FPGA-oriented data conversion
10. Vivado simulation

## Machine Learning

A linear SVM classifier with One-vs-One (OvO) classification is used.

For four crop classes, six binary classifiers are used.

Each 64 × 64 RGB image produces:

64 × 64 × 3 = 12,288 features

## FPGA-Oriented Implementation

The trained SVM parameters and image data are converted into FPGA-compatible formats.

Generated files include:

- `test_image.txt`
- `feature_mem.txt`
- `svm_weights.txt`
- `svm_bias.txt`

The hardware-oriented design is simulated using Vivado and Verilog HDL.

## Project Structure

```text
Agriculture-Field-Segmentation/
│
├── 4_2_project_report.pdf
├── README.md
│
└── python/
    └── agriculture_svm.py