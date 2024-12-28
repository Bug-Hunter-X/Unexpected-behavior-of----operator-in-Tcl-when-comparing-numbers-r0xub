# Tcl Bug: Unexpected behavior of == operator when comparing numbers

This repository demonstrates a common error in Tcl: the unexpected behavior of the `==` operator when comparing numbers.  Tcl's `==` operator performs string comparison, not numerical comparison. This can lead to subtle bugs in your code.  The example demonstrates the issue and its solution.

## Bug Description

The `badproc` procedure in `bug.tcl` is intended to check if two numbers are equal. However, due to the use of `==`, it performs a string comparison and yields unexpected results.

## Solution

The `bugSolution.tcl` file shows the corrected version, using the `eq` operator for numerical comparison. The `eq` operator performs a numerical comparison, correcting the behavior.

## How to reproduce

1. Clone this repository.
2. Run `tclsh bug.tcl` and observe the incorrect output.
3. Run `tclsh bugSolution.tcl` and observe the correct output.