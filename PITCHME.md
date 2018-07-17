# Introduction To Ruby
---
### Once you've learnt a programming language, you can pick up the next one much more easily.
Syntax is the main difference.
---
## Execution
- REPL (http://repl.it/)
- Interactive Ruby Shell (IRB)
- Execute Ruby File.
+++ 
### Get Familiar with the terminal!
---
## Display
+++
Javascript
```js
console.log("Hello world")
console.info("Goodbye world")
```
Ruby
```ruby
p "Hello world"
puts "Hello world"
print "Hello world"
```
---
## Variables
+++
Javascript
```js
let greetWorld = "Hello world"
const byeWorld = "Goodbye world"
```
Ruby
```ruby
greet_world = "Hello world"
BYE_WORLD = "Goodbye world"
```
---
## Commenting
+++
Javascript
```js
  // This is a javascript comment
```
Ruby
```ruby
  # This is a ruby comment
```
---
## Data Types
Ruby
- String 
```ruby
"Hello World" # => not unique
```
- Symbols
```ruby
:symbol # => unique
```
- Number(Integer, Float)
```ruby
100
1.2
```
+++
- Boolean
```ruby
true
false
```
- Array
```ruby
[1,"a", true]
```
- Hash
```ruby
{a: 1, b: 2}
```
+++
Javascript
```js
null
```
Ruby
```ruby
nil
```
+++
Unlike Javascript, only `false` and `nil` evaluate to falsy values.
+++
Creating arrays
```ruby
  [1,2,3]     # => [1,2,3]
  Array.new() # => []
```
Adding elements
```ruby
  array = []
  array << 1
  array.push(2)
```
+++
Creating hashes (symbol and strings are not the same)
```ruby
string_hash = {"a" => 1, "b" => 2}
symbol_hash = {a: 1, b:2} 
string_hash["a"]
symbol_hash[:b]
```
+++
Like a Javascript Object, Ruby Hash is a key-value pair and you access it in a similar way.
```ruby
hash = {a: 1, b: 2}
hash[:a] # => 1
```
+++
Be explicit about your types
```ruby
1 + "1" # => FAIL
1 + 1  # => ?
"1" + "1" # => ?
```
+++
### Converting types
```ruby
1.to_s
"2".to_i
```
---
## Control Flow
+++
### Conditionals
```ruby
if x > 5
  puts "greater than 5"
elsif x < 2
  puts "less than 2"
else
  puts "between 2 and 5"
end
```
+++
### Loops
- for (on interables only)
- while
```ruby
x = 0 
while x < 3 do
  p x 
  x += 1
end
```
- until
```ruby
x = 0
until x == 3 do
  p x 
  x += 1
end
```
+++
Strings, array and hashes are iterables
```ruby
  for x in [1,2,3,4,5] do
    p x
  end
```
---
### Methods 
Or as you're more familiar with: functions
+++
```ruby
def function_name(args)
  # Code block
end
```
+++
```ruby
def sum(num_1, num_2)
  num_1 + num_2
end

sum(1, 2) # => 3
```
+++
```ruby
def sum(num_1, num_2)
  return "Hello"
  num_1 + num_2
end
```