# JavaScript Type Coercion with the + Operator

This example demonstrates a common issue in JavaScript related to type coercion with the `+` operator.  The `+` operator is overloaded; it performs addition for numbers and concatenation for strings.  When used with a mix of number and string types, it can lead to unexpected results.

## Bug
The `foo` function intends to add two numbers. However, when a string is passed as an argument, it concatenates instead of adding.

## Solution
The solution uses `parseInt()` to explicitly convert the string to a number before the addition operation, ensuring consistent behavior.