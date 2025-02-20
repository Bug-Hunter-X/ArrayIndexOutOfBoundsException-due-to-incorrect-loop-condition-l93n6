# Java Bug: ArrayIndexOutOfBoundsException

This repository demonstrates a common Java error: an `ArrayIndexOutOfBoundsException` caused by an off-by-one error in a for loop.

The `bug.java` file contains the buggy code. The `bugSolution.java` file provides the corrected version.

## Problem

The original code attempts to sum the elements of an array. However, the for loop's condition `i <= arr.length` causes an `ArrayIndexOutOfBoundsException` because array indices start at 0 and end at `arr.length - 1`. Accessing `arr[arr.length]` attempts to access an element beyond the array's bounds.

## Solution

The corrected code in `bugSolution.java` uses the condition `i < arr.length` to prevent the out-of-bounds access. This ensures the loop iterates correctly through all elements of the array.