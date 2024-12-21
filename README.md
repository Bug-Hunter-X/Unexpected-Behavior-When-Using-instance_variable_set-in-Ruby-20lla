# Unexpected Behavior When Using instance_variable_set in Ruby

This example demonstrates a potential issue when using `instance_variable_set` in Ruby. Directly modifying an object's internal state using this method can lead to unexpected behavior if not carefully managed. This is especially true in larger codebases or when multiple parts of the code interact with the same object.  The example shows how modifying the instance variable `@value` directly via `instance_variable_set` bypasses any potential validation or logic that might be present in a standard accessor method.  Best practice is to use accessor methods, ensuring that data is handled consistently across the code. 