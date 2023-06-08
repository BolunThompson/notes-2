HYPERION CODE IS CORRECT
Example Code does not work, proving that point (also seg faults?)
    could haeve messed smtn up
fake_octere_ds works so load_octree is not bad

224945 = len(ref)
form len(ref): if (n_octs - 1) * 8 + 1: n_octs = 28119

from files: nocts = 21821

ref_octs * 8 + nocts = len(ref)
nocts is known

inconsistencies:
    (n_octs - 1) * 8 + 1 produces 3 octs for below, but I count two (or ten?) depending on what is an oct
        [True,
             False,
             False,
             True,
               False,
               False,
               False,
               False,
               False,
               False,
               False,
               False,
             False,
             False,
             False,
             False,
             False,
         ]
    example from load_octree does not have 8 child octs per refined octs


QUESTION:
What is the format of the octree_mask? If it's the format as in the hyperion docs, what is the n_octs thing in the docs? I assume it must be wrong, right?
If this is wrong: sort through the recursive_octree code

If what I'm doing is correct:
sort through recursively_visit_octs and figure something out

True
    False
    False
    False
    False
    True
        False
        True
            False
            False
            False
            False
            False
            False
            False
            False
        True
            False
            False
            False
            False
            False
            False
            False
            False
example does meet rule w/ octs being # of true / more refined

depth first octree (or breadth first? search)
step 1.: octree not assuming # of zones

I actually need to make my octree code less shit b/c it will be transplanted
octree represented by bitstrings for each root node 

two passes:
    first pass to get root node / leaf node # (save in mode code)
        first goal is to get ^ working by loading it using frontend frontend then transplanting that code into yt
    second pass to load the data on demand
sparse octree for nodes
    key value pairs somehere

goal is to eventually iterate over h5 files in "data centered" way instead of how it is in memory

each oct node contains two spatial or pointers to other memory
    first for look up hash table to its file
    second one is an offset
not necessary for a file to contain an entire root node and its file

TODO:
    1. Finish Issue
    2. Finish other tasks
    3. Submit issue for segfaulting w/ weird load_octree values -- suspiscion is with nz pr
    4. submit documentation pr

should it be 8 or 1?
