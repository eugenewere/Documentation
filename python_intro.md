# Python
Python is a popular programming language.

- web development (server-side),
- software development,
- mathematics,
- system scripting.

## Python Indentation

Indentation refers to the spaces at the beginning of a code line.

Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.

Python uses indentation to indicate a block of code.

```python
if 5 > 2:
  print("Five is greater than two!")
```
## Logging in python 

```javascript
print("This is Looging")
```


## Python Variables

In Python, variables are created when you assign a value to it:

```javascript
x = 5
y = "Hello, World!"
```

## Data Types

In programming, data type is an important concept.

Variables can store data of different types, and different types can do different things.

Python has the following data types built-in by default, in these categories:

| Text Type: |	str |
| ----------  | ---- |
| Numeric Types: |	int, float |
| Sequence Types: |	list, |
| Boolean Type: |	bool |
| None Type: |	NoneType |


## Casting

There may be times when you want to specify a type on to a variable. This can be done with casting. Python is an object-orientated language, and as such it uses classes to define data types, including its primitive types.

Casting in python is therefore done using constructor functions:

- **int()** - constructs an integer number from an integer literal, a float literal (by removing all decimals), or a string literal (providing the string represents a whole number)
- **float()** - constructs a float number from an integer literal, a float literal or a string literal (providing the string represents a float or an integer)
- **str()** - constructs a string from a wide variety of data types, including strings, integer literals and float literals


```javascript
x = int(1)   # x will be 1
y = int(2.8) # y will be 2
z = int("3") # z will be 3


x = float(1)     # x will be 1.0
y = float(2.8)   # y will be 2.8
z = float("3")   # z will be 3.0
w = float("4.2") # w will be 4.2


x = str("s1") # x will be 's1'
y = str(2)    # y will be '2'
z = str(3.0)  # z will be '3.0'
```

### type()
What is the data type of an element

```javascript
mylist = ["apple", "banana", "cherry"]
print(type(mylist)) // <class 'list'>
```


### Python Operators

Operators are used to perform operations on variables and values.

In the example below, we use the ``+`` operator to add together two values:

| Operator |	Name |	Example |
| -------  |  ------ |  ------ |
| + |	Addition |	x + y |
| - |	Subtraction |	x - y |
| * |	Multiplication |	x * y |
| / |	Division |	x / y |
| % |	Modulus |	x % y |

### Python Comparison Operators
Comparison operators are used to compare two values:


| Operator | 	Name                             | 	Example	 | 
|----------|-----------------------------------|-----------|
|  ==      | 	Equal | 	x == y   |
 |  !=      | 	Not equal | 	x != y   |
 |  >       | 	Greater than | 	x > y    |
 |  <       | 	Less than | 	x < y    |
 |  >=      | 	Greater than or equal to | 	x >= y   |
 |  <=      | 	Less than or equal to | 	x <= y   |


### Logical Operators
Logical operators are used to combine conditional statements:

| Operator| 	Description	|   Example| 
|----------|-----------------------------------|-----------|
| and |  	Returns True if both statements are true |	x < 5 and  x < 10 |
| or	|  Returns True if one of the statements is true |	x < 5 or x < 4 |
| not	|  Reverse the result, returns False if the result is true |	not(x < 5 and x < 10) |

###  Identity Operators

Identity operators are used to compare the objects, not if they are equal, but if they are actually the same object, with the same memory location:

|Operator|	Description|	Example|
|----------|-----------------------------------|-----------|
|is |	Returns True if both variables are the same object|	x is y|
|is not|	Returns True if both variables are not the same object|	x is not y|

### Membership Operators

Membership operators are used to test if a sequence is presented in an object:

 |Operator |	Description |	Example |
|----------|-----------------------------------|-----------|
 |in | 	Returns True if a sequence with the specified value is present in the object |	x in y |
 |not in |	Returns True if a sequence with the specified value is not present in the object |	x not in y |

### Operator Precedence

Operator precedence describes the order in which operations are performed.
Parentheses has the highest precedence, meaning that expressions inside parentheses must be evaluated first:

```javascript
print((6 + 3) - (6 + 3))
```

Multiplication * has higher precedence than addition +, and therefor multiplications are evaluated before additions:

```javascript
print(100 + 5 * 3)
```


## Python Lists

Lists are used to store multiple items in a single variable.

```javascript
thislist = ["apple", "banana", "cherry"]
print(thislist)
```

### List Length

To determine how many items a list has, use the len() function:

```javascript
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```

### Access Items
List items are indexed and you can access them by referring to the index number:

```javascript
thislist = ["apple", "banana", "cherry"]
print(thislist[1])
```

### Negative Indexing

Negative indexing means start from the end

``-1`` refers to the last item, ``-2`` refers to the second last item etc.

```javascript
thislist = ["apple", "banana", "cherry"]
print(thislist[-1])
```

### Range of Indexes

You can specify a range of indexes by specifying where to start and where to end the range.

When specifying a range, the return value will be a new list with the specified items.

```javascript
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])


thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[:4])

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:])

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[-4:-1])
```

### Check if Item Exists

To determine if a specified item is present in a list use the in keyword:

```javascript
thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")
```

### Change List Items

To change the value of a specific item, refer to the index number:


```javascript
thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"
print(thislist)
```

Change a Range of Item Values

```javascript
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]
thislist[1:3] = ["blackcurrant", "watermelon"]
print(thislist)
```

 Change the second and third value by replacing it with one value:
 
```javascript
thislist = ["apple", "banana", "cherry"]
thislist[1:3] = ["watermelon"]
print(thislist)
```

### Add List Items

To add an item to the end of the list, use the append() method:

#### Append Items

```javascript
thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)

```

#### Insert Items

To insert a list item at a specified index, use the insert() method.

The insert() method inserts an item at the specified index:

```javascript
thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)
```

### Extend List

To append elements from another list to the current list, use the extend() method.

```javascript
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)
```

### Remove List Items

The remove() method removes the specified item

```javascript
thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)
```

### Remove Specified Index

The pop() method removes the specified index.

```javascript
thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)
```

#### N/B
If you do not specify the index, the pop() method removes the last item.

### Using **Del**
The del keyword also removes the specified index:

```javascript
thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)
```

The del keyword can also delete the list completely.

```javascript
thislist = ["apple", "banana", "cherry"]
del thislist
```

### Loop Lists
You can loop through the list items by using a for loop:

```javascript
thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)
```


## Python If ... Else

Python supports the usual logical conditions from mathematics:

- Equals: a == b
- Not Equals: a != b
- Less than: a < b
- Less than or equal to: a <= b
- Greater than: a > b
- Greater than or equal to: a >= b
These conditions can be used in several ways, most commonly in "if statements" and loops.

An "if statement" is written by using the if keyword.

```javascript
a = 33
b = 200
if b > a:
  print("b is greater than a")
```


### Elif
The elif keyword is Python's way of saying "if the previous conditions were not true, then try this condition".
```javascript
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```

### Else
The else keyword catches anything which isn't caught by the preceding conditions.

```javascript
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```

### And
The and keyword is a logical operator, and is used to combine conditional statements:


```javascript
a = 200
b = 33
c = 500
if a > b and c > a:
  print("Both conditions are True")
```

### Or
The or keyword is a logical operator, and is used to combine conditional statements:

```javascript
a = 200
b = 33
c = 500
if a > b or a > c:
  print("At least one of the conditions is True")
```

### Not
The not keyword is a logical operator, and is used to reverse the result of the conditional statement:

```javascript
a = 33
b = 200
if not a > b:
  print("a is NOT greater than b")
```

### Nested If
You can have if statements inside if statements, this is called nested if statements.

```javascript

x = 41

if x > 10:
  print("Above ten,")
  if x > 20:
    print("and also above 20!")
  else:
    print("but not above 20.")
```

## For Loops

A for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).

This is less like the for keyword in other programming languages, and works more like an iterator method as found in other object-orientated programming languages.

With the for loop we can execute a set of statements, once for each item in a list, tuple, set etc.

```javascript
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)


for x in "banana":
   print(x)


for x in range(6):
   print(x)

for x in range(2, 6):
   print(x)

// Increment the sequence with 3 (default is 1):
for x in range(2, 30, 3):
    print(x)
```

### Nested Loops

A nested loop is a loop inside a loop.

The "inner loop" will be executed one time for each iteration of the "outer loop":

```javascript
adj = ["red", "big", "tasty"]
fruits = ["apple", "banana", "cherry"]

for x in adj:
  for y in fruits:
    print(x, y)
```

## Functions

A function is a block of code which only runs when it is called.

You can pass data, known as parameters, into a function.

A function can return data as a result.


```javascript
def my_function():
  print("Hello from a function")
```

### Calling a Function

To call a function, use the function name followed by parenthesis

```javascript
def my_function():
  print("Hello from a function")

my_function()
```

### Arguments

```javascript
def my_function(fname):
  print(fname + " Refsnes")

my_function("Emil")
my_function("Tobias")
my_function("Linus")
```

### Arbitrary Arguments, *args

If you do not know how many arguments that will be passed into your function, add a * before the parameter name in the function definition.

This way the function will receive a tuple of arguments, and can access the items accordingly:

```javascript
def my_function(*kids):
  print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus")

```


### Keyword Arguments **kwargs
You can also send arguments with the key = value syntax.

This way the order of the arguments does not matter.


```javascript
def my_function(child3, child2, child1):
  print("The youngest child is " + child3)

my_function(child1 = "Emil", child2 = "Tobias", child3 = "Linus")
```

### Default Parameter Value
The following example shows how to use a default parameter value.

If we call the function without argument, it uses the default value:


```javascript
def my_function(country = "Norway"):
  print("I am from " + country)

my_function("Sweden")
my_function("India")
my_function()
my_function("Brazil")
```

### Return Values
To let a function return a value, use the return statement
```javascript
def my_function(x):
  return 5 * x

print(my_function(3))
print(my_function(5))
print(my_function(9))
```


# Classes/Objects

Python is an object oriented programming language.

Almost everything in Python is an object, with its properties and methods.

A Class is like an object constructor, or a "blueprint" for creating objects.

```javascript
class MyClass:
  x = 5

p1 = MyClass()
print(p1.x)
```

### The __init__() Function

The examples above are classes and objects in their simplest form, and are not really useful in real life applications.

To understand the meaning of classes we have to understand the built-in __init__() function.

All classes have a function called __init__(), which is always executed when the class is being initiated.

Use the __init__() function to assign values to object properties, or other operations that are necessary to do when the object is being created:


```javascript
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)
```

### Object Methods

Objects can also contain methods. Methods in objects are functions that belong to the object.

Let us create a method in the Person class:

```javascript
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    print("Hello my name is " + self.name)

p1 = Person("John", 36)
p1.myfunc()
```


### The self Parameter

The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.

It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class:

```javascript
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    print("Hello my name is " + self.name)

p1 = Person("John", 36)
p1.myfunc()
```

## Modules

Consider a module to be the same as a code library.

A file containing a set of functions you want to include in your application.

```javascript
import mymodule

mymodule.greeting("Jonathan")
```

### Import From Module

You can choose to import only parts from a module, by using the from keyword.


```javascript
from anmimal import person

print (person["age"])
```


### PIP

PIP is a package manager for Python packages, or modules if you like.

```shell
pip install camelcase
```

#### Using a Package

```javascript
import camelcase

c = camelcase.CamelCase()

txt = "hello world"

print(c.hump(txt))
```


#### Remove a Package


Use the uninstall command to remove a package:


```shell
pip uninstall camelcase
```

#### List Packages
Use the list command to list all the packages installed on your system:


```shell
pip list
```

## Datetime

A date in Python is not a data type of its own, but we can import a module named datetime to work with dates as date objects.

```javascript
import datetime

x = datetime.datetime.now()
print(x)
print(x.year)
print(x.strftime("%A"))
```

### Creating Date Objects

To create a date, we can use the datetime() class (constructor) of the datetime module.

The datetime() class requires three parameters to create a date: year, month, day.

```javascript
import datetime

x = datetime.datetime(2020, 5, 17)

print(x)
```

### strftime() Method

The datetime object has a method for formatting date objects into readable strings.

The method is called strftime(), and takes one parameter, format, to specify the format of the returned string:

```javascript
import datetime

x = datetime.datetime(2018, 6, 1)

print(x.strftime("%B"))
```


formats

| Directive |	Description |	Example	 |
|-----------| ------------- | ---------- |
| %a        |	Weekday, short version |	Wed |
 | %A        |	Weekday, full version |	Wednesday |
 | %w        |	Weekday as a number 0-6, 0 is Sunday |	3 |
 | %d        |	Day of month 01-31 |	31 |
 | %b        |	Month name, short version |	Dec |
 | %B        |	Month name, full version |	December |
 | %m        |	Month as a number 01-12 |	12 |
 | %y        |	Year, short version, without century |	18 |
 | %Y        |	Year, full version |	2018 |
 | %H        |	Hour 00-23 |	17 |
 | %I        |	Hour 00-12 |	05 |
 | %p        |	AM/PM	 |PM |
 | %M        |	Minute 00-59 |	41 |
 | %S        |	Second 00-59 |	08 |
 | %f        |	Microsecond 000000-999999 |	548513 |
 | %z        |	UTC offset |	+0100 |
 | %Z        |	Timezone |	CST |
 | %j        |	Day number of year 001-366 |	365 |
 | %U        |	Week number of year, Sunday as the first day of week, 00-53 |	52 |
 | %W        |	Week number of year, Monday as the first day of week, 00-53 |	52 |
 | %c        |	Local version of date and time	Mon Dec 31 17:41:00 | 2018 |
 | %C        |	Century |	20 |
 | %x        |	Local version of date |	12/31/18 |
 | %X        |	Local version of time |	17:41:00 |
 | %%        |	A % character |	% |
 | %G        |	ISO 8601 year |	2018 |
 | %u        |	ISO 8601 weekday (1-7) |	1 |
 | %V        |	ISO 8601 weeknumber (01-53) |	01 |


## JSON

JSON is a syntax for storing and exchanging data.

JSON is text, written with JavaScript object notation.

### JSON in Python

Python has a built-in package called json, which can be used to work with JSON data.

```javascript
import json
```

## Reading JSON

```javascript
import json

x =  { "name":"John", "age":30, "city":"New York"}


print(y["age"])
```


# Python Try Except

The ```try``` block lets you test a block of code for errors.

The ```except``` block lets you handle the error.

The ```else``` block lets you execute code when there is no error.

The ```finally``` block lets you execute code, regardless of the result of the try- and except blocks.

## Exception Handling

When an error occurs, or exception as we call it, Python will normally stop and generate an error message.

These exceptions can be handled using the try statement:

```javascript
try:
  print(x)
except:
  print("An exception occurred")
```

## Many Exceptions

You can define as many exception blocks as you want, e.g. if you want to execute a special block of code for a special kind of error:

```javascript
try:
  print(x)
except NameError:
  print("Variable x is not defined")
except:
  print("Something else went wrong")
```

### Else
You can use the else keyword to define a block of code to be executed if no errors were raised:

```javascript
try:
  print("Hello")
except:
  print("Something went wrong")
else:
  print("Nothing went wrong")
```

### Finally
The finally block, if specified, will be executed regardless if the try block raises an error or not.

```javascript
try:
  print(x)
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
```


### Raise an exception

As a Python developer you can choose to throw an exception if a condition occurs.

To throw (or raise) an exception, use the raise keyword.

```javascript
x = -1

if x < 0:
  raise Exception("Sorry, no numbers below zero")


y = "hello"

if not type(y) is int:
    raise TypeError("Only integers are allowed")
```





## String Formatting

To make sure a string will display as expected, we can format the result with the format() method.

### String format()

The format() method allows you to format selected parts of a string.

Sometimes there are parts of a text that you do not control, maybe they come from a database, or user input?

To control such values, add placeholders (curly brackets {}) in the text, and run the values through the format() method:


```javascript
price = 49
txt = "The price is {} dollars"
print(txt.format(price))

// or

quantity = 3
itemno = 567
price = 49
myorder = "I want {0} pieces of item number {1} for {2:.2f} dollars."
print(myorder.format(quantity, itemno, price))



```
or using ``f`` string

```javascript
quantity = 3
itemno = 567
price = 49
myorder = f"I want {quantity} pieces of item number {itemno} for {price} dollars."
print(myorder)
```


















