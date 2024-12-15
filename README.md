# Off-by-one Error in Dart List Iteration

This repository demonstrates a common off-by-one error in Dart when iterating over a list.  The error occurs because the loop attempts to access an index that is outside the valid range of indices for the list. This can lead to an `IndexOutOfRangeException`.

The `bug.dart` file contains the code with the error.  The `bugSolution.dart` file shows the corrected code.

## How to reproduce

1. Clone this repository.
2. Run `bug.dart`. You will observe an error.
3. Run `bugSolution.dart`. The code will run without error, correctly summing the numbers in the list.

## Solution

The solution involves correcting the loop condition to iterate up to, but not including, `numbers.length`.  This ensures that the loop does not attempt to access an index that is out of bounds.