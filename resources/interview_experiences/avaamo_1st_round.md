### Avaamo First Round Interview

1. TDD vs BDD
2. 
```ruby
2d_arr = [
  ["*", ".", ".", "*", ".", ".", "*", ".", "."],
  [".", "*", ".", ".", "*", ".", ".", "*", "."],
  ["*", ".", ".", "*", ".", ".", "*", ".", "."],
  [".", "*", ".", ".", "*", ".", ".", "*", "."]
]
```
Update all `"."` with the count of `"*"` touching its boundaries<br>
e.g., line 1 will become `["*", "2", "2", "*", "2" , "2", "*", "2" , "1"]`

3. STI - Single Table Inheritance. How does it identify which type is current object of. Any changes in table column to implement STI
4. NoSQL v SQL
5. How/why do we use DynamoDB
6. How can we improve API performance.
7. 
```
User (:id, :name)
Order (:id, :price, user_id: foreign_key)
```
Order table has 5 orders with prices: 100, 200, 300, 400, 400.<br>
Write SQL/ Active record query second largest order by price for user `"Shubham"`

8. `attr_accessor` question:
Suppose I have a class User and I want to create getter/ setter for a new attribute on the instance.<br>
How to do it manually, without using attr_accessor.

Using attr_accessor
```ruby
class User < ApplicationRecord
  attr_accessor :type_of_user
end

user = User.new
user.type_of_user = 'middle-aged'
puts user.type_of_user  # outputs 'middle-aged'
```

Without using attr_accessor
```ruby
class Example
  # Getter method
  def foo
    @foo
  end
  
  # Setter method
  def foo=(value)
    @foo = value
  end
end

class AnotherClass
  def set_and_get_foo
    example_instance = Example.new
    example_instance.foo = 42 # setter method to set value of foo
    puts example_instance.foo # getter method to get value of foo
  end
end

obj = AnotherClass.new
obj.set_and_get_foo   # Output will be 42
```
9. Monkey-patching/ Meta-programming
10. How is ruby hash implemented in the memory
11. Difference between `.each()` and `.map()`
