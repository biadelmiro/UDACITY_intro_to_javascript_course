# Intro to JavaScript
A collection of summaries to Udacity's Intro to JavaScript

## Table of Contents
1. [What is JavaScript?](#what-is-javascript)
   1. [Introduction to JavaScript](#introduction-to-javascript)
   2. [History of JavaScript](#history-of-javascript)
   3. [The JavaScript Console](#the-javascript-console)
   4. [Developer Tools on Different Browsers](#developer-tools-on-different-browsers)
   5. [Console Log](#console-log)
   6. [JavaScript Demo](#javascript-demo)
   7. [Lesson 1 Summary](#lesson-1-summary)
2. [Data Types and Variables](#data-types-and-variables)
   1. [Introduction to Data Types](#introduction-to-data-types)
   2. [Numbers](#numbers)
   3. [Comments](#comments)
   4. [Quiz: First Expression (2-1)](#quiz-first-expression-2-1)
   5. [Strings](#strings)
   6. [String Concatination](#string-concatination)
   7. [Variables](#variables)
   8. [Quiz: Converting Temperatures (2-2)](#quiz-converting-temperatures-2-2)
   9. [String Index](#string-index)
   10. [Escaping Strings](#escaping-strings)
   11. [Comparing Strings](#comparing-strings)
   12. [Quiz: Favorite Food (2-3)](#quiz-favorite-food-2-3)
   13. [Quiz: String Equality for All (2-4)](#quiz-string-equality-for-all-2-4)
   14. [Quiz: All Tied Up (2-5)](#quiz-all-tied-up-2-5)
   15. [Quiz: Josa Buson (2-6)](#quiz-josa-buson-2-6)
   16. [Booleans](#booleans)
   17. [Quiz: Facebook Post (2-7)](#quiz-facebook-post)
   18. [Null, Undefined and NaN](#null-undefined-and-nan)
   19. [Equality](#equality)
   20. [Quiz: Semicolons!(2-8)](#quiz-semicolons-2-8)
   21. [Quiz: What's My Name?(2-9)](#quiz-whats-my-name-2-9)
   22. [Quiz: Out to Dinner (2-10)](#quiz-out-to-dinner-2-10)
   23. [Quiz: Mad Libs (2-11)](#quiz-mad-libs-2-11)
   24. [Quiz: One Awesome Message (2-12)](#quiz-one-awesome-message-2-12)
   25. [Lesson 2 Summary](#lesson-2-summary)
3. [Conditionals](#conditionals)
4. [Loops](#loops)
5. [Functions](#functions)
6. [Arrays](#arrays)
7. [Objects](#objects)

## What is JavaScript?
### Introduction to JavaScript
JavaScript is a programming language for the web and is the the final piece needed to make your websites come to life. It was created to make it easier to add interactive and dynamic elements to websites. Today, the language is used for all sorts of applications, from programming a robot with an Arduino to writing a game script in Unity or even building a code editor. It has grown to be one of the most popular languages in the world and is considered one of the three foundational pillars of front end web development.

### History of JavaScript
JavaScript was created in just 10 days by Brendan Eich back in 1995 while he was working on Netscape Navigator which was one of the Internet’s first web browsers. Nowadays, mostly Google Chrome, Mozilla Firefox, Apple Safari and Microsoft Edge are used to surf the web. Prior to Eich’s creation of JavaScript, websites just existed as pages of HTML and CSS with the occasional plug-in or Java applet. JavaScript was originally called LiveScript, but was changed to JavaScript as a marketing decision in order to ride on the coattails of Java's popularity at the time. As the language evolved, competing versions of the language emerged. So JavaScript was eventually taken to Ecma International to be standardized. Today, the language itself is still referred to as JavaScript, however, recent versions are referenced by their ECMAScript version number, such as, ES5 or ES6. Even more recently, the standards body has transitioned to a year-based number to promote a more consistent release cycle with ES2016, ES2017, etc.

### The JavaScript Console

In Google Chrome, you can access the console by opening the developer tools, which can be done by right clicking the page and selecting inspect. Once open, navigate to the console tab. Alternatively, the keyboard shortcut is Cmd+Option+J on a Mac or Ctrl+Shift+J on Windows. For more Chrome developer tools keyboard shortcuts [click here](https://developers.google.com/web/tools/chrome-devtools/shortcuts).

You can write and test JavaScript code directly in the console. For example, to write your first line of code you could start by writing your name. As you see, just writing your name will actually result in an error. To be able to actually write your name in JavaScript without an error you need to format your name as a data type called a string put inside quotes:
```js 
"Michael"
```
Why don’t we try something else? Here’s some code that creates an alert that says, Hello, Julia, how are you? And it pushes it to the browser:
```js
alert("Hello, Michael! How are you?!");
```
Now writing code directly in your browser is something you can do to test out new code snippets where you’re not really sure what they do. But it could actually get pretty annoying once you start writing larger and larger programs. For example, if you wanted to create more than just one alert, it may seem simple at first, but each time you need to go to the next line, you would have to type Shift+Return instead of just the Return key.
```js
alert("Hello");
alert(":(");
```
```js
alert("Hello");
alert("This is great!");
alert("JavaScript is fun!");
```
This is going to get pretty annoying pretty fast. Eventually, you’ll learn about other ways to run JavaScript files. But for now we recommend using a text editor like Atom or Sublime Text and then pasting your code in the console once you’re ready to test it.

### Developer Tools on Different Browsers
Every modern web browser includes its own set of developer tools. Developer tools allow you to debug and test out your ideas directly in the browser. If you're familiar with HTML or CSS, you may have used them to experiment with the style of a webpage, however, you can also use them with JavaScript. They are often used as a sandbox, that is, a place to mess around with any code without any long-term consequences. You can use them to debug problems you run in to or to test a piece of code. If you open any website that uses JavaScript, the console will tell you if there are any warnings or errors on the page and will also display any output and print it with console.log. Warnings and errors are very common when visiting sites and will not affect your code.

DevTools can be separated into three categories; independent, Mac and Windows. Independent browsers, such as, Google Chrome, Mozilla Firefox and Opera can be used regardless of operating system. Specific browsers, such as, Safari, Internet Explorer and Microsoft Edge Mac are dependent on their respective Mac or Windows operating system. Below is a guide to the various web browsers and their respective developer tools:

- [Independent](#independent)
- [Mac](#mac)
- [Windows](#windows)
- [Further Reading](#further-reading)

#### Independent
With most independent browsers, such as, Google Chrome, Mozilla Firefox and Opera, you can access them with a right-click on an element and then selecting Inspect Element. Alternatively, you can use the following shortcuts:
- Command + Option + i (Mac)
- Ctrl + Shift + i (Windows/Linux).

#### Mac
Safari has the same options to access it's DevTools as with independent browsers, however, you first have to enable the Develop menu in Safari’s Advanced preferences in order to use them.

#### Windows
Internet Explorer and Microsoft Edge have the F12 DevTools, which are accessible by simply pressing F12 on the Keyboard. Testing for Internet Explorer 8, 9, 10 and 11 is arguably still best practice for web based projects, because they often present unique problems. Apparently, due to Microsoft Edge's tools having been written in TypeScript, it is always running and no reload is required. In addition, F12 developer tools documentation is now fully available on [GitHub](https://github.com/MicrosoftDocs/edge-developer).

#### Further Reading
- [Google Chrome](https://developers.google.com/web/tools/chrome-devtools/)
- [Mozilla Firefox](https://developer.mozilla.org/en-US/docs/Tools)
- [Opera](https://www.opera.com/dragonfly/)
- [Safari](https://developer.apple.com/safari/tools/)
- [Internet Explorer 8](https://msdn.microsoft.com/en-us/library/dd565628.aspx)
- [Internet Explorer 9](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/samples/gg589512(v=vs.85))
- [Internet Explorer 10](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/dev-guides/hh673549(v=vs.85))
- [Internet Explorer 11](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/dev-guides/bg182636(v=vs.85))
- [Microsoft Edge](https://docs.microsoft.com/de-de/microsoft-edge/devtools-guide)

### Console Log
console.log is used to print content to the JavaScript console:
```js
console.log("hiya friend!");
```
**Prints:** "hiya friend!"

The message logged is a data type called a **string** (a sequence of characters).

#### Optional demo example
Let’s use console.log to do something a little more interesting. Here’s a block of JavaScript code that loops through the numbers 0 through 9 and prints them out to the console:
```js
for (var i = 0; i < 10; i++) {
  console.log(i);
}
```
**Prints:** 0 1 2 3 4 5 6 7 8 9

This is called a **loop**.

Based on this loop's settings, any code written inside the curly brackets {...} will be repeated 10 times. In this case, console.log is printing out the value of i each time the loop runs. Don't worry if you're not sure about what the syntax means at this point. You will learn more about how and when to use loops later.

### JavaScript Demo
So you saw how to use console.log to print a message to the JavaScript console. Now, let’s see how you can use the console as a sandbox to test a new line of JavaScript in the browser.

Open [the following site](https://daringfireball.net/projects/markdown/) in a new tab and in that tab also open up developer tools. Then paste the following code:
```js
document.getElementsByTagName("h1")[0].style.color = "#ff0000";
```
As you can see, the heading changed red. Styling elements on the page is great, but you could also do that by just modifying the CSS. What makes JavaScript so special in this case? Refresh the page, then paste this line of code in the JavaScript console.
```js
document.body.addEventListener('click', function () {
     var myParent = document.getElementById("Banner"); 
     var myImage = document.createElement("img");
     myImage.src = 'https://thecatapi.com/api/images/get?format=src&type=gif';
     myParent.appendChild(myImage);
     myImage.style.marginLeft = "160px";
});
```
If you’re confused because nothing happened. Don’t worry. Click somewhere on the page. As you can see, an image was added to the page.

### Summary
Before we move on to the JavaScript language itself, how about we recap some of the things you just learned? First, you learned that all major browsers come with built-in JavaScript engines. This allows browsers to run and execute JavaScript code. Next, you got practice using the JavaScript console. The JavaScript console allows you to print strings and execute lines of JavaScript code on the fly, right inside of your browser. And finally, you wrapped up with some exercises where you use JavaScript to add styles and animations to a web page. Hopefully, you’re beginning to see the power of JavaScript. And you’re ready to dive in and explore the language.

## Data Types and Variables
### Introduction to Data Types
Data is everywhere. It’s the grade you made on your first math test, it’s the conversation you have with a loved one and it’s the decision you made to sit down and watch this video. All of these things can be represented as data. Data’s important because it helps us understand the world, recognize trends, make educated guesses and inform our future decisions. This is no different in programming. Data and data types are the building blocks of any programming language because they help us organize information and determine how our programs will run. When you look on your Facebook profile, what do you see? Your name, the number of friends you have, the date of your last post, a list of status updates and whether you liked the comment your friend just made. All this information is being gathered, calculated and presented to your friends and family visiting your profile. And when you look at your bank account, what do you see? An account number, an account balance, dates of each transaction and the name of the company that you made a purchase from. It’s important to be aware of what types of data you’re using and when it’s appropriate to use each type. In this lesson, we’ll start by learning how to define and manipulate the primitive data types of JavaScript. Numbers, strings, Booleans, undefined and null. Once you’re familiar with these data types, you’ll see how you can store data into variables so you can reuse and manipulate data throughout your code.

### Numbers
Defining a number in JavaScript is actually pretty simple. The **Number** data type includes any positive or negative integer, as well as decimals. Entering a number into the console will return it right back to you:
```js
3
```
**Returns:** 3

There, you did it.

#### Arithmetic operations
You can also perform calculations with numbers pretty easily. Basically type out an expression the way you would type it in a calculator:
```js
3 + 2.1
```
**Returns:** 5.1

Now you try!

QUESTION 1 OF 2

Enter the expressions (one at a time) into the console and determine what each expression evaluates to:

2 + 10 - 19 + 4 - 90 + 1 = -92

-20 + -19 - (-10) - (-1) + 24 = -4

(10/5) * 4 - 20 = -12

4096 % 12 = 4

#### Comparing numbers
What about comparing numbers? Can you do that? Well of course you can!

Just like in mathematics, you can compare two numbers to see if one’s greater than, less than, or equal to the other:
```js
5 > 10
```
**Returns:** false
```js
5 < 10
```
**Returns:** true
```js
5 == 10
```
**Returns:** false

Comparisons between numbers will either evaluate to true or false. Here are some more examples, so you can try it out!

| Operator | Meaning |
| :---: | :--- |
| < | Less than |
| > | Greater than |
| <= | Less than or equal to |
| >= | Greater than or equal to |
| == | Equal to |
| != | Not equal to |

QUESTION 2 OF 2

Enter the expressions (one at a time) into the console and determine what each expression evaluates to.

| Expression | Solution |
| :---: | --- |
| 43 > 47 | false |
| 12 == 17 | false |
| 3 <= 3 | true |
| 1 != 0 | true |

**TIP:** The values ```true``` and ```false``` have significant importance in JavaScript. These values are called **Booleans** and are another data type in JavaScript. Later in this lesson, you’ll learn more about why Booleans are so important in programming.

### Comments
You can use comments to help explain your code and make things clearer. In JavaScript, comments are marked with a double forward-slash //. Anything written on the same line after the // will not be executed or displayed. To have the comment span multiple lines, mark the start of your comment with a forward-slash and star, and then enclose your comment inside a star and forward-slash /* … */.
```js
// this is a single-line comment

/*
this is
a multi-line
comment
*/
```
Some of the quizzes in this course might include comments that give you hints or instructions to complete the quiz. Comments are often used to clarify and document non-obvious code. It's good practice to include code comments to improve code readability.

Alright, good luck!

### Quiz: First Expression (2-1)
#### Directions:
Write an expression that uses at least 3 different arithmetic operators.

The expression should equal 42.

**Hint:** +, -, *, /, and % are possible arithmetic operators

**Your Code:**
```js
/*
 * Programming Quiz: First Expression (2-1)
 *
 * Write an expression that uses at least three, different, arithmetic operators
 * to log the number 42 to the console.
 */

// this expression equals 4, change it to equal 42
console.log(4 * 10 + 8 - 6);
```

### Strings
Let’s take a look at the string datatype. You’ve actually used a string before, and maybe just didn’t know it. When you type a message inside console.log, that message is actually just a JavaScript string. So here, Hiya, Friend, is just a string. Strings can be single letters, like the character h, or even contain numbers, like the string 123. The important thing is that you use quotes to signify a string. It doesn’t matter if the quotes are single or double quotes, but they do have to match. I used double quotes here and single quotes here. If I try to pass the string to the console.log but forget to use the quotes, JavaScript will return back an error. I get this reference error, because the JavaScript engine thinks I’m talking about a variable called hello instead of a string with the value of hello. We haven’t talked about variables just yet, but the moral of the story here is to remember to use quotes when using strings. If I add the quotes in, then the string gets printed out to the console.

**TIP:** It is correct to either use “ or ‘ quotes with strings, as long as you’re consistent. The [JavaScript Udacity style guide](http://udacity.github.io/frontend-nanodegree-styleguide/javascript.html) for labs and projects suggests using single quotes to define string literals.

### String Concatination
**Strings** are a collection of characters enclosed inside double or single quotes. You can use strings to represent data like sentences, names, addresses, and more. Did you know you can even add strings together? In JavaScript, this is called **concatenating**. Concatenating two strings together is actually pretty simple!
```js
"Hello," + " New York City"
```
**Returns:** "Hello, New York City"

You will see other ways to concatenate and do even more with strings later in this course. But for now, practice using the addition + operator.

QUESTION 1 OF 3

What's the result with ```"hello" + "world"```?

**Answer:** "helloworld"

QUESTION 2 OF 3

What do you think will happen when you type ```"Hello + 5*10"``` into the JavaScript console?

**Answer:** "Hello + 5*10"

QUESTION 3 OF 3

What do you think will happen when you type ```"Hello" + 5*10``` into the console?

**Answer:** "Hello50"

### Variables
So you have all these numbers, strings and booleans, but what are you supposed to do with them? All this data so far has been for a one time use only. You define the string, Hello, it’s returned and that’s it. That’s the end. The string Hello is now gone. You need a way to be able to store data, so that you can use it or change it later. To do this you can use variables. You’ve probably heard of variables before, maybe in a math class. Let’s say you have a variable called X, and it’s assigned the value 5. And then let’s say we have the expression X + 1. Since X has the value of 5, we can substitute the value of 5 in for X. So the expression becomes 5 + 1 = 6. In JavaScript, variable stored data, much like how the variable you just saw stored the value of 5. And they’re not limited to the storing of just numerical values, you can store any variable in to a variable. To create a variable, use the var keyword followed by the variableName, and the assignment operator. The assignment operator is the equal sign. And then on the right side of the assignment operator, put the value you want to assign to the variable. As an example, here’s my cat Zoe. We can use a variable called name and set it equal to the string Zoe for her name. And for her age, we can create a variable called age, and set that to the number 4, since Zoe’s 4 years old. Eventually, when Zoe has her next birthday, I’ll be able to use the age variable I created to increment Zoe’s age by 1, so the variable age will return Zoe’s updated age of 5. Now, Zoe’s 5 years old.

With variables, you no longer need to work with one-time-use data.

At the beginning of this course, you declared the value of a string, but you didn't have a way to access or reuse the string later.
```js
"Hello"; // Here's a String "Hello"
"Hello" + " World"; // Here's a new String (also with the value "Hello") concatenated with " World"
```
Storing the value of a string in a variable is like packing it away for later use.
```js
var greeting = "Hello";
```
Now, if you want to use "Hello" in a variety of sentences, you don't need to duplicate "Hello" strings. You can just reuse the ```greeting``` variable.
```js
greeting + " World!";
```
**Returns:** Hello World!
```js
greeting + " Mike!";
```
**Returns:** Hello Mike!

You can also change the start of the greeting by reassigning a new string value to the variable ```greeting```.
```js
greeting = "Hola";
greeting + " World!";
```
**Returns:** Hola World!
```js
greeting + " Mike!";
```
**Returns:** Hola Mike!

#### Naming Conventions
When you create a variable, you write the name of the variable using camelCase (the first word is lowercase, and all following words are uppercase). Also try to use a variable name that accurately, but succinctly describes what the data is about.
```js
var totalAfterTax = 53.03; // uses camelCase if the variable name is multiple words
var tip = 8; // uses lowercase if the variable name is one word
```

Not using camelCase for your variables names is not going to necessarily *break* anything in JavaScript. But there are recommended style guides used in all programming languages that help keep code consistent, clean, and easy-to-read. This is especially important when working on larger projects that will be accessed by multiple developers.

You can read more about Google's JavaScript StyleGuide [here](https://google.github.io/styleguide/jsguide.html).

QUIZ QUESTION

Which of these are good variable names?
```js
var thingy = 1;

var count = 1;

var postLiked = false;

var firstname = "Richard";
```
**Answer:**
```js
var count = 1;

var postLiked = false;
```
### Quiz: Converting Temperatures (2-2)
To convert [Celsius](https://en.wikipedia.org/wiki/Celsius) to [Fahrenheit](https://en.wikipedia.org/wiki/Fahrenheit), you can use the following formula:

F=C×1.8+32

#### Directions:
Use this equation and the variables ```fahrenheit``` and ```celsius``` to print the Fahrenheit equivalent of 12°C.

**NOTE:** "12°C" reads as "12 degrees Celsius".

**Your Code:**
```js
/*
 * Programming Quiz: Converting Tempatures (2-2)
 *
 * The Celsius-to-Fahrenheit formula:
 *
 *    F = C x 1.8 + 32
 *
 * 1. Set the fahrenheit variable to the correct value using the celsius variable and the forumla above
 * 2. Log the fahrenheit variable to the console
 *
 */

var celsius = 12;
var fahrenheit = celsius * 1.8 + 32;

console.log(fahrenheit);
```
### String Index
#### Indexing
Did you know that you can access individual characters in a string? To access an individual character, you can use the character's location in the string, called its **index**. Just put the index of the character inside square brackets (starting with ```[0]``` as the first character) immediately after the string. For example:
```js
"James"[0];
```
**Returns:** "J"

or more commonly, you will see it like this, using a variable:

```js
var name = "James";
name[0];
```
**Returns:** "J"

Characters within a string are indexed starting from 0, where the first character is at position 0, to n-1, where the last character is at position n-1 (n represents the total number of characters within a string).

QUIZ QUESTION

What character will be printed to the JavaScript console after running the following lines of code.
```js
var quote = "Stay awhile and listen!";
console.log(quote[6]);
```
**Answer:** w

### Escaping Strings
#### Escaping strings
There are some cases where you might want to create a string that contains more than just numbers and letters. For example, what if you want to use quotes in a string?
```js
"The man whispered, "please speak to me.""
```
**Uncaught SyntaxError:** Unexpected identifier
If you try to use quotes within a string, you will receive a ```SyntaxError``` like the one above.

Because you need to use quotes to denote the beginning and end of strings, the JavaScript engine misinterprets the meaning of your string by thinking ```"The man whispered, "``` is the string. Then, it sees the remaining ```please speak to me.""``` and returns a ```SyntaxError```.

If you want to use quotes *inside a string*, and have JavaScript not misunderstand your intentions, you’ll need a different way to write quotes. Thankfully, JavaScript has a way to do this using the backslash character ( \ ).

If you forget to use the backslash to escape characters, then the JavaScript engine can misinterpret your strings.

#### Escaping characters
In JavaScript, you use the backslash to **escape** other characters.

*Escaping a character* tells JavaScript to ignore the character's special meaning and just use the literal value of the character. This is helpful for characters that have special meanings like in our previous example with quotes ```"…"```.

Because quotes are used to signify the beginning and end of a string, you can use the backslash character to escape the quotes in order to access the literal quote character.
```js
"The man whispered, \"please speak to me.\""
```
**Returns:** The man whispered, "please speak to me."

This guarantees that the JavaScript engine doesn’t misinterpret the string and result in an error.

By using the backslash to escape characters, the JavaScript engine can understand the meaning of your strings.

#### Special characters
Quotes aren’t the only special characters that need to be escaped, there’s actually [quite a few](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Using_special_characters_in_strings). However, to keep it simple, here’s a list of some common special characters in JavaScript.

| Code | Character |
| :--- | :--- |
| \\ | \ (backslash) |
| \" | '' (double quote) |
| \' | ' (single quote) |
| \n | newline |
| \t | tab |

The last two characters listed in the table, newline ```\n``` and tab ```\t```, are unique because they add additional **whitespace** to your Strings. A newline character will add a line break and a tab character will advance your line to the next [tab stop](https://en.wikipedia.org/wiki/Tab_stop).
```
"Up up\n\tdown down"
```
**Returns:**
```
Up up
   down down
```
QUIZ QUESTION

Select the string that returns the following output:
```js
"The file located at "C:\\Desktop\My Documents\Roster\names.txt" contains the names on the roster."
```
**Answer:**
```js
"The file located at "C:\\Desktop\My Documents\Roster\names.txt" contains the names on the roster."
```
### Comparing Strings
#### Comparing strings
Another way to work with strings is by comparing them. You've seen the comparison operators ```==``` and ```!=``` when you compared numbers for equality. You can also use them with strings! For example, let’s compare the string ```"Yes"``` to ```"yes"```.
```js
"Yes" == "yes"
```
**Returns:** false

When you run this in the console, it returns false. Why is that? ```"Yes"``` and ```"yes"``` are the same string, right? Well not quite.

##### Case-sensitive
When you compare strings, case matters. While both strings use the same letters (and those letters appear in the same order), the first letter in the first string is a capital ```Y``` while the first letter in the second string is a lowercase ```y```.
```js
'Y' != 'y'
```
**Returns:** true

QUIZ QUESTION

Enter each expression into the console. Check the ones that evaluate to ```true```.
```js
"green" == "blue" // false
"green" == "green" // true
"green" == "Green" // false
"Green" == "green" // false
"green" > "blue" // true
"green" > "green" // false
"green" > "Green" // true
"Green" > "green" // false
```
**Answers:**
```js
"green" == "green"
"green" > "blue"
"green" > "Green"
```

### Quiz: Favorite Foods (2-3)
#### Directions:
Create a string with the name of your favorite food. The first letter of the string should be capitalized.

**Your Code:**
```js
/*
 * Programming Quiz: Favorite Food (2-3)
 */

console.log("Pizza");
```

### Quiz: String Equality for All (2-4)
#### Directions:
Fix the right side expression so it evaluates to ```true```.

**Your Code:**
```js
/*
 * Programming Quiz: String Equality for All (2-4)
 */

// fix the right side of the expression
var answer = "ALL Strings are CrEaTeD equal" == "ALL Strings are CrEaTeD equal";
console.log(answer);
```

### Quiz: All Tied Up (2-5)
#### Directions:
Build a single string that resembles the following joke.

```
Why couldn't the shoes got out and play?
They were all "tied" up!
```
Your joke should take the format of a **question** and **answer**. The first line should be a question and the second line should be an answer.

**Hint:** *You will need to use special characters to produce the following output.*

**Your Code:**
```js
/*
 * Programming Quiz: All Tied Up (2-5)
 */

var joke = "Why couldn\'t the shoes got out and play?\nThey were all \"tied\" up!"
console.log(joke);
```

### Quiz: Yosa Buson (2-6)
#### Directions:
Build a string using concatenation by combining the lines from this famous haiku poem by [Yosa Buson](https://en.wikipedia.org/wiki/Yosa_Buson).
```
Blowing from the west
Fallen leaves gather
In the east.
```
Each string should be printed on its own line.

**Hint:** *You will need to use special characters to produce the following output. For a refresher, feel free to review the previous **Escaping Strings** lesson in this course.*

**Your Code:**
```js
/*
 * Programming Quiz: Yosa Buson (2-6)
 */

var haiku = "Blowing from the west\n" + "Fallen leaves gather\n" + "In the east."
console.log(haiku);
```

### Booleans
You’ve now seen how you can perform basic operations, as well as comparisons on numbers and strings. Whenever you compare data, the result of the comparison will always be a value of true or false. This is important, because our third primitive data type, Booleans, only includes these two values. Just think, yes or no, on and off, true or false, ones and zeroes. These are all values that really represent the same thing. And this Boolean logic is a huge part of how we think about problems. Code either runs or it doesn’t, there’s no in-between, at least not in programming. In this section, you’ll dive deeper into Booleans by comparing data of different types and learning about different ways to express equality.

### Quiz: Facebook Post (2-7)
### Null, Undefined and NaN
### Equality
### Quiz: Semicolons! (2-8)
### Quiz: What's My Name? (2-9)
### Quiz: Out to Dinner (2-10)
### Quiz: Mad Libs (2-11)
### Quiz: One Awesome Message (2-12)
### Lesson 2 Summary

## Conditionals
## Loops
## Functions
## Arrays
## Objects
