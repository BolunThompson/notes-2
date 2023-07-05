---
bibliography: "2023-reu-research_plan.bib"
csl: "yt.csl"

title: "Octree Frontend for Enzo-E in YT"
author: 
    - Bolun Thompson:
        institute: "REU FoDoMMaT Visiting Scholar"
    - Matthew Turk:
        institute: "Assistant Professor at the School of Information Sciences"
date: "July 6th, 2023"
---

# Volumetric Simulations
- Formation of stars and galaxies
- Nuclear reactor mechanics

# Why?
Connects theories with data

# What
- Enzo: **Adaptive Mesh Refinement** (AMR) astrophysical simulation code
    [@Bryan_2014]
    - Multi-purpose
- Adaptive Mesh Refinement
    - Increase simulation accuracy in turbulent or interesting parts
    - Inconsistent

![Patch-based AMR [@turk]](block_selection.svg){ height=50% width=50% }

# Enzo-E
- Enzo-E: Rearchitecture of Enzo for exascale computing [@bordner2018]
    - Datasets $>2048^3$ blocks ($>1$ TB)
<!-- - {if time mention Cello} -->
- Uses **array-of-octree** AMR
- Octree
    - Tree data structure to represent 3D space
    - Recursively subdivided
- Array-of-octree
    - 3D Array of Octrees
    - Easily parallelizable

![AMR Quadtree [@dunning2020]](block_amr.png){ height=50% width=50% }

# yt
- yt: Python analysis and visualization package [@turk]
- For any type of volumetric data 
    - Both Enzo and Enzo-E

---
:::::::::::::: {.columns}

::: {.column width="50%"}
![Slice over z axis of density](galaxy0030_Slice_z_density.png)
:::

::: {.column width="50%"}
![3D visualization of density](galaxy0030_3dviz.png){ height=85% width=85% }
:::

::::::::::::::



# Frontends
- yt supports a variety of **frontends** to load data
- Frontends can be implement in various formats
    - Grid-based
        - Inconsistent across the domain 
    - Array-of-octree

# Problem
Enzo-E analysis in yt is slow!

# Problem
- Slow on large datasets
- Can't practically analyze enzo-e datasets of over $256^3$ blocks
    - $256^3$ blocks → multiple hours to load in the data
- Needs to analyze datasets of size $2048^3$ blocks
    - $\approx 1$ TB

# Current Frontend
- Collection of grids
    - Each grid is a python object
        - $\approx 1$ KB
- Largely single threaded

# New frontend
- Array of Octree
- Multithreaded
- Each Oct is a C struct
    - At most 88 bytes

# Result
- Faster
- Can analyze datasets of size $2048^3$ blocks
    - $\approx 1$ TB

# Current Status
- New frontend is partially built
- Non refined data can be loaded in

![Incorrect visualization. The "Hi" is mirrored and rotated from what it should
  be.](new2.jpg){ height=50% width=50% }

# Future Work
- New frontend is unoptimized
    - Initially slower
- Other simulation codes interpreted as grid-based, instead of oct-based

# References {.allowframebreaks}
