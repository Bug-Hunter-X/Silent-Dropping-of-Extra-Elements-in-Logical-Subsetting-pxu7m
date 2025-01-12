# R Silent Subsetting Bug

This repository demonstrates a subtle bug in R's subsetting mechanism. When you use a logical vector longer than the number of rows in a data frame for subsetting, R silently drops the extra elements. This can lead to unexpected behavior and make debugging difficult. 

The `bug.R` file contains the problematic code. The `bugSolution.R` file offers a solution using error checking to prevent the unexpected behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.R`.
3. Run the R script. Note that no error is raised, but the result is likely not what you expect. 
4. Open `bugSolution.R` to see a corrected version of the code.