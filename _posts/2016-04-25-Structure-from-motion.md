---
layout: post
title: "Structure from motion"
publish: true
---
### Affine ambituity

decomposition is not unique. M->MC, S->C^-1S

m images and n features

for each image i, center the feature coordinates

Construct a

### Sequential structure from motion

Initialize motion from two

images using fundamental matrix

For each additional view

Determine projection matrix of new camera using all known 3D points that are visible
in its image-calibration

Refine and extend structure: compute new 3D points, re-optimize existing points that are

### Bundle adjustment(光束平差法)

E(P,X) =

- Minimize sum of square reprojection errors

- Handle large number of views
- Handle missing data

- Limitations: Large minimization problem
- Require good initial condition

- Used as the final step of SFM
- Factorization or algebraic approaches

###
