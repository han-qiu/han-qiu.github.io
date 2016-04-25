---
layout: post
title: "opencv functions"
publish: true
---
### solvePnP

Finds an object pose from 3D-2D point correspondences.

C++: bool solvePnP(InputArray objectPoints, InputArray imagePoints, InputArray cameraMatrix, InputArray distCoeffs, OutputArray rvec, OutputArray tvec, bool useExtrinsicGuess=false, int flags=ITERATIVE )
