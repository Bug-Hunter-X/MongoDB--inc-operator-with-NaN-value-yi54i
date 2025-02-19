# MongoDB $inc Operator with NaN Value
This example demonstrates an uncommon error in MongoDB when using the $inc operator with a NaN value. The $inc operator is used to increment a numerical field by a specified value. However, if you try to use NaN (Not a Number) with $inc, it will result in an error because NaN cannot be used in numerical operations.

## Bug
The bug is in the usage of the $inc operator. The provided code attempts to increment the 'counter' field by NaN, leading to an error.

## Solution
To fix this, ensure that the value being used with $inc is a valid number. Replacing NaN with a numerical value resolves this issue.