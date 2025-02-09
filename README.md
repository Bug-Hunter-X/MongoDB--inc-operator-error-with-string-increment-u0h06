# MongoDB $inc operator error with string increment
This example demonstrates an incorrect usage of the `$inc` operator in a MongoDB update query.  The issue arises from attempting to increment a numerical field with a string value.

The `$inc` operator is designed to increment a numerical field by a specified amount.  Providing a string value instead causes the operation to fail silently or result in unexpected behavior, depending on the MongoDB version and configuration. 

**Bug:** Incorrect use of `$inc` with a string value.

**Solution:** Use the correct data type (integer or number) for the increment value.