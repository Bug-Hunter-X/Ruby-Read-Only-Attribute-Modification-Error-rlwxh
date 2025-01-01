# Ruby Read-Only Attribute Modification Error

This repository demonstrates a common error in Ruby when dealing with attributes that are implicitly read-only due to the lack of a setter method.  The `bug.rb` file contains the erroneous code, while `bugSolution.rb` provides a corrected version.

The issue arises when trying to modify an attribute that only has a getter method defined.  Ruby will raise a `NoMethodError` in this situation, as it cannot find a method to handle the assignment.

The solution involves explicitly defining a setter method (`value=`) to allow modification of the attribute.