# All versions of the pph program in C

## pph_in_C/
    The first version of the pph program

## pph_in_C_v02/
    The second version of pph. Now the filtration is loaded 
    from an external file and not more created by taking all combinations.
    The regular paths are created previously by taking cartesian products
    on the relational database supported by sqlite3

## pph_in_C_optimized_O1/
    The third version of pph where I have implemented some optimizations.
    Firstly, the weight matrix of the user's graph is loaded only once,
    avoiding unnecessary communication with the hard disk.
    Secondly, now part of the code is paralelized. That is, the calculation
    of the path persistent homology, for dimensions 0 and 1, are made in paralell,
    with the help of the 'pthreads' library.
