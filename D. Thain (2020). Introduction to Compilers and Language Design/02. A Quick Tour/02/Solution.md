# Statement
Determine how to change the optimization level for your local com-
piler. Find a non-trivial source program and compile it at multiple
levels of optimization. How does the compile time, program size,
and run time vary with optimization levels?
# Solution
Compiler optimizations for `gcc`:
- `-O0` (default): Reduce compilation time.
- `-O1` (`-O`): Reduces code size and execution time.
- `-O2`: Further reduces execution time but increases compilation time.
- `-O3`: Further reduces execution time but increases compilation time.
- `-Os`: Similar to `-O2` but prioritizes code size.
- `-Oz`: Further reduces code size.