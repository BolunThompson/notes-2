why can't block-structured data,  an octree , just use the octree frontend
    inconsistent refinement: each block is the most refined portion, but some are more refined than others
    
what am I optimizing for: initial load speed (that is, build index speed), but if other things get faster than it would be good

# format notes
block: A block string consisting of (0, 1), with optionally one colon. The
    number of digits after the colon is the refinement level. The combined
    digits denote the binary representation of the left edge.
endianess: idk?


# todo:
1. dw Will Hicks email
3. dw paperwork (by friday EOD) & retirement
2. dw slack issue
4. read over yt paper / continue on fake alternative frontend pr / read over enzo-e/cello documentation / read over yt octree code / etc
# code plan
convert enzo-e frontend patch based system to an array of octree subsets, using "partial_coverage" to inconsistenly refine the blocks

questions:
what is a zone?
    - is it just a subset of a block which I don't need to care about? <- current suspiscion
# slack oref change 
assuming zone = cell
old: oref is n where 2^n = zones per dimension
new: oref is the number of zone/cells
nz = oref
factor to cell width = 1/(nz^1/3)
factor from cell width = nz^1/3
## call questions
what is the difference between a zone and a cell, ignoring ghose zones


