# YT Enzo-E Octree Research Plan
{Authors}
## Notes
### Steps for YT
1. Write front-end for YT to load Enzo-E data in an octree format
2. If extra time: optimize the front-end so that it can be used in the real world
3. Demonstrate that the octree frontend can be used in a real-world style problem
    - Halo finding?
4. Perhaps write an octree frontend for FLASH and GAMER formats?
### Additional Goals
1. Go through ML Workshops
    - Perhaps complete a project using ML? Although I don't want to try to find
        a project for a technology.
2. Complete REU material
### Todo
What should I include?
    Look at old papers or research plans about it?
    Should I include a summary?
        No -- it should be short enough that it is unnecessary
        The purpose is basically it
    Should I include a background?
        Maybe? Will people unfamiliar with the project actually read it
            Is it necessary after the purpose?
        If i do should it include the history of work on this?
    Should I include a timeline?
        Maybe? Will they want it? Idc
    Should I detail the work that has already been done?
## Purpose (ie: abstract)
`yt` is a software package for the analysis of volumetric data. It can interpret
data in a varietry of formats; of note here, patch-based adaptive mesh
refinement (AMR) grids and octree-based AMR. Enzo-E is a parallel
array-of-octree AMR application which can run highly scalable simulations for
the investigation of processes such as the formation of stars and galaxies.
`yt` currently interprets Enzo-E data in a patch-based format, despite the data
natively being octree-based. The purpose of this project is to write a frontend
usable in the real-world to load Enzo-E data into `yt` in an octree-based
format. A further goal would be to write front-ends to load FLASH and Gamer,
other octree-based simulaton codes, as octrees into `yt`, instead of as
patch-based data.
## Objectives
1. Prepare `yt` octree ?
2. Prep scripts (detail ?
1. Write a front-end for `yt` to load Enzo-E data in an octree format
2. Optimize the front-end so that it can be used in the real world
3. Demonstrate that the octree frontend can be used in a real-world style problem
    - Halo finding?
4. Write an octree frontend for FLASH and GAMER formats, and repeat the above
   process
