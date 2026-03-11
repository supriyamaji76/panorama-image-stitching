# Panorama Image Stitching in C++ (OpenCV)

A C++ implementation of a **Panorama Image Stitching Pipeline** using OpenCV.  
The system automatically stitches multiple overlapping images into a single seamless panorama.

This project demonstrates core **computer vision algorithms** used in real-world applications such as robotics, autonomous vehicles, mapping systems, and AR/VR.

---

## Features

- Feature detection using **ORB / SIFT**
- Feature matching between images
- Homography estimation
- Camera parameter estimation
- Bundle adjustment for alignment optimization
- Image warping (spherical / cylindrical projections)
- Exposure compensation
- Seam finding
- Multi-band image blending

---

## Panorama Stitching Pipeline

The following pipeline is implemented in this project:

Input Images
↓
Feature Detection
↓
Feature Matching
↓
Homography Estimation
↓
Bundle Adjustment
↓
Image Warping
↓
Exposure Compensation
↓
Seam Finding
↓
Multi-band Blending
↓
Final Panorama

This pipeline is similar to the architecture used in **OpenCV’s internal Stitcher implementation**.

---

## Requirements

- C++17
- OpenCV 4.x
- CMake

---

## Install Dependencies (Mac)

Install OpenCV using Homebrew:

---

## Build the Project

mkdir build
cd build
cmake ..
make

---

## Run the Panorama Stitcher

./panorama ../images/a1.png ../images/a2.png ../images/a3.png
