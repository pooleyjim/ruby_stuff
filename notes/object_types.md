# Object types in Ruby.

Everything in Ruby is an object.

Objects can be thought of as real world items but also abstract items such as a conversation.

## Variables

Variables are an exception which are used to store or reference an object. Assign variables with understandable names and in lower case:

```ruby
my_first_variable = 1
my_second_variable = 2
```

### Variable Scopes:

Scope    | notation
---------|-----------
Global   | $var_name
Class    | @@var_name
Instance | @var_name
Local    | var_name
Block    | var_name

## Integers
Whole numbers that are sub-classed as 'Fixnum' or 'Bignum' for smaller or bigger numbers respectively. Ruby dynamically changes according to what is most memory efficient.

## Floats
Floating point or decimal numbers. Indicates that precision is important. 

*Integers divided by integers will result in an integer. Use floats if accuracy is important.*

## Strings
A series of mixed characters between double or single quotes. Single quotes will mean ruby takes that content literally, double quotes will have added expansion. 

To quote a variable and apply methods:
```ruby
my_first_variable="woo"
"My first variable is #{my_first_variable}".upcase
=> "MY FIRST VARIABLE IS WOO"
```

## Array
An ordered list of values. Defined like so:
```ruby
my_first_array = [ 1, 2.0, "three" ]
```
Indexing starts from zero. Pull from array:
```ruby
my_first_array[0]
 => 1
```
Edit particular items in array position:
```ruby
my_first_array[0] = 5
 => 5
my_first_array
 => [5, 2.0, "three"]
```
Append to with double less than:
```ruby
my_first_array << 6
 => [5, 2.0, "three", 6]
```
Items in array can be mixed types.

## Some Array methods

inspect - returns array as string.<br>
to_s - joins content of array into string.<br>
join(",") - joins an array but splits each element with comma.<br>
split(",") - creates an array splitting each element at the comma.<br>
reverse - print array in reverse.<br>
sort - simple sort.<br>
uniq - new array with unique values.<br>

Add exclamation mark with methods to edit in line.

delete_at(n) - delete at position n.<br>
delete(value) - deletes "value" from array and returns it.<br>
push(arg) - add "arg" to end of array.<br>
pop - returns and removes the last element of the array.<br>
shift and unshift - same as push and pop but for first element.<br>
You can add arrays together with '+'.<br>

You can search for extra methods in docs.

## Hash

Hashes are object-indexed unordered collection of objects i.e. a collection of key=value pairs.

Create a hash:
```ruby
my_first_hash = { 'key1' => 'value1', 'key2' => 'value2' }
```

Pull from hash by key:
```ruby
my_first_hash['key1']

Pull from hash by value:
```ruby
my_first_hash.index('value2')
```

Hashes can be a mix of object types.

*methods:*
keys - returns keys.
values - returns values.
length - returns length.
size - returns size.
to_a - turn each element of hash into an array and the hash as a whole into an array.
clear - empty the hash.
Add to:
```ruby
my_first_hash['key3'] = 'value3'
```

## Symbols
Defined with colon followed by string e.g.:
```ruby
:my_first_symbol
```
Object id does not change for symbols. Useful inside of hashes:
```ruby
my_first_hash = { :key1 => 'value1', :key2 => 'value2' }
```
Quote with:
```ruby
my_first_hash[:key1]
```

Labels cannot be assigned a value like a variable. Rule of thumb, if needed for output use string otherwise consider label.

## Booleans
Either true or false.

Comparisons:

Test                     |Operator
-------------------------|---------
Equal                    | ==
Less than                | <
Greater than             | >
Less than or equal to    | <=
Greater than or equal to | >=
Not                      | !
Not equal                | !=
And                      | &&
Or                       | \|\|

Question marks can be used after a lot of methods to test. Examples:
```ruby
x.nil?
x.between?(1,10)
x.empty?
array.include?(1)
hash.has_key?('key1')
hash.has_key?(:key2)
hash.has_value?(value1)
```

## Ranges
Two kinds:

Inclusive
```ruby
1..10
1,2,3,4,5,6,7,8,9,10
```
Exclusive
```ruby
1...10
1,2,3,4,5,6,7,8,9
```
Methods:
```ruby
begin
end
first
last
include?
[*1..10] - * is 'splat' - to expand
```

## Constants
Similar to variables in that:
- Not true objects
- Pointers to objects

Different to variables:
- Constants are *constant* i.e. they do not change

Define a constant with all caps. 
```ruby
CONSTANT = 1
Also_a_constant = 2
variable = 3
```
