# `Python Data`
___

Covered in this File
1. Data Types
2. Data Literals

<br>

# `Data Types`
___
To work with data it must by classified into types, we will begin with literal data
> * **Literal Data**: actual values that do not represent anything else


## Beginner Data Types
*Beginners should begin with the data types below as they compose the vast majority of data you will work with.*


```python
True          # boolean (True or False)
5             # integer (whole number)
3.14          # float (decimal number)
"a"           # character (single symbol) in quotes use "" or ''
"Hello World" # String (text) in quotes use "" or '' 

["a","b","c"] # list (contains multiple items called elements)
# 0   1   2   # indexes (are used to access each element)

#There are more data types but these are the main types for beginners.
```

<br>

## All Data Types

> * Data types can be classified into two groups: Mutable Data, and Immutable Data  

* **Mutable Data:** the data can be changed
    * ie. Lists, Sets, Dictionaries
* **Immutable Data:** the data cannot be changed
    * ie. number types, booleans, strings, tuples
    
<br>

### Determining Type of Data: builtin ***type( )*** function call
syntax:
```
type(data)
```

***type( )*** returns the type of the data that was passed as an argument


```python
#The type() function returns the type of data passed to it.
type()
# type() requires an argument in order to determine the type.

type(None)                   # Returns: <class 'NoneType'>
type(True)                   # Returns: <class 'bool'>
type(5)                      # Returns: <class 'int'>
type(3.14)                   # Returns: <class 'float'>
type(1j)                     # Returns: <class 'complex'>
type("a")                    # Returns: <class 'str'>
type("Hello")                # Returns: <class 'str'>
type(["a","b","c"])          # Returns: <class 'list'>
type(("a","b","c"))          # Returns: <class 'tuple'>
type({"a","b","c"})          # Returns: <class 'set'>
type({"a":97,"b":98,"c":99}) # Returns: <class 'dict'>
```

For large numbers you can use underscores( _ ) to make them more readable


```python
1_000_000_000 #Returns: 1000000000 --> Notice it doesn't return with the underscores
```

Scientific notation is also available, use E to represent (x 10^)


```python
1E9 # Returns: 1000000000.0 --> Notice it returns a float
```

More advanced data types


```python
1j               # Complex Numbers (j replaces i as the imaginary unit--> sqrt(-1) imaginary numbers)
("a","b","c")    # Tuples a collection which is ordered, immutable and allows duplicate members.
{"a","b","c"}    # Sets a collection which is unordered, unchangeable*,unindexed, and allows NO duplicate members.
{"a":97,"b":98 } # Dictionaries are a collection of key:value pairs; they are ordered**, mutable, and allows NO duplicate members.

#Additional data types are defined by classes, here are a few examples:
range(5)            # Ranges represent a sequence of numbers 
bytearray(b'hello') # Byte Arrays are mutable sequences of bytes
None                # Null type meaning nothing
```

<br>

# `Data Literals`
___
> * Literal: refers to a notation for representing a fixed actual value
> * Literals do not represent something else

<br>

### **Null Literals <class 'NoneType'>**
> * Null means nothing or having no value


```python
None #Null type in python
```

<br>

### **Boolean Literals <class 'bool'>**
> * Booleans have two states, usually represented as True or False


```python
True              # boolean literal
False             # boolean literal
```

<br>

### **Integer Literals <class 'int'>**
> * Integers are whole numbers, meaning they have no fractional parts


```python
0                 # integer literal
1                 # integer literal
-1                # integer literal
10                # integer literal
100               # integer literal
50239             # integer literal
12                # integer literal
-11               # integer literal
```

<br>

### **Float Literals <class 'float'>**
> * Floats or floating point numbers are fractional numbers named after the point (.) used to destinguish the whole from the fractional part of the number.


```python
1.12            #float literal
2.71            #float literal
3.141592653589  #float literal
6.023           #float literal
-10.1           #float literal
-78.91          #float literal
```

<br>

### **Complex Literals <class 'complex'>**
* Complex numbers have a real and an imaginary part (i or sqrt(-1))
* In python i is replaced with j for complex numbers


```python
3 + 2j      # complex literal 
-1 + 5j     # complex literal 
0 + 7j      # complex literal 
4 - 3j      # complex literal 
-2 - 6j     # complex literal 
1 + 0j      # This is a real number but represented as a complex number
2 - 4j      # complex literal 
-3 + 8j     # complex literal 
6 - 2j      # complex literal 
2 + 2j      # complex literal       
```

<br>

### **Character Literals <class 'str'>**
* Characters are single units of text, such as a letter, digit, punctuation mark, symbol, or whitespace
* Characters in python are single length strings


```python
'A'   # Uppercase letter character literal
'b'   # Lowercase letter character literal
'5'   # Digit character literal
'@'   # At character literal
'%'   # Percent character literal
' '   # Whitespace character literal
'\n'  # Newline character literal
'\t'  # Tab character literal
'['   # Left Square Bracket character literal
']'   # Right Square Bracket character literal
```

<br>

### **String Literals <class 'str'>**
* Strings are a collection of characters


```python
"Python"                                         # String Literal
"Programming"                                    # String Literal
"Literals"                                       # String Literal
"Hello World!"                                   # String Literal
"13189238912"                                    # String Literal
"asdf1239043hf"                                  # String Literal
"The quick brown fox jumps over the lazy dog."   # String Literal
```

<br>

### **Collection Literals**

There are four collection data types in the Python programming language:

**List:**   
> collection which is ordered(indexed), mutable, allows duplicate members, and uses [ ] to enclose members.

**Tuple:**  
> collection which is ordered(indexed), immutable, allows duplicate members and uses ( ) to enclose members.

**Set:**   
> collection which is unordered(not indexed), mutable, does NOT allow duplicate members and uses { } to enclose members.

**Dictionary:**   
> collection which is ordered(indexed with a key), mutable, does NOT allow duplicate members and uses { : } to enclose members.

|**List**|**Tuple**|**Set**|**Dictionary**|
|:-:|:-:|:-:|:-:|
|ordered (numerically indexed)|ordered (numerically indexed)|unordered (not indexed)|ordered (indexed with a key)|
|mutable|immutable|mutable|mutable|
|duplicates|duplicates|NO duplicates|NO duplicates|
|**[ ]**|**( )**|**{ }**|**{ : }**| 

* *Data Structure: a specialized format for organizing, processing, retrieving, and storing data.*
* *Collection: a data structure that holds multiple elements*
* *Member: an item stored within a collection*
* *Element: is a synonym for member*
* *Ordered: having a specific order 0,1,2,... (ie. indexed)*
* *Indexed:  elements are associated with a specific identifier (index), which can be used to directly locate and access the data*
* *Mutable: elements can change*
* *Immutable: elements cannot change*

<br>

### **List Literals <class 'list'>**
> * Basically: A list is a collection of comma seperated elements
> * Specifically: A list is a collection of data that is ordered, mutable, and allows duplicate members.
> * Each item stored in a list is called an element

Lists are denoted with square brackets [ ]


List syntax:
```
[element, element, element, ...]
```

```python
["a","b","c"] # list (contains multiple items called elements)
# 0   1   2   # indexes (are used to access each element)
```


```python
[None, None, None]              # List Literal containing multiple Null Types
[True, False, True]             # List Literal containing multiple booleans
[42, 123, -7]                   # List Literal containing multiple integers
[3.14, 2.718, 0.5]              # List Literal containing multiple floats
[2 + 3j, 1 - 1j, 5j]            # List Literal containing multiple complex numbers
['a', 'b', 'c']                 # List Literal containing multiple characters 
['hello', 'world', 'python']    # List Literal containing multiple strings

[1, 3.14, 'grape', False, (2+3j), 'kiwi'] # List Literal containing multiple types
```

<br>

### **Tuple Literals <class 'tuple'>**

> * Basically: a list that cannot be changed
> * Specifically: collections which are ordered(indexed), immutable, allow duplicate members and uses ( ) to enclose members.
> * Each item stored in a tuple is called an element

Tuples are denoted with parenthesis ( )

Tuple syntax:
```
(element, element, element, ...)
```

```python
("a","b","c") # tuple (contains multiple items called elements)
# 0   1   2   # indexes (are used to access each element)
```


```python
(None, None, None)              # Tuple Literal containing multiple Nones
(True, False, True)             # Tuple Literal containing multiple booleans
(42, 123, -7)                   # Tuple Literal containing multiple integers
(3.14, 2.718, 0.5)              # Tuple Literal containing multiple floats
(2 + 3j, 1 - 1j, 5j)            # Tuple Literal containing multiple complex numbers
('a', 'b', 'c')                 # Tuple Literal containing multiple characters (represented as strings)
('hello', 'world', 'python')    # Tuple Literal containing multiple strings

(5, 6.7, 'orange', True, (7+8j)) # Tuple Literal containing multiple types
```

<br>

### **Set Literals <class 'set'>**

> * Basically: a list with no order, and no duplicates.
> * Specifically: collection which is unordered(not indexed), mutable, and does NOT allow duplicate members.

Sets are denoted with curly braces { }

Set syntax:
```
{element, element, element, ...}
```

```python
{None}                          # Set literal Containing a Null Type
{False, True}                   # Set literal Containing booleans
{42, 123, -7}                   # Set literal Containing integers
{0.5, 2.718, 3.14}              # Set literal Containing floats
{(1-1j), (2+3j), 5j}            # Set literal Containing complex numbers
{'b', 'a', 'c'}                 # Set literal Containing characters
{'python', 'hello', 'world'}    # Set literal Containing strings
```

<br>

### **Dictionary Literals <class 'dict'>**
> * Basically: a list with data pairs, one that is a key and one that is the value  
> * Specifically: collection which is ordered(indexed with a key), mutable, does NOT allow duplicate members and uses { : } to enclose members.
> * in other languages are called: map, hashmap, or associative arrays

Dictionaries are denoted using curly braces { : }  

Dictionary syntax:
```
{key:value, key:value, key:value, ...}
```

```python
{'apple': 5, 'banana': 3, 'orange': 7}                      # Dictionary Literal with String Keys, and Integer Values

{1: 'one', 2: 'two', 3: 'three'}                            # Dictionary Literal with Integer Keys, and String Values

{('a', 'b'): [1, 2, 3], ('x', 'y'): ['foo', 'bar']}         # Dictionary Literal with Tuple Keys, and List Values

{3.14: True, 2.718: False}                                  # Dictionary Literal with Float Keys, and Boolean Values

{True: {'a': 1, 'b': 2}, False: {'x': 10, 'y': 20}}         # Dictionary Literal with Boolean Keys, and Dictionary Values

{'name': 'John', 42: 'answer', (1, 2): ['tuple', 'values']} # Dictionary Mixed Type Key:Value pairs
```
