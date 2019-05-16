## W4D1 Intro to Javascript Part II

Hey everyone! Great work tonight! So today we did a review of:

- Console.logs
- Data types
- Variables
- If statements
- Functions

Then we looked at Objects, Arrays, and Loops

### Objects

Objects are a way of organizing related information in key-value pairs which we can save inside variables.

Objects are best when you want to organize based on data labels sort of like a newspaper. When you read a newspaper you don’t necessarily read it back to front - you flip to different sections based on a section's name.

Wherever that section in the newspaper is located, you can flip to it immediately and have the right context.

This is different from a book, where the order of the chapters and sections matter.

If you need a real world example, check out this analogy: [JavaScript Arrays and Objects are like Book and Newspapers](https://medium.freecodecamp.org/javascript-arrays-and-objects-are-just-like-books-and-newspapers-6e1cbd8a1746)

```javascript
var book= {
      title: “Harry Potter and the Prisoner of Azkaban”,
    author: “J.K Rowling”,
    releaseDate: “July 8, 1999”,
}
```

To access the values stored in an object you can use:

**_Bracket Notation:_** call the name of the object then the key name you are accessing. They key name is wrapped in square brackets.
`book['title']``

**_Dot Notation:_** call the name of the object, then a dot and the key name you are accessing;
These behave the same way but sometimes you’ll need to use bracket notation (which we will learn in later classes!)
`book.title`

### Arrays

Arrays let your store a list or collection of items.

In JavaScript, an array can be of any length and contain any data type.

Both arrays and objects and be used to store related pieces of data.

To define an array, we can assign it to a variable.

We list items in an array and separate each item with a comma.

```javascript
var readingList = [“1984”, “The Great Gatsby”, “Lord of the Flies”, “Charlotte’s Web”, “The Hobbit”]

	var mixedArray = [“string”, true, 23, 37, false, “false”]
```

To access values in an array we use the same bracket notation we use for objects,
But instead of key names we put the values “index” or the position inside the array.

**_ARRAYS START AT ZERO_** - so the first position is accessed by using zero.

`readingList[4]` will give us The Hobbit.

### Loops

Loops are a really useful feature of JavaScript.

They let us repeat the same action or piece of code to each item in a set.

For loops are used to loop over arrays:

`for`
The keyword

`()`
The loop’s expressions will be wrapped in round braces

`var i = 0`

The first expression initializes the loop with a new variable named i for “index”. We set it to zero so the loop starts at the first item in the and counts up.

`i < array.length`

The second expression is the loop’s condition. It tells the loop to keep running as long as the “ index ” is less than the length of the array being looped over;
.length: Like “console.log” this is another javascript helper function. It will return the length of an array.

`i++`

A final expression that is evaluated at the end of each loop. It usually updates the counter variable “ i “.
“ i++” increments the counter by +1.

```javascript
for (var i = 0; i < readingList.length; i++) {
  console.log(readingList[i]);
}
```

### While loops

While loops will keep performing their action until the condition provided evaluates to false.

```javascript
var count = 1;

while (count < 10) {
  console.log(count);
  count += 2;
}
```
### Fizz Buzz

```javascript
for (var i = 1; i < 101; i++) {
  if (i % 15 == 0) {
    console.log("FizzBuzz");
  } else if (i % 3 == 0) {
    console.log("Fizz");
  } else if (i % 5 == 0) {
  console.log("Buzz");
  } else {
    console.log(i);
  }
}
```

### Yellow Pager

```javascript
function yellowPager(word) {
  let str = word.toLowerCase().split("");
  if (str.length != 10) {
    return false
  }
  let answer = "";

  for (var i = 0; i < str.length; i++) {
    if (str[i] == "a" || str[i] == "b" || str[i] == "c") {
      answer += "2";
    } else if (str[i] == "d" || str[i] == "e" || str[i] == "f") {
      answer += "3";
    } else if (str[i] == "g" || str[i] == "h" || str[i] == "i") {
      answer += "4";
    }
  }

  console.log(answer);
}

yellowPager("Lighthouse");
```

```javascript
function yellowPager(word) {
  let phone = {
    a: 2,
    b: 2,
    c: 2,
    d: 3,
    e: 3,
    f: 3,
    g: 4,
    h: 4,
    i: 4,
    j: 5,
    k: 5,
    l: 5,
    m: 6,
    n: 6,
    o: 6,
    p: 6,
    q: 7,
    r: 7,
    s: 7,
    t: 8,
    u: 8,
    v: 8,
    w: 9,
    x: 9,
    y: 9,
    z: 9,
  }
  let str = word.toLowerCase().split("");
  if (str.length != 10) {
    return false
  }
  let res = []

  for (var i = 0; i < str.length; i++) {
    res.push(phone[str[i]])
  }

  console.log(res.join(""));
}

yellowPager("Lighthouse");
```

Last but not least, [here](https://www.codecademy.com/learn/introduction-to-javascript) is a link to CodeAcademy's Javascript course. It's free and gives some great practice on the things we've covered already to get more comfortable with things like loops etc.
