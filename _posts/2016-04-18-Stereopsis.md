---
layout: post
title: "stereopsis"
publish: true
---

### Why Stereo Vision?

2D images project 3D points into 2D

3D points on the same viewing line have the same 2D image

3D imaging results in depth information loss

Refers to the ability of :

The ability to infer information on the 3D structure and distance of a scene from two or more images taken from different points of view.

### Application: Face Modeling
From one stereo pair to 3D head model.

Z-keying: mix live  and synthetic

### Triangulation

Depth can be recovered with two images and Triangulation.

### Problems

- Correspondence Problem
  - Determine which pixel on the left corresponds to which pixel on the right

- Reconstruction Problem
  - Given a number of correspondence pairs and camera geometry information, find location and 3D geometry information, find location and 3D structure of the observed objects

### Find correspondences:

### 3D Reconstruction

### Epilolar Geometry

- Depth can be reconstructed based on corresponding points(disparity)

- Finding corresponding points is hard & computationally expensive

- Epipolar Geometry helps to significantly reduce search from 2D to 1-D

### Epipolar
Op*[OO'×O'p'] = 0

### The Essential Matrix

Matrix that relates image of point in one camera to a second camera, given translation
and rotation.

Assumes cameras are calibrated(intrinsic parameters and known)

5 independent parameters.

### What if Camera Calibration is unknown

u^T F u' = 0 => F = K^-T \epsilon K^-1

F has 7 parameters up to scale and can be estimated from 7 point correspondence

### The normalized eight-point algorithm

### Stereo image rectification

### Stereo correspondence algorithm
