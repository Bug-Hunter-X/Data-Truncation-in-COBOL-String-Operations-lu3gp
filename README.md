# COBOL Data Truncation Bug

This repository demonstrates a common error in COBOL programs: data truncation during string manipulation. The `bug.cob` file contains a program that might truncate data if the input string is longer than the defined area.  The `bugSolution.cob` file shows how to mitigate this issue.  This is a crucial consideration when dealing with variable-length data in COBOL, as failure to handle data lengths correctly can lead to subtle and hard-to-debug problems.

## Reproducing the Bug

1. Compile and run `bug.cob`.
2. Modify the input string ('Hello, world!') to be longer than 100 characters.
3. Observe that the output is truncated, possibly leading to unexpected results.

## Solution

The solution involves carefully considering the maximum string lengths and using appropriate techniques to handle potential truncation, as shown in `bugSolution.cob`.