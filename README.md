# Off-by-One Error in Java Array
This repository demonstrates a common off-by-one error in Java when iterating over arrays. The `BuggyArray.java` file contains the erroneous code, which attempts to access an array element beyond its valid index. The `FixedArray.java` file provides the corrected code.  This is a subtle but frequently encountered error in programming that can lead to unexpected crashes or incorrect results.

**How to reproduce the bug:**
1. Compile and run `BuggyArray.java`. 
2. Observe the `ArrayIndexOutOfBoundsException` that occurs.

**Solution:**
The correct way to iterate is to use `< arr.length`, ensuring you don't attempt to access the element beyond the last valid index.