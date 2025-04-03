# 331AI
# AIML331 Assignment 1 - Computer Vision Fundamentals

## Overview
This repository contains my implementation for Assignment 1 of AIML331 2025 at Victoria University of Wellington. The assignment focuses on fundamental computer vision concepts including camera transformations, image processing, and histogram manipulation techniques.

## Problem Description

### 1. Camera Problem (15 points)
- **1.1:** Computing the [R,t] transformation matrix for a pinhole camera positioned at [0,0,-10] and pointing 30 degrees to the right of the world coordinate origin.
- **1.2:** Using homogeneous coordinates to find the equation of a line on the projective plane passing through projected points.

### 2. Checkerboard Problem (30 points)
- **2.1:** Finding and converting a checkerboard image to grayscale
- **2.2:** Computing image histogram and cumulative probability function
- **2.3:** Implementing low-pass filtering in the spatial domain
- **2.4:** Analysis of filter separability
- **2.5:** Implementing the same low-pass filter in the frequency domain
- **2.6:** Computing the histogram of the filtered image
- **2.7:** Using cumulative distribution functions to achieve uniform intensity distribution

## Repository Structure
```
.
├── README.md                 # This file
├── camera_transforms.py      # Implementation for Problem 1
├── checkerboard_processing/
│   ├── image_acquisition.py  # Code for finding and converting checkerboard image
│   ├── histogram.py          # Histogram and CDF implementation
│   ├── spatial_filter.py     # Spatial domain filtering
│   ├── frequency_filter.py   # Frequency domain filtering
│   └── histogram_equalize.py # Histogram equalization
├── images/                   # Directory for storing input/output images
└── report.pdf                # Final report with explanations and results
```

## Requirements
- Python 3.8+
- NumPy
- Minimal external libraries (only file handling and NumPy, except for DFT/FFT)

## Usage
Each component can be run independently:

## Implementation Notes
- All code is written from scratch as per assignment requirements
- The camera transformation uses standard pinhole camera model
- The checkerboard processing uses a Gaussian filter for low-pass filtering
- The implementation minimizes external library dependencies

## Report
The accompanying pdf contains:
- Detailed explanation of all implemented solutions
- Mathematical derivations for camera transformations
- Analysis of filter separability
- Comparison of spatial vs. frequency domain filtering
- Visualization of histograms and processing results

## References
- Lecture notes from AIML331 2025
- Szeliski, R. (2022). Computer Vision: Algorithms and Applications
- Prince, S. J. (2012). Computer Vision: Models, Learning, and Inference
