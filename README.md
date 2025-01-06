# Groovy Null Pointer Exception Handling

This example demonstrates a common issue in Groovy related to null pointer exceptions when dealing with function parameters.  Groovy's loose typing can sometimes lead to unexpected behavior if null values aren't explicitly handled.  The solution provides a robust approach to gracefully manage null inputs.

**Bug:** The original `calculate` function doesn't explicitly handle `null` values. If either `a` or `b` is `null`, a `NullPointerException` occurs in the `a + b` operation.

**Solution:** The improved version includes an explicit check for `null` values. If either parameter is `null`, the function returns 0.  This prevents the exception and provides a more predictable result.