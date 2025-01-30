# MongoDB $inc Operator Error: Incorrect Usage with String Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numerical field by a specified value.  However, providing a string value to `$inc` will result in an error.

## Bug
The `bug.js` file contains a MongoDB update query that attempts to increment a field using a string value as the increment.

## Solution
The `bugSolution.js` file shows the correct usage, using a numeric value instead of a string to increment the field.

## How to reproduce the bug
1.  Ensure you have a MongoDB instance running.
2.  Create a collection called `myCollection`.
3.  Insert a document with an `_id` of 1.
4.  Run the code in `bug.js`.

You'll encounter an error because you're attempting to increment using a string value.