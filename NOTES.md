JAVA SCRIPT NOTES


JavaScript program is a list of programing statements that are to be executed by a computer.
	*composed of values, operators, expressions, keywords, and // comments
	*executed one by one or same order as they are written
	*Avoid code lines longer than 80 characters 
	*if it doesn’t fit on one line break it after an operator
	*must begin with a letter, $, or _
	*case sensitive
	* - only used for subtractions

JavaScript HTML methods		getElementById()

JavaScript code is inserted between <code>window.alert('hello')</code>
	*as many scripts as you would like in HTML
	*can be placed in the <body> or <head> can be both as well
	*placed in external files

Finds an HTML element example:

```js
document.getElementById("demo").innerHTML = "Hello JavaScript";
```

Change HTML styles example:

```js
document.getElementById("demo").style.fontSize = "16px";
```

Hide HTML elements example:

```js
document.getElementById("demo").style.display = "none";
```

Show HTML elements example:


			document.getElementById("demo").style.display = "block";
				example: <script>document.getElementById("demo").innerHTML = 
							"My First JavaScript";
							</script>
Semicolons ;
	*separate JavaScript statements at the end of each executable statement
	*separated by semicolons multiple statements are allowed 
	*not required but highly recommended

JavaScript White Space:
	*ignores multiple spaces
	*can be added to make your text more readable

JavaScript Code Blocks:
	*can be grouped in code blocks {} to make execution together

JavaScript Syntax:
	*fixed values- literals
		*numbers- written with or without decimals and extra large or extra small numbers can be written with scientific exponent notation
		*strings- text written within double or single quotes ”” or ‘’
	*variable values- variables
		*store data values 
		*var, let and const to declare variables
		*= to assign values to variables
		*allowed in any program

JavaScript Operators:
	*arithmetic operators (+ = * / ) to compute values (called operands)
		*two number can be literals, variables or expressions
	*assignment operators( =)

JavaScript Keywords:
	*let - tells the browser to create variables
	*var- tells the browser to create variables
		*both produce same result
		*hold different data types numbers, strings, objects and more

JavaScript Comments:
	* / / , /* and */
	*ignored not executed 

JavaScript Functions and Events
	*block of JavaScript code that can be executed 
	*Event is pushing a button
	*can be placed in the <head> to push a button in the <body>
	*can be placed in the <body>
	*place as many as you would like
	*External scripts cannot contain <script> 

External JavaScript
	*practical when same code for many different web pages
	
	Example:
	function myFunction() {
  document.getElementById("demo").innerHTML = "Paragraph changed.";
}
	
	*JavaScript files have .js
	*to use you put the name of the script file in the src (source) attribute of a <script>

	Example: 
	<script src="myScript.js"></script>

innerHTML
	*document.getElementById(id) method.
		*id defines the HTML element
	* innerHTML property defines the HTML content
	*Changing the innerHTML property of an HTML element is a common way to display data in HTML

Document. write()
	*testing purposes
	*after an HTML doc is loaded it will delete all existing HTML

Window.alert()
	*display data

console.log()
	*debugging 
	* away for the browser to display data

JavaScript Print
	*no print objects or print methods
	*cannot access output devices rom JavaScript
	* exceptions window.print() in the browser to bring the content of the current window

JavaScript const
	*always declare variables with const unless the blue of the variable changes
		
		example:
		const price1 = 5;
		const price2 = 6;
		let total = price1 + price2;

	*must be assigned a value when declared
	*used when new array, object, function, or RegExp
	*does not define a constant value defines constant reference 
	*change elements of constant array
	*change properties of constant object

JavaScript String Operators
	* + , += can be used to add concatenate strings
	* strings can can have ‘ ‘ or  “ “ as long as they do not match the quotes surrounding the string 

JavaScript Booleans
	* two values true or false 
	* conditional testing 

JavaScript Arrays 
	* written with []
	*separated by ,
	*zero based 1st item is 0 next item is 1

		example: const states = [“Florida, “California”, “Illinois”]

JavaScript Objects
	*written with {}
	* written as name:value pairs, separated by commas
		
		example has 4 properties: const person = {firstName:”Miranda”, lastName:”Olson”, age:35, eyeColor:"brown”};

Accessing Object Properties
	*objects are containers for named values called properties

		example: objectName. propertyName or objectName[‘propertyName’]
	
	*objects can also have methods which are actions that can be preformed on objects and stored in properties as function definitions.

		example: objectName.methodName() or name = person.fullName();
	
	*avoid string, number and boolean objects slow down execution speed 

JavaScript Events
	* events that can happen to HTML elements

JavaScript Event Handlers
	* things that should be done every time loading a page or closing
	*action that should b preformed when clicking a button
	*content that should be verified when a user inputs data

JavaScript String
	* methods and properties are available to primitive values but cannot have properties or methods 	

JavaScript string length example:
	let txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
	let length = txt.length;	

Extracting String parts
	* slice (start, end) - extracts a port and returns the extracted part to a new string
		example: let str = “Orchid, Hibiscus, Rose ;
				let part = str.slice(7, 13);
		example if negative: let str = “Orchid, Hibiscus, Rose” ;
						    let part = str.slice(-12, -6);
		
	*substring (start, end)- start and end values less than 0 are treated as 0 in substring()
	* sustr(start, length)- second parameter specifies the length of the extracted part.

Replacing String Content
	*Strings are immutable: strings cannot be changed only replaced
	*returns a new string
	*replaces only the first match (replace all matches us /g flag set
	example first match: let text = "Please visit Microsoft!";
					    let newText = text.replace("Microsoft", "W3Schools");
	example of all matches: let text = "Please visit Microsoft and Microsoft!";
						   let newText = text.replace(/Microsoft/g, "W3Schools");

JavaScript string toUpperCase()
	example: let text1 = "Hello World!";
			let text2 = text1.toUpperCase();

JavaScript string toLowerCase()
	example: let text1 = "Hello World!";       // String
			 let text2 = text1.toLowerCase();  // text2 is text1 converted to lower

JavaScript String concat()
	* joining tow or more strings
	*used instead of plus operator

JavaScript string trim()
	* removes whitespace 
 		Example: let text1 = "      Hello World!      ";
				 let text2 = text1.trim();

JavaScript string padstart()
	*method is a string
	* to pad a number, convert the number to a string first
		Example: let numb = 8;
				let text = numb.toString();
				let padded = text.padStart(7,”0”);

JavaScript padEnd()
		Example:	let text = “8”;
				let text = numb.toString();
				let padded = text.padEnd(7,”0”);

Extracting String Characters
	*charAt (position)- returns the charter at a specified position in a string
		Example: let text = "HELLO WORLD";
				let char = text.charAt(0);
	*charCodeAt (position)- returns the unicode of the character at a specified index in a string (returns a UTF-16 code)
		Example: let text = "HELLO WORLD";
				let char = text.charCodeAt(0);
	*Property access [ ]-ECMAScript (09) allows access on strings
		Example: let text = "HELLO WORLD";
				let char = text[0];

JavaScript string split ( )
	*string can be converted to an array with the split( ) 
		Example: text.split(",")    // Split on commas
	*if separator is omitted, returned array will contain the whole string in index [0]
	* if separator is “ “, returned array will be an array of single character

JavaScript Search Methods
	* string indexOf(). - returns the index of the first occurrence of a specified text in a string but cannot take a powerful search values (reg. expressions)
		*search() -  searches a string for a specified value and returns the position of the match but cannot take a second start position argument
			* 
	*string lastIndexOf() - returns the index of the last occurrence of a specified text in a string
		*if second parameter is 18, search starts at position 18 then searches to the beginning of the string.
	*string startsWith()  - return -1 if the text is not found
	*string endsWith(). -return -1 if the text is not found

JavaScript String match()
	*searches a string for a match against a reg. expression and return the matches as an array object

JavaScript String includes()
	* returns true if a string contains a specified value

JavaScript String startsWith()
	*returns true if a string begins with a specified value, otherwise false
	*case sensitive

JavaScript String endsWith()
	*returns true if a string ends with a specified value, otherwise false
	*case sensitive

JavaScript Template Literals
	*Back-Tics Syntax  - ` ` instead “ “ define a string
	*quotes inside strings  - use both single and double quotes inside a string
		Example: let text = `She’s often called “Miranda”`;
	*multiline strings. - allows multiple strings
	*interpolation. -easy way to interpolate variables and expressions into a string
	*Variable Substitutions  - variables in strings
		*string interpolation is automatic replacing of variables with real values ion a string
	*Expression Substitution. - expressions in a string
		*string interpolation is automatic replacing of substitution with real values ion a string

        // left off on JavaScript Number Methods