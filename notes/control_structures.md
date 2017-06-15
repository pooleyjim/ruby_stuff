# Control Structures

## Conditionals

### If
If statements defined with:
```ruby
if boolean test
  ...
elsif another boolean test
  ...
else
  ...
end
```

Another quick if:
```ruby
print "action" if test == "true"
```

### Others
- unless:
```ruby
unless boolean_test
  ...
end
```
Unless boolean test is true do something. Another way using if:
```ruby
if !boolean_test
  ...
end
```
- case
Useful when there are lots of conditionals:
```ruby
case test_value
when value
  ...
when value
  ...
end
```   
- ternary operator
Shortcut for simple if/else:
```ruby
boolean ? code1 : code2
```
- or/or-equals
Shortcut for:
```ruby
if a
  b = a
else
  b = c
end
```
Would be:
```ruby
b = a || c
```
Another shortcut:
```ruby
unless a
  a = b
end
```
would be
```ruby
a ||= b
```

### loops
Define a loop:
```ruby
loop do
  ...
end
```
There needs to be controls over loops else they may continue infinitely. These are:
- break = Terminate the entire loop
- next = Jump to next loop
- redo = redo loop
- retry = start the whole loop over
```ruby
loop do
  do stuff
  break if boolean_test
  next if anther_test
end
```
There are also while and until with the breaks built in.
```ruby
while boolean_test
  do stuff
end
```
While boolean_test returns true do stuff.
```ruby
until boolean_test
  do stuff
end
```
Until boolean_test is true do stuff.

### Iterators
Perform action for each value input.
Example:
```ruby
5.times do
  puts "Huzzah!"
end

1.upto(5) do |num|
  puts "Huzzah!"
end

5.downto(1) do { puts "Huzzah!" }
```
Lots of methods that can be used as iterators on diffirent object types. Check docs.
