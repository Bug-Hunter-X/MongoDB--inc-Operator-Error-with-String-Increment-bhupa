# MongoDB $inc Operator Error with String Increment
This example demonstrates an error in MongoDB update operations using the $inc operator with a string value instead of a number. The $inc operator is designed to increment numerical values and passing a string results in unexpected behavior.

## Bug Description
The code uses the $inc operator with a string ('1') instead of a number (1) when updating the `count` field.  This incorrect usage may result in failure, unexpected values or silent data corruption.

## Bug Solution
The correct code below shows how to use the $inc operator to increment a numerical field.  Ensure the value you pass is an integer or a floating-point number, not a string.