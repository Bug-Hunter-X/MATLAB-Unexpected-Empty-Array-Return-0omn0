# MATLAB Unexpected Empty Array Return

This repository demonstrates a common, yet often overlooked, error in MATLAB:  functions unexpectedly returning empty arrays ([]).  This issue can be subtle and lead to difficult-to-debug problems.

The `bug.m` file shows a function that, under certain conditions, returns an empty array.  The `bugSolution.m` file provides a solution to correctly handle the empty array return.

**Problem:**  MATLAB functions sometimes unintentionally return empty arrays.  If downstream code isn't designed to handle this case, errors or unexpected behavior can result.

**Solution:**  Check for empty arrays using `isempty()` before proceeding with operations that assume a non-empty result. Implement appropriate error handling or alternative logic to handle empty array cases gracefully.