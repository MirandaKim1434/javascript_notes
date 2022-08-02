# JavaScript Notes

#### JavaScript program is a list of programing statements that are to be executed by a computer that are composed of values, operators, expressions, keywords, and // comments, these are executed one by one or same order as they are written. When writing a line of codes it is best to avoid lines longer then 80 characters, if it doesnt fit on one line break it after an operator. Keep in mind JavaScript is case sensitive

## JavaScript HTML methods

#### `getElementById()` this is inserted between a script tag and you may write as many scripts as you would like in HTML. It can be placed in the body or head tag or both as well. JavaScript can be place in external files.

### Finds an HTML element example:

```js
document.getElementById("demo").innerHTML = "Hello JavaScript";
```

### Change HTML styles example:

```js
document.getElementById("demo").style.fontSize = "16px";
```

### Hide HTML elements example:

```js
document.getElementById("demo").style.display = "none";
```

### Show HTML elements example:

```js
document.getElementById("demo").style.display = "block";
```

### Example insdie a script tag:

```js
  document.getElementById("demo").innerHTML = "My First JavaScript";
```

## Semicolons ;

#### Not required but highly recommended because it separtes JavaScript statements at the end of each executable statement and also allow multiple statements.

## JavaScript White Space:

#### Ignores multiple spaces and can be added to make your text more readable

## JavaScript Code Blocks:

#### Can be grouped in code blocks {} to make execution together

## JavaScript Syntax:

#### Fixed values are literals which are numbers that written with or without decimals and extra large or extra small numbers can be written with scientific exponent notation or strings of text written within double or single quotes `” ”` or `‘ ’`.

#### Variable values are variables that store data values, for instance; var, let and const to declare variables. The = is to assign values to variables these are \* allowed in any program.

## JavaScript Operators:

#### Are arithmetic operators (`+ = * /`) to compute values (called operands). Two number can be literals, variables or expressions

## JavaScript Keywords:

#### The `let` will tells the browser to create variables and `var` will tell the browser to create variables, both produce same result. Which hold different data types numbers, strings, objects and more.

## JavaScript Comments:

#### Comments are ignored and not executed.

### Example of comments:

`// comments`

`/*`

`*/`

## JavaScript Functions and Events

#### Block of JavaScript code that can be executed, event is pushing a button, can be placed in the `<head>` to push a button in the `<body>`. You can place as many as you would like but external scripts cannot contain `<script>`

## External JavaScript

#### Practical when same code for many different web pages. It separates HTML and code which makes it easier to read and manage. Can also speed up page loads. These can be referenced in 3 different ways: full URL, file path, or no path to line to notes.js

### Example:

```js
function myFunction() {
  document.getElementById("demo").innerHTML = "Paragraph changed.";
}
```

'''js
<script src="notes.js"></script>
'''

## innerHTML

#### This defines the HTML element and property defines the HTML content. Cahanging the innerHTML property of an HTML element is a comman way to display data in your HTML

### Example:

`document.getElementById(id) method.`

### Document. write()

#### Is for testing purposes after an HTML document is loaded it will delete all existing HTML.

### Window.alert()

#### Display data in a pop window. Another way to write it is inside a script tag

`alert(5+6)`

### console.log()

#### Used for debugging and away for the browser to display data

### JavaScript Print

#### There are no print objects or print methods and cannot access output devices from JavaScript, exceptions `window.print()` in the browser to bring the content of the current window

### JavaScript const

#### Always declare variables with const unless the value of the variable changes and must be assigned a value when declared. This is used for new array, object, function or RegExp. It also does not define a constant value defines constant reference. And changes elements of constant array and properties of constant object.

### example:

```js
const price1 = 5;
const price2 = 6;
let total = price1 + price2;
```

## JavaScript String Operators

#### `+` and `+=` can be used to add concatenate strings. Strings can have ‘ ‘ or “ “ as long as they do not match the quotes surrounding the string.

## JavaScript Booleans

#### Have two values true or false and conditional testing

## JavaScript Arrays

#### Written with `[]` and separated by `,`. It is also zero based 1st item is 0 next item is 1

### Example:

`const states = [“Florida, “California”, “Illinois”]`

## JavaScript Objects

#### Ojects are written with `{}` and written as name:value pairs, separated by commas.

### Example has 4 properties:

`const person = {firstName:”Miranda”, lastName:”Olson”, age:35, eyeColor:"brown”};`

## Accessing Object Properties

#### objects are containers for named values called properties

### example:

`objectName. propertyName` or `objectName[‘propertyName’]`

#### Objects can also have methods which are actions that can be preformed on objects and stored in properties as function definitions. Also avoid string, number and boolean objects slow down execution speed

### example:

`objectName.methodName()` or `name = person.fullName();`

## JavaScript Events

#### Events that can happen to HTML elements

## JavaScript Event Handlers

#### Things that should be done every time loading a page or closing and action that should b preformed when clicking a button. Content that should be verified when a user inputs data.

## JavaScript String

#### Methods and properties are available to primitive values but cannot have properties or methods

## JavaScript string length

### Example:

```js
let txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
let length = txt.length;
```

## Extracting String parts

#### Slice (start, end) extracts a port and returns the extracted part to a new string

### example:

```js
let str = “Orchid, Hibiscus, Rose ;
let part = str.slice(7, 13);
```

### example if negative:

```js
let str = “Orchid, Hibiscus, Rose” ;
let part = str.slice(-12, -6);
```

#### substring (start, end) start and end values less than 0 are treated as 0 in `substring()` and sustr(start, length) second parameter specifies the length of the extracted part.

## Replacing String Content

#### Strings are immutable and strings cannot be changed only replaced.This returns a new string and replaces only the first match. Make sure to replace all matches us `/g` flag set.

### example first match:

```js
let text = "Please visit Microsoft!";
let newText = text.replace("Microsoft", "W3Schools");
```

### Example of all matches:

```js
let text = "Please visit Microsoft and Microsoft!";
let newText = text.replace(/Microsoft/g, "W3Schools");
```

## JavaScript string `toUpperCase()`

### Example:

```js
let text1 = "Hello World!";
let text2 = text1.toUpperCase();
```

## JavaScript string `toLowerCase()`

### Example:

```js
let text1 = "Hello World!"; // String
let text2 = text1.toLowerCase(); // text2 is text1 converted to lower
```

## JavaScript String `concat()`

#### Joining two or more strings and used instead of plus operator

## JavaScript string `trim()`

#### Removes whitespace

### Example:

```js
let text1 = "      Hello World!      ";
let text2 = text1.trim();
```

## JavaScript string `padstart()`

#### String to pad a number, convert the number to a string first

### Example:

```js
let numb = 8;
let text = numb.toString();
let padded = text.padStart(7,”0”);
```

## JavaScript `padEnd()`

### Example:

```js
let text = “8”;
let text = numb.toString();
let padded = text.padEnd(7,”0”);
```

## Extracting String Characters

#### charAt (position) returns the charter at a specified position in a string

### Example:

```js
let text = "HELLO WORLD";
let char = text.charAt(0);
```

#### charCodeAt (position) returns the unicode of the character at a specified index in a string (returns a UTF-16 code)

### Example:

```js
let text = "HELLO WORLD";
let char = text.charCodeAt(0);
```

## Property access [ ]-ECMAScript (09) allows access on strings

### Example:

```js
let text = "HELLO WORLD";
let char = text[0];
```

## JavaScript string `split( )`

#### String can be converted to an array with the split()

### Example:

```js
text.split(","); // Split on commas
```

#### If separator is omitted, returned array will contain the whole string in index [0] but if separator is `“ “`, returned array will be an array of single character

## JavaScript Search Methods

## String `indexOf().`

##### Returns the index of the first occurrence of a specified text in a string but cannot take a powerful search values (reg. expressions)

## `Search()`

#### Searches a string for a specified value and returns the position of the match but cannot take a second start position argument

## `String lastIndexOf()`

#### Returns the index of the last occurrence of a specified text in a string. If second parameter is 18, search starts at position 18 then searches to the beginning of the string.

## `String startsWith()`

#### Return -1 if the text is not found

## `String endsWith().`

#### Return -1 if the text is not found

## JavaScript String `match()`

#### Searches a string for a match against a reg. expression and return the matches as an array object

## JavaScript String `includes()`

#### Returns true if a string contains a specified value

## JavaScript String `startsWith()`

#### Returns true if a string begins with a specified value, otherwise false and case sensitive

## JavaScript String `endsWith()`

#### Returns true if a string ends with a specified value, otherwise false and case sensitive

## JavaScript Template Literals

##### Back-Tics Syntax ` ` instead `“ “` define a string. Quotes inside strings use both single and double quotes inside a string

### Example:

```js
let text = `She’s often called “Miranda”`;
```

#### Multiline strings allow multiple strings

#### Interpolation is an easy way to interpolate variables and expressions into a string

#### Variable Substitutions are variables in strings

#### String interpolation is automatic replacing of variables with real values ion a string

#### Expression Substitution are expressions in a string

#### String interpolation is automatic replacing of substitution with real values ion a string

```js
// left off on JavaScript Number Methods
```
