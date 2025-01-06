# F# Mutable Variable Swap Bug

This example demonstrates unexpected behavior when using mutable variables in F# to swap two values within a function. The `swap` function, designed to swap the values of `x` and `y`, does not produce the intended result. The issue lies in the scope of the mutable variables within the function.

## How to reproduce the bug:
1. Compile and run the provided `bug.fs` file.
2. Observe that the output is not the expected swapped values of `x` and `y`.

## Solution:
The solution (`bugSolution.fs`) demonstrates the correct approach to swapping mutable variables in F# by using `let` bindings to create new values instead of modifying the existing ones directly in the function. This approach correctly swaps the values and avoids the confusion caused by mutable variables. 
