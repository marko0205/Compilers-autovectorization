# Compilers-autovectorization
This is a course project of HPC by university of Salerno

Updated version of TSVC test suite. The original paper which laid out the details of the suite and provided results (D. Callahan, J. Dongarra, and D. Levine. Vectorizing compilers: a test suite and results. Proceedings. Supercomputing ’88) originally had the loops in Fortran.


## Optimizations

This reposority is the subject of a study on the vectorization of the GCC 12 and LLVM 14 compilers, some loops that were not automatically vectorized have been optimized with the openMP library and through code transformation.

For more information about how the repository check the doc: A Reseach on Compilers Auto Vectorization.pdf

## Compiling

To compile the code, modify the makefile corresponding to the compilers to use, selecting the desired version of the compiler

For example, with the GNU compiler:

    make COMPILER=GNU

This will create a folder called `bin/GNU/` with vectorised and non vectorised versions of the program.


