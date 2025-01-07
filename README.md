# Unexpected Immutability of Instance Variables in Ruby

This example demonstrates a common error in Ruby where instance variables appear immutable because a setter method is missing.  Attempting to modify the instance variable `@value` directly outside the class does not change its value.

The `bug.rb` file shows the incorrect code, while `bugSolution.rb` provides a corrected version that adds a setter method, resolving the issue.

## How to Reproduce
1. Run `bug.rb`.
2. Observe the output: The second `puts` statement will print 10, not 20, even though we tried to assign a new value.

## Solution
Add a setter method to allow modification of the instance variable from outside the class.