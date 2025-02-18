# Tcl String Comparison Bug

This repository demonstrates a subtle bug in Tcl related to string comparison and empty strings. The `badproc` procedure in `bug.tcl` incorrectly handles empty string inputs when using the `==` operator for comparison. The `bugSolution.tcl` file provides a corrected version.

## Bug Description
The original `badproc` procedure uses `==` to compare two strings.  This operator behaves unexpectedly when one or both strings are empty. This can lead to incorrect results or unexpected behavior in the calling code.

## Solution
The corrected procedure in `bugSolution.tcl` uses the `eq` operator for string comparison, which handles empty strings correctly.