## Title
Octree Frontend for Enzo-E Astrophysics Simulation Code in yt Analysis Toolkit
## Abstract
Enzo-E is an octree-based astrophysics adaptive mesh refinement (AMR) simulation
code. yt is a Python package for the analysis and visualization of volumetric
data, including Enzo-E datasets. Enzo-E can generate datasets of size $2048^3$
blocks ($\approx 1$ TB). However, its corresponding front-end in yt suffers from
performance bottlenecks, leading to datasets of at most $256^3$ blocks
being practical to load.

The current frontend for Enzo-E in yt interprets the dataset as a collection of
grids. 

dw productivity

