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

inspect - returns array as string.
to_s - joins content of array into string.
join(",") - joins an array but splits each element with comma.
split(",") - creates an array splitting each element at the comma.
reverse - print array in reverse.
sort - simple sort.
uniq - new array with unique values.

Add exclamation mark with methods to edit in line.

delete_at(n) - delete at position n
delete(value) - deletes "value" from array and returns it.
push(arg) - add "arg" to end of array.
pop - returns and removes the last element of the array.
shift and unshift - same as push and pop but for first element.
You can add arrays together with '+'.

You can search for extra methods in docs.
