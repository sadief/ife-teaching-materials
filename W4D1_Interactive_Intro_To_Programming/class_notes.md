## W4D1 Intro to Javascript

Hey everyone! We're officially halfway through the program and done the HTML and CSS portion! Now we're learning Javascript!

### console.log

console.log is a function that is built into JavaScript and is used for printing values to the screen and helping to fix bugs in code.

### Comments

Comments are notes for you the developer. They are like sticky notes written in invisible ink that the outside world (your computer) can't see.

### Data Types

All the values we use in JavaScript are of a certain type. When we write JavaScript, it's important to remember what types we use so we can understand how our code will behave.

#### Numbers

Numbers are just like numbers in real life. We can use JavaScript to add, subtract, multiply, and divide Numbers

```javascript
// Add
1 + 1;
// Subtract
10 - 1;
// Multiply
10 * 2;
// Divide
10 / 2;
```

#### Strings

Strings are words! They can be used to represent many different things in code. We use quotation marks to represent strings in JavaScript. You can use either single or double quotation marks.

```javascript
// Can contain letters
"Hello";
// Can contain Numbers (this is a STRING not a NUMBER)
"123";
// Can contain symbols
"Huh?!?!!?";
// Or all of them
"alsdfklj230823roi";
```

You can add (concatenate) Strings

```javascript
console.log("Hello " + "There");
```

- Remember computers don't recognize whitespace so you have to factor that in.

#### Booleans

Booleans represent values that are either true or false.

```javascript
console.log(true);
console.log(false);
console.log("true"); //Not a boolean - this is a STRING
```

### Comparison Operators

Comparison Operators are used to compare two values

#### Equality

The triple equals sign checks to see if tow values are the same value AND the same type and will return a boolean value.

```javascript
console.log("Lighthouse Labs" === "Lighthouse Labs");
// This will return true because they are the same string

console.log("1" === 1);
// This will return false because they are not the same type.
```

#### Greater Than

```javascript
console.log(1 > 10);
// This will return false because 1 is not greater than 10
console.log(100 > 76);
// This will return true because 100 is greater than 76
```

#### Less Than

```javascript
console.log(1 < 10);
// This will return true because 1 is less than 10
console.log(100 < 76);
// This will return false because 100 is not less than 76
```

#### Not Equal

Not equal is evaluated using '!=='

```javascript
console.log(1 !== 10);
// This will return true because 1 is not equal to 10
console.log(100 !== 100);
// This will return false because 100 is equal to 100
```

### Variables

Variables are used when you want to save a value for later to be reused

```javascript
var firstName = "Lighthouse";
```

To declare a variable:

1. Start with the keyword var
2. Add a variable name(use camelCase)
3. Assign a value

### If Statements

If statements help us control what our program will do in specific circumstances.

```javascript
if (condition) {
  // Do something
}
```

To write an if statement:

1. Use the keyword 'if'
2. Have a condition to evaluate
3. Have an action to execute.

If you have more than two conditions you can use else if - you can have multiple else if's but only ever one 'else'

```javascript
var temperature = 12;

if (temperature < 0) {
  console.log("You should wear a scarf");
} else if (temperature < 15) {
  console.log("Wear long sleeves");
} else if (temperature > 25) {
  console.log("Bring a sun hat");
} else {
  console.log("You should be fine with a sweater");
}
```

### Functions

A function is a block of code that executes in a certain order.

- Arguments are passed into a Function
- You can change the arguments each time you run the function, but the way it runs will be the same.
- The function returns a result.

```javascript
function nameIt() {
  // Do Something
}

nameIt();
```

You can add parameters by:

```javascript
function nameIt(parameter) {
  /Do something with parameter
}

nameIt(parameter);
```
