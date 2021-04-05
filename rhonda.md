# Python Basics and Functions

## Types of Data
- Numbers
  - ints `1,5,-1`
  - floats `1.5, -1.2`
- Strings
  - `"hello"`
  - `'goodbye'`
- Booleans
  - `True`
  - `False`
- Lists
  - `[1,2,3]`
- Tuples 
  - `(1,2,3)`
- Dictionaries/HashMaps
- `{"key": value}`  
- `{"test": 1}`

## Boolean Operators
These are used for conditional statements -> they evaluate to a boolean value

- `==` -> Evaluate if equal
  - `'a' == 'a'` -> `True`
  - `'7' == 7
    ` -> `False`
  - `x == x` -> `True`
  - `x == y` -> `False`

- `>` -> Evaluate if greater than
  - `7 > 6` -> `True`
  - `7 > 8` -> `False`
  
- `>=` -> Evaluate if greater than or equal to
  - `7 >= 7` -> `True`
  - `7 >= 8` -> `False`

- `<` -> Evaluate if less than
  - `7 < 8` -> `True`
  - `7 < 6` -> `False`
  
- `<=` -> Evaluate if less than or equal to
  - `7 <= 7` -> `True`
  - `7 <= 6` -> `False`

- `and` -> Evaluate if both expressions/values are true
  - `True and True` -> `True`
  - `True and False` -> `False`
  - `False and True` -> `False`
  - `False and False` -> `False`
  
- `or` -> Evaluate if one of the expressions/values is true
  - `True or True` -> `True`
  - `True or False` -> `True`
  - `False or True` -> `True`
  - `False or False` -> `False`
  
- `not` -> Only takes one operand and evaluates the opposite
  - `not True` -> `False`
  - `not False` -> `True`
  - `not (not True)` -> `True`
  - `not (not False)` -> `False`
  
These expressions can be combined in various ways for more complex truth tables

## Lists 
- Collection of data that can be indexed using 0-based indexing
```
x = [1,2,3]
x[0] -> 1
x[2] -> 3
x[3] -> Error because only 3 elements
```
- allows for slicing -> slice(start, stop, stride)
  - start is the index to start the slice - is **inclusive** and `default = 0`
  - stop is the index to end the slice and is **exclusive** and `default = length of list`
  - stride is how many elements to "step" and `defaults to 1` 
```
x = [1,2,3,4,5,6]
y = x[1:5]
y -> [2,3,4,5]
z = x[::-1]
z -> [6,5,4,3,2,1]
y = x[0:4:2]
y -> [1,3]
```
- Can be concatenated using the `+`
```
x = [1,2,3]
y = [4,5,6]
z = x + y
z -> [1,2,3,4,5,6]
```

### Functions
- `append(x)` - add element `x` to the end of the list
```
x = [1,2,3]
x.append(4)
x -> [1,2,3,4]
```
- `count(x)` - returns the count of the element in the list
```
x = ['Apple', 'Cherry', 'Cherry', 'Melon']
y = x.count('Cherry')
y -> 2
```

## Strings
- Start and end with `"` or `'`
- Function similar to lists (can be sliced, indexed, etc.)
```
x = 'Hello'
y = " World"
z = x + y
z -> 'Hello World'
test = x[1:3]
test -> 'el'
```

## Functions
- `upper()` - turns the string into all uppercase
- `lower()` - turns the string into all lowercase
```
x = 'HelLo'
y = x.upper()
z = x.lower()
y -> 'HELLO'
z -> 'hello'
```

### Dictionaries
- Map of keys and values 
- Indexed by key and returns value
- Keys are separated by values with the `:`
```
x = {"test": 1}
y = x['test']
y -> 1
x['newKey'] = 2
x -> {"test": 1, "newKey": 2}
```

### Misc Functions
- `len(list)` -> returns the `length` of the list/string/iterable
```
x = [1,2,3,4]
y = len(x)
y -> 4
x = []
y = len(x)
y -> 0
z = 'Hello'
v = len(z)
v -> 5
```