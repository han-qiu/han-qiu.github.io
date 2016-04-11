---
layout: post
title: "Camera Calibration"
publish: true
---

### Pinhole Camera Model
P = M_in*M_out*P

- Extrinsic parameters(R,T)

Rotation and Translation

- Intrinsic parameter(f)

P' = MP_w = K[R T]P_w

intrinsic parameter:

### Goal of Calibration

Estimate intrinsic and extrinsic parameters from 1 or multiple images

mainly intrinsic parameter

- Extrinsic

p_1,...,p_n with known position

the precision of parameter usually gain .1 the precision of points

### Calibration
- Known calibration object, many views
- Compute intrinsic and extrinsic
- Retain intrinsic, toss extrinsic

### Harris Corner Detection

### Direct linear calibration - homogeneous

### Perspective Camera Model(nonlinear)

### The calibration problem
- Given
  1. Calibration pattern with N corners
  2. K

### calibration questions
- Can we determine the intrinsic parameters by exposing the camera to many known object?

### Calibration by nonlinear Least Squares
- Least Mean Square
- Gradient Descent

### How many corners and how many views
4 instrinsic(distortion:+2)
6K extrinsics:
2NK >= 6K+4

(N-3)*K >= 2

### Problem with least Squares
- Many
-

### Multiple-plane
*IEEE:A flexible new technique for camera calibration*
has been implemented in opencv

Easy to implement calibration technique

- It only requires a planar pattern
- Images at a few orientations
- Motions need not be known

Radial lens distortion modeled

###  Homography and image Anignment(Algorithms and applications)

### Motivation: Mosaics

### Homography

- Geometric Transformations

- General Affine
- Homogeneous Transformations
- *planar Perspective transformations*

### Homography
- How to relate two images from the same camera center?
- e.g.: camera rotation, different camera to capture the same plane.

### Analysing patterns and shapes

### Building panorama

Can't create a 360 degree of panorama:(Because it's based on plane)

You can use spherical plane instead to create a 360 degree of panorama

### Image warping with homographies

### Image Alignment Algorithm

Given images A and B

1. Compute image features for A and B
2. Matching features between A and B
3.

we can use RANSAC Algorithm to prevent wrong matches

Froward Warping

What if pixel lands "between" two pixels ?

Inverse Warping

resample values from interpolated image

Possible interpolation filters:

- nearest neighnor
- bilinear
- bicubic
- sinc

- Need to prevent jaggies

### Blending

to erase the edge of merging

Feathering

Alpha Blending

- Mapping to a cylindrical surface

Cylindrical Projection

### Readings
F&P

Szeliski,CAAA
