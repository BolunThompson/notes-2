two options:
    1. if only octs up to level 0 need to be allocated
        then: calculate oct count from lone 1, 2s, etc in file at start
    2. if lower:
        above, then calculated number of zeros necessary
    3. or: just use dynamic array
    it is 2 probably
plan: use dynamic array, but calculate overflow to determine what is the issue / if it's something else
    realloc it in // REALLOC functions if necessary; prefer to realloc in EnzoEOctree.add method

