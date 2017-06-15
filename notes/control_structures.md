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
