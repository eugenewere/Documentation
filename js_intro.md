# JavaScript

### JavaScript Can Change HTML Content.

One of many JavaScript HTML methods is.

```javascript
getElementById()
```

```javascript
document.getElementById("demo").innerHTML = "Hello JavaScript";
```

### JavaScript Can Change HTML Styles (CSS)


```javascript
document.getElementById("demo").style.display = "none";
```

### JavaScript Can Show HTML Elements
```javascript
document.getElementById("demo").style.display = "block";
```


### The "script" Tag

```html
<script>
    document.getElementById("demo").innerHTML = "My First JavaScript";
</script>
```

```html
<!DOCTYPE html>
<html>
    <head>
        <script>
            function myFunction() {
            document.getElementById("demo").innerHTML = "Paragraph changed.";
            }
        </script>
    </head>
    <body>
        <h2>Demo JavaScript in Head</h2>

        <p id="demo">A Paragraph</p>
        <button type="button" onclick="myFunction()">Try it</button>
        <script>
            function myFunction() {
            document.getElementById("demo").innerHTML = "Paragraph changed.";
            }
        </script>
    </body>
    
</html>
```


### External JavaScript

Scripts can also be placed in external files:

```html
<script src="myScript.js"></script>
```

### External References

An external script can be referenced in 3 different ways:

- With a full URL (a full web address)
- With a file path (like /js/)
- Without any path

This example uses a full URL to link to myScript.js:

```html
<script src="https://www.w3schools.com/js/myScript.js"></script>
<script src="/js/myScript.js"></script>
<script src="myScript.js"></script>
```

### Using console.log()

For debugging purposes, you can call the **console.log()** method in the browser to display data.

```html
<!DOCTYPE html>
<html>
    <body>

        <script>
        console.log(5 + 6);
        </script>

    </body>
</html>
```


### Using innerHTML

To access an HTML element, JavaScript can use the document.**getElementById(id)** method.

The id attribute defines the HTML element. The innerHTML property defines the HTML content:


```html
<body>

    <h1>My First Web Page</h1>
    <p>My First Paragraph</p>

    <p id="demo"></p>

    <script>
    document.getElementById("demo").innerHTML = 5 + 6;
    </script>

</body>
```

### Using document.write()

For testing purposes, it is convenient to use document.write():

```html
<!DOCTYPE html>
<html>
    <body>
        <h1>My First Web Page</h1>
        <p>My first paragraph.</p>

        <script>
            document.write(5 + 6);
        </script>
    </body>
</html>
```

### Semicolons ;
Semicolons separate JavaScript statements.

Add a semicolon at the end of each executable statement:

```javascript
let a, b, c;  // Declare 3 variables
a = 5;        // Assign the value 5 to a
b = 6;        // Assign the value 6 to b
c = a + b;    // Assign the sum of a and b to c
```

### JavaScript Keywords

JavaScript statements often start with a keyword to identify the JavaScript action to be performed.


| Keyword | Description                                                    |
| ------- |----------------------------------------------------------------|
| var | Declares a variable                                            |
| let | Declares a block variable                                      |
| const | Declares a block constant                                      |
| if | Marks a block of statements to be executed on a condition      |
| switch | Marks a block of statements to be executed in different cases  |
| for | Marks a block of statements to be executed in a loop           |
| function | Declares a function                                            |
| return | Exits a function                                               |
| try | Implements error handling to a block of statements             |


### Variables

Variables are Containers for Storing Data

JavaScript Variables can be declared in 4 ways:

- Automatically  

    ```x = 5;```
- Using var  

    ```var x = 5;```
- Using let 

    ```let x = 5;```
- Using const  

    ```const x = 5;```


When to Use var, let, or const?

1. Always declare variables

2. Always use const if the value should not be changed

3. Always use const if the type should not be changed (Arrays and Objects)

4. Only use let if you can't use const

5. Only use var if you MUST support old browsers.


### Declaring a JavaScript Variable
Creating a variable in JavaScript is called "declaring" a variable.

You declare a JavaScript variable with the var or the let keyword
```javascript
    var carName;
    let carName;
```

To assign a value to the variable, use the equal sign:

```javascript

carName = "Volvo";

```

### One Statement, Many Variables

```javascript
let person = "John Doe", carName = "Volvo", price = 200;
```

## Assignment

### The = Operator

The Simple Assignment Operator assigns a value to a variable.

```javascript
let x = 10 + y;

let x = 10;
```

### The += Operator

The Addition Assignment Operator adds a value to a variable.

```javascript
let x = 10;

x += 5;
```

### The -= Operator

The Subtraction Assignment Operator subtracts a value from a variable.

```javascript
let x = 10;

x -= 5;
```
### The *= Operator
The Multiplication Assignment Operator multiplies a variable.

### The **= Operator
The Exponentiation Assignment Operator raises a variable to the power of the operand.

```javascript
let x = 10;

x **= 5; // 100000
```

### The /= Operator
The Division Assignment Operator divides a variable.

### The %= Operator
The Remainder Assignment Operator assigns a remainder to a variable.

## Data Types

JavaScript has 8 Datatypes
1. String
2. Number
3. Bigint
4. Boolean
5. Undefined
6. Null
7. Symbol
8. Object

The Object Datatype. 
The object data type can contain:

1. An object
2. An array
3. A date

```javascript

// Numbers:
let length = 16;
let weight = 7.5;

// Strings:
let color = "Yellow";
let lastName = "Johnson";

// Booleans
let x = true;
let y = false;

// Object:
const person = {firstName:"John", lastName:"Doe"};

// Array object:
const cars = ["Saab", "Volvo", "BMW"];

// Date object:
const date = new Date("2022-03-25");
```


### The Concept of Data Types
In programming, data types is an important concept.

To be able to operate on variables, it is important to know something about the type.

Without data types, a computer cannot safely solve this:

```javascript
let x = 16 + "Volvo";
```

Does it make any sense to add "Volvo" to sixteen? Will it produce an error or will it produce a result?

JavaScript will treat the example above as:

```javascript
let x = "16" + "Volvo";
```

### JavaScript Types are Dynamic

JavaScript has dynamic types. This means that the same variable can be used to hold different data types:

```javascript
let x;       // Now x is undefined
x = 5;       // Now x is a Number
x = "John";  // Now x is a String
x = true;  // Now x is a Boolean
x  = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};  // Now x is a Object
x  =  ["Saab", "Volvo", "BMW"];  // Now x is a Array
```

## The typeof Operator

You can use the JavaScript typeof operator to find the type of a JavaScript variable.

The typeof operator returns the type of a variable or an expression:

```javascript
typeof ""             // Returns "string"
typeof "John"         // Returns "string"
typeof "John Doe"     // Returns "string"
typeof 0              // Returns "number"
typeof 314            // Returns "number"
typeof 3.14           // Returns "number"
typeof (3)            // Returns "number"
typeof (3 + 4)        // Returns "number"
```


### Undefined

In JavaScript, a variable without a value, has the value undefined. The type is also undefined.

```javascript
let car;    // Value is undefined, type is undefined
car = undefined;    // Value is undefined, type is undefined
```

## Functions

// Function to compute the product of p1 and p2
```javascript
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```
example 
```javascript
function myFunction(p1, p2) {
  return p1 * p2;
}
```
### Return

When JavaScript reaches a return statement, the function will stop executing.

```javascript
// Function is called, the return value will end up in x
let x = myFunction(4, 3);

function myFunction(a, b) {
// Function returns the product of a and b
  return a * b;
}
```

### Local Variables

Variables declared within a JavaScript function, become LOCAL to the function.

Local variables can only be accessed from within the function.

```javascript
function myFunction() {
  let carName = "Volvo";
  // code here CAN use carName
}
```

## Events

HTML events are "things" that happen to HTML elements.

When JavaScript is used in HTML pages, JavaScript can "react" on these events.

```javascript
<button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
```

```javascript
<button onclick="this.innerHTML = Date()">The time is?</button>
```

```javascript
<button onclick="displayDate()">The time is?</button>
```

## Strings

JavaScript strings are for storing and manipulating text.

### String Length

```javascript
let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
let length = text.length;
```

### String slice()
slice() extracts a part of a string and returns the extracted part in a new string.

The method takes 2 parameters: start position, and end position (end not included).

```javascript
let text = "Apple, Banana, Kiwi";
let part = text.slice(7, 13); //Banana
let part2 = text.slice(7); // Banana, Kiwi
let part3 = text.slice(-12); //Banana, Kiwi
let part4 = text.slice(-12, -6); // Banana
```

### Replacing String Content

The replace() method replaces a specified value with another value in a string:

```javascript
let text = "Please visit Microsoft!";
let newText = text.replace("Microsoft", "W3Schools");
```

By default, the replace() method is case sensitive. Writing MICROSOFT (with upper-case) will not work:

```javascript
let text = "Please visit Microsoft!";
let newText = text.replace("MICROSOFT", "W3Schools");
```

By default, the replace() method replaces only the first match:

```javascript
let text = "Please visit Microsoft and Microsoft!";
let newText = text.replace("Microsoft", "W3Schools");
```

### ReplaceAll

The replaceAll() method allows you to specify a regular expression instead of a string to be replaced.
```javascript
text = text.replaceAll("Cats","Dogs");
text = text.replaceAll("cats","dogs");
```

### toUpperCase and toLowerCase

```javascript
let text1 = "Hello World!";
let text2 = text1.toUpperCase();
let text3 = text1.toLowerCase();
```

### concat

```javascript
let text1 = "Hello";
let text2 = "World";
let text3 = text1.concat(" ", text2);
```

### trim

The trim() method removes whitespace from both sides of a string:

```javascript
let text1 = "      Hello World!      ";
let text2 = text1.trim();
```

### trimStart

The trimStart() method works like trim(), but removes whitespace only from the start of a string.


### trimEnd

The trimEnd() method works like trim(), but removes whitespace only from the end of a string.

### padStart

The padStart() method pads a string from the start.

It pads a string with another string (multiple times) until it reaches a given length.

```javascript
let text = "5";
let padded = text.padStart(4,"0");
let padded = text.padStart(4,"x");
```
### padEnd

The padEnd() method pads a string from the end.

It pads a string with another string (multiple times) until it reaches a given length.


```javascript

let text = "5";
let padded = text.padEnd(4,"0");

let text = "5";
let padded = text.padEnd(4,"x");
```

### charAt

The charAt() method returns the character at a specified index (position) in a string:

``` javascript
let text = "HELLO WORLD";
let char = text.charAt(0);
```

### charCodeAt

The charCodeAt() method returns the unicode of the character at a specified index in a string:

The method returns a UTF-16 code (an integer between 0 and 65535).

```javascript
let text = "HELLO WORLD";
let char = text.charCodeAt(0); // 72
```

### split

A string can be converted to an array with the split() method:

```javascript
text.split(",")    // Split on commas
text.split(" ")    // Split on spaces
text.split("|")    // Split on pipe
```

## String Search

### indexOf

The indexOf() method returns the index (position) the first occurrence of a string in a string:

```javascript
let text = "Please locate where 'locate' occurs!";
let index = text.indexOf("locate");
```

### lastIndexOf

The lastIndexOf() method returns the index of the last occurrence of a specified text in a string:

```javascript
let text = "Please locate where 'locate' occurs!";
let index = text.lastIndexOf("locate");
```

Both indexOf(), and lastIndexOf() return -1 if the text is not found:

### search

The search() method searches a string for a string (or a regular expression) and returns the position of the match:

```javascript
let text = "Please locate where 'locate' occurs!";
text.search("locate");
```

### includes

The includes() method returns true if a string contains a specified value.

Otherwise it returns false.

```javascript
let text = "Hello world, welcome to the universe.";
text.includes("world");
```

### startsWith

The startsWith() method returns true if a string begins with a specified value.

Otherwise it returns false:

```javascript
let text = "Hello world, welcome to the universe.";
text.startsWith("Hello");
```

### endsWith

The endsWith() method returns true if a string ends with a specified value.

Otherwise it returns false:

```javascript
let text = "John Doe";
text.endsWith("Doe");
```

## Template Literals

Template Literals use back-ticks (``) rather than the quotes ("") to define a string:


### Variable Substitutions

Template literals allow variables in strings:

```javascript
let firstName = "John";
let lastName = "Doe";

let text = `Welcome ${firstName}, ${lastName}!`;
```

## Number Methods

| Method          | Description                                          |
|-----------------|------------------------------------------------------|
| toString()      | 	Returns a number as a string                        |
 | toExponential() | 	Returns a number written in exponential notation    |
 | toFixed()       | 	Returns a number written with a number of decimals  |
 | toPrecision()   | 	Returns a number written with a specified length    |
 | ValueOf()       | 	Returns a number as a number                        |

### toString 

```javascript
let x = 123;
x.toString();
(123).toString();
(100 + 23).toString();
```

### toExponential
```javascript
let x = 9.656;
x.toExponential(2);
x.toExponential(4);
x.toExponential(6)
```

### toFixed

```javascript
let x = 9.656;
x.toFixed(0);
x.toFixed(2);
x.toFixed(4);
x.toFixed(6);
```

### toPrecision
```javascript
let x = 9.656;
x.toPrecision();
x.toPrecision(2);
x.toPrecision(4);
x.toPrecision(6)
```

### valueOf
```javascript

let x = 123;
x.valueOf();
(123).valueOf();
(100 + 23).valueOf();
```


### Number

The Number() method can be used to convert JavaScript variables to numbers:

```javascript
Number(true); // 1
Number(false); // 0
Number("10"); // 10
Number("  10"); // 10
Number("10  "); // 10
Number(" 10  "); // 10
Number("10.33"); // 10.33
Number("10,33"); // NaN
Number("10 33"); // NaN
Number("John"); // NaN

```

### parseInt

parseInt() parses a string and returns a whole number. Spaces are allowed. Only the first number is returned:
```javascript
parseInt("-10"); // -10
parseInt("-10.33"); // -10
parseInt("10"); // 10
parseInt("10.33"); // 10
parseInt("10 20 30"); // 10
parseInt("10 years"); // 10
parseInt("years 10"); // NaN

```

parseFloat

parseFloat() parses a string and returns a number. Spaces are allowed. Only the first number is returned:

```javascript

parseFloat("10"); // 10
parseFloat("10.33"); // 10.33
parseFloat("10 20 30"); // 10
parseFloat("10 years"); // 10
parseFloat("years 10") // NaN
```

## Arrays

An array is a special variable, which can hold more than one value:

```javascript
const cars = ["Saab", "Volvo", "BMW"];
```

You can also create an array, and then provide the elements:

```javascript
const cars = [];
cars[0]= "Saab";
cars[1]= "Volvo";
cars[2]= "BMW";
```