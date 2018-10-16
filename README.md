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
   1. [Intro to Conditionals](#intro-to-conditionals)
   2. [Quiz: Flowcharts (3-1)](#quiz-flowcharts-3-1)
   3. [Flowchart to Code](#flowchart-to-code)
   4. [If...Else Statements](#if-else-statements)
   5. [Else If Statements](#else-if-statements)
   6. [Quiz: Even or Odd (3-2)](#quiz-even-or-odd-3-2)
   7. [Quiz: Musical Groups (3-3)](#quiz-musical-groups-3-3)
   8. [Quiz: Murder Mystery (3-4)](#quiz-murder-mystery-3-4)
   9. [More Complex Problems](#more-complex-problems)
   10. [Logical Operators](#logical-operators)
   11. [Logical AND and OR](#logical-and-or)
   12. [Quiz: Checking your Balance (3-5)](#quiz-checking-your-balance-3-5)
   13. [Quiz: Ice Cream (3-6)](#quiz-ice-cream-3-6)
   14. [Quiz: What do I Wear? (3-7)](#quiz-what-do-i-wear-3-7)
   15. [Advanced Conditionals](#advanced-conditionals)
   16. [Truthy and Falsy](#truthy-and-falsy)
   17. [Ternary Operator](#ternary-operator)
   18. [Quiz: Navigating the Food Chain (3-8)](#quiz-navigating-the-food-chain-3-8)
   19. [Switch Statement](#switch-statement)
   20. [Falling-through](#falling-through)
   21. [Quiz: Back to School (3-9)](#quiz-back-to-school-3-9)
   22. [Lesson 3 Summary](#lesson-3-summary)
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

**Hint:** *You will need to use special characters to produce the following output. For a refresher, feel free to review the previous **Escaping Strings** lesson in this course*.

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
Dissecting a Facebook post is actually quite simple; anything written is most likely to be a String, anything numerical a Number and the Like button certainly a Boolean.

### Null, Undefined and NaN
#### Null and Undefined
So far, we’ve looked at the data types number, string, and boolean. But there are a couple more we need to look at, and those are null and undefined. At first they might seem somewhat confusing, because they are pretty similar. So you might want to replay this explanation a couple of times. Null is a data type that has no value, just like how you can set a variable to a value of 10. You could explicitly set a variable to a value of null. Undefined is a data type that indicates the absence of value. It’s a bit confusing, but it’s not the same as null. Null is a value that means nothing or totally empty. But undefined actually means does not have a value, not even a value of nothing. You could declare a variable x and try to use it, and it will return undefined. It’s undefined because the variable x exists, it just doesn’t have a value yet. If you set a variable to the value of null and try to use it, it will return null. In other words, undefined will be returned to you, if you didn’t assign a value to something. Null will be returned if you purposefully assign the value to nothing.

```null``` refers to the "value of nothing", while ```undefined``` refers to the "absence of value".

#### What is NaN?

```NaN``` stands for "Not-A-Number" and it's often returned indicating an error with number operations. For instance, if you wrote some code that performed a math calculation, and the calculation failed to produce a valid number, ```NaN``` might be returned.
```js
// calculating the square root of a negative number will return NaN
Math.sqrt(-10)

// trying to divide a string by 5 will return NaN
"hello"/5
```

QUIZ QUESTION

What will be printed out?
```js
var signedIn;
console.log(signedIn);
```
**Answer:** undefined

### Equality
#### Equality
So far, you’ve seen how you can use == and != to compare numbers and strings for equality. However, if you use == and != in situations where the data you’re comparing is mixed, it can lead to some interesting results. For example:
```js
"1" == 1
```
**Returns:** true

and
```js
0 == false
```
**Returns:** true

both evaluate to true. Why is that?

#### Implicit type coercion
JavaScript is known as a *loosely typed language*.

Basically, this means that when you’re writing JavaScript code, you do not need to specify data types. Instead, when your code is interpreted by the JavaScript engine it will automatically be converted into the "appropriate" data type. This is called *implicit type coercion* and you’ve already seen examples like this before when you tried to concatenate strings with numbers.
```js
"julia" + 1
```
**Returns:** "julia1"

In this example, JavaScript takes the string ```"julia"``` and adds the number ```1``` to it resulting in the string ```"julia1"```. In other programming languages, this code probably would have returned an error, but in JavaScript the number ```1``` is converted into the string ```"1"``` and then is concatenated to the string ```"julia"```.

It’s behavior like this which makes JavaScript unique from other programming languages, but it can lead to some quirky behavior when doing operations and comparisons on mixed data types.

QUESTION 1 OF 2

What value do you think the result of ```"Hello" % 10``` will be?

**Answer:** NaN

**DEFINITION:** A **strongly typed language** is a programming language that is more likely to generate errors if data does not closely match an expected type. Because JavaScript is loosely typed, you don’t need to specify data types; however, this can lead to errors that are hard to diagnose due to implicit type coercion.

**Example of strongly typed programming language code**
```
int count = 1;
string name = "Julia";
double num = 1.2932;
float price = 2.99;
```
Equivalent code in JavaScript
```js
// equivalent code in JavaScript
var count = 1; 
var name = "Julia";
```
In the example below, JavaScript takes the string ```"1"```, converts it to ```true```, and compares it to the boolean ```true```.
```js
"1" == true
```
**Returns:** true

When you use the ```==``` or ```!=``` operators, JavaScript first converts each value to the same type (if they’re not already the same type); this is why it's called "type coercion"! This is often not the behavior you want, and **it’s actually considered bad practice to use the** ```==``` **and** ```!=``` **operators when comparing values for equality**.

#### Strict equality
Instead, in JavaScript it’s better to use **strict equality** to see if numbers, strings, or booleans, etc. are identical in *type* and *value* without doing the type conversion first. To perform a strict comparison, simply add an additional equals sign ```=``` to the end of the ```==``` and ```!=``` operators.
```js
"1" === 1
```
**Returns:** false

This returns false because the string ```"1"``` is not the same type *and* value as the number ```1```.
```js
0 === false
```
**Returns:** false

This returns false because the number ```0``` is not the same type *and* value as the boolean ```false```.

QUESTION 2 OF 2

Check the expressions that evaluate to ```true```.
```js
"3" > 1 // true
3 != 3 // false
true >= 0 // true
1 !== false // true
"false" === 0 // false
3 === 3 // true
```
### Quiz: Semicolons! (2-8)
One thing to take notice of in all the examples you've seen so far is the use of semicolons ```;``` at the end of each line. Semicolons make it clear where one statement ends and another begins. This is especially handy when multiple lines of code are written on the same line (which is valid JavaScript, but definitely not recommended!). For instance:
```js
var totalAfterTax = 53.03 var tip = 8 // this is incorrect!
```
**Uncaught SyntaxError:** Unexpected token var
```js
var totalAfterTax = 53.03; var tip = 8; // this is correct!
```
Not adding semicolons to the end of each line *can* cause bugs and errors in your programs. JavaScript does have ways to *occasionally* predict where semicolons *should* be, but just like how type coercion can result in some unexpected quirky behavior in JavaScript, it's good practice to not depend on it.

#### Directions:
Define two variables called ```thingOne``` and ```thingTwo``` and assign them values. Print the values of both variables in **one** ```console.log``` statement using concatenation. For example,
```js
red blue
```
where ```"red"``` is the value of ```thingOne``` and ```"blue"``` is the value of ```thingTwo```. **Don't forget to use semicolons**!

**Your Code:**
```js
/*
 * Programming Quiz: Semicolons! (2-8)
 */

var thingOne = "red ";
var thingTwo = "blue";

console.log(thingOne + thingTwo);
```
### Quiz: What's My Name? (2-9)
#### Directions:
Create a variable called ```fullName``` and assign it your full name as a string.

**Your Code:**
```js
/*
 * Programming Quiz: What's my Name? (2-9)
 */

var fullName = "Michael Hodges";
console.log(fullName);
```
### Quiz: Out to Dinner (2-10)
#### Directions:
Create a variable called ```bill``` and assign it the result of 10.25 + 3.99 + 7.15 (don't perform the calculation yourself, let JavaScript do it!). Next, create a variable called ```tip``` and assign it the result of multiplying ```bill``` by a 15% tip rate. Finally, add the ```bill``` and ```tip``` together and store it into a variable called ```total```.

Print the ```total``` to the JavaScript console.

**Hint:** *15% in decimal form is written as* ```0.15```_._

**TIP:** To print out the ```total``` with a dollar sign ( ```$``` ) use string concatenation. To round ```total``` up by two decimal points use the ```toFixed()``` method. To use ```toFixed()``` pass it the number of decimal points you want to use. For example, if ```total``` equals ```3.9860```, then ```total.toFixed(2)``` would return ```3.99```.

**Your Code:**
```js
/*
 * Programming Quiz: Out to Dinner (2-10)
 */

var bill = 10.25 + 3.99 + 7.15;
var tip = bill * 0.15;
var total = bill + tip;

console.log("$" + total.toFixed(2));
```
### Quiz: Mad Libs (2-11)
#### Directions:
[Mad Libs](https://en.wikipedia.org/wiki/Mad_Libs) is a word game where players have fun substituting words for blanks in a story. For this exercise, use the adjective variables below to fill in the blanks and complete the following message.
```js
"The Intro to JavaScript course is __________. James and Julia are so __________. I cannot wait to work through the rest of this __________ content!"
```
```js
var adjective1 = "amazing";
var adjective2 = "fun";
var adjective3 = "entertaining";
```
Assign the resulting string to a variable called ```madLib```.

**Your Code:**
```js
/*
 * Programming Quiz: MadLibs (2-11)
 * 
 * 1. Declare a madLib variable
 * 2. Use the adjective1, adjective2, and adjective3 variables to set the madLib variable to the message:
 * 
 * 'The Intro to JavaScript course is amazing. James and Julia are so fun. I cannot wait to work through the rest of this entertaining content!'
 */

var adjective1 = 'amazing';
var adjective2 = 'fun';
var adjective3 = 'entertaining';

var madLib = "The Intro to JavaScript course is " + adjective1 + ". James and Julia are so " + adjective2 + ". I cannot wait to work through the rest of this " + adjective3 + " content!";
console.log(madLib);
```
### Quiz: One Awesome Message (2-12)
#### Directions:
Here are two awesome messages:
```
Hi, my name is Julia. I love cats. In my spare time, I like to play video games.
Hi, my name is James. I love baseball. In my spare time, I like to read.
```
Declare and assign values to three variables for each part of the sentence that changes (```firstName```, ```interest```, and ```hobby```).

Use your variables and string concatenation to create your own awesome message and store it in an ```awesomeMessage``` variable. Finally, print your awesome message to the JavaScript console.

**Your Code:**
```js
/*
 * Programming Quiz: One Awesome Message (2-12)
 *
 * 1. Create the following variables:
 *     - firstName
 *     - interest
 *     - hobby
 * 2. Create a variable named awesomeMessage and set it to an awesome message using
      string concatenation and the variables above.
 * 3. Log the awesomeMessage variable to the console.
 */

/*
 * Notes:
 * - The `awesomeMessage` should have the format of:
 *   Hi, my name is _____. I love _____. In my spare time, I like to _______.
 *
 * - Using the above as an example, firstName would have been assigned to "Julia",
 *   interest to "cats", and hobby to "play video games" to produce the message:
 *   Hi, my name is Julia. I love cats. In my spare time, I like to play video games.
 *
 * - Be sure to include spaces and periods where necessary!
 */

var firstName = "Julia";
var interest = "cats";
var hobby = "play video games";

var awesomeMessage = "Hi, my name is " + firstName + ". I love " + interest + ". In my spare time, I like to " + hobby + ".";
console.log(awesomeMessage);
```
### Lesson 2 Summary
That about wraps it up for data types and variables. You should congratulate yourself on a job well done. That was a huge lesson. In this lesson, we covered all the basic data types in JavaScript, including numbers, strings, boolean, null and undefined. Also, we looked at how you can store data into variables. Don’t forget operations on numbers and strings. Right, that too. In the next lesson, we’ll build upon your new knowledge of data types and variables to learn how to write code to solve logical problems. See you there.

## Conditionals
### Intro to Conditionals
In the last lesson, you got a basic understanding for how data is represented and stored in the variables. But what good is that data if you can’t put it to use? When you’re writing code, the main goal is to solve a problem. The steps your code takes to solve a problem is known as an algorithm. Ultimately, for any code that you write, you will be breaking down a problem into an algorithm that is executed by a computer. Let me try explaining it another way. Let’s imagine you’re the computer. Do you remember the last time you had to decide whether to purchase something? How did you solve that problem? Besides figuring out if you really wanted or needed the item, your decision to purchase the item was ultimately dependent on whether or not you had enough money to purchase it. So you ask yourself, self, do I have enough money to purchase this item? If you answered, yes, then you purchase the item. But if you answered, no, then you didn’t purchase the item. The process you went through in your head to solve that problem, and the steps you took in order to do so, is really what’s at the heart of writing code. And that’s what you’ll be learning in this lesson. Up next, you’ll see a flowchart. A flowchart is just a diagram for how to solve a problem. Try to look at it, and try to answer the next question.

### Quiz: Flowcharts (3-1)
**DEFINITION:** A **flowchart** is a visual diagram that outlines the solution to a problem through a series of logical statements. The order in which statements are evaluated and executed is called the **control flow**.

QUESTION 1 OF 2

![Flowchart 1](img/buy-the-item-cropped.jpg)

Take a look at the flowchart above. What data type would best represent (Yes/No) if you have enough money to purchase the item?

**Answer:** Boolean

QUESTION 2 OF 2

![Flowchart 2](img/approaching-the-castle-flowchart.jpg)

Here’s a different flowchart for approaching the castle gates. If you decide to storm the castle, what is the immediate resulting outcome?

**Answer:** A dragon appears and attacks!

### Flowchart to Code
Let’s revisit the example from the beginning of the lesson, and try to put it in the context of what’s happening using JavaScript code. Now if you don’t remember, the scenario we had was whether or not to purchase an item from the store. To make this a little more realistic, let’s say the store I’m purchasing the item from is JD’s Department Store. Let’s say the item that I want to purchase is a hammer, and let’s say it costs 15 bucks. I’ll update this flowchart and, okay, there we go, that looks a little better. We’ve got purchased hammer from JD’s Department Store. If we got enough money, yes, buy the hammer. If we don’t, don’t buy the hammer. So the real question here is, do we have enough money to purchase the hammer? And to answer that question, we need to know two things. We need to know how much money do I have, and how much does the hammer cost. Now we already know that the hammer costs $15, so in code, I can store that value in a variable called price. So let’s do that right now. Okay, so Ive got my text editor open, and we’ll say var price = $15. And that’s going to be the price of our hammer, all right. And let’s say, I have $20 on me, and we’ll store that into another code called money, and set that equal to the $20. So this is how much money I have, cool. This gives us enough information to answer whether or not I have enough money to purchase the hammer. But in order to represent that question in code, we’ll need to use a comparison. If you remember back to the last lesson on data types, we can use a comparison to compare two strings or two numbers. So for this situation, I’ll write my comparison to see if my money is greater than or equal to my price of the hammer. Now by itself, we know that this expression will either evaluate to true or false. If it evaluates to true, then I know I’ve got enough money to purchase the hammer. If it evaluates to false, then I’m out of luck and can’t buy the hammer. But this code doesn’t really do anything for us by itself. So here’s where things get really awesome. We can actually represent this question and both possible results using an if else statement. So let me type that out, and then explain what’s going on. Okay, so the way this code reads is if money is greater than or equal to price, then we’ll want to print out, buy the hammer. Otherwise, or else, we’ll want to say, don’t buy the hammer. So what this actually means is, if our money is greater than or equal to the price, run the code inside these curly braces. Otherwise, run the code inside these curly braces. Now pay attention to the curly braces here, because they’re super important. Whatever code is written inside of these things is going to be the code that’s executed when our condition is either true, like it is up here, or false. Also, notice how I’ve indented the code over, so you can tell what part of our code belongs to which block. The code here belongs to our if statement. The code here belongs to our else statement. So to show you this code working, I’m just going to copy and paste it over to the JavaScript console. We paste it in, awesome. That’s what we expect to see. So our money, which is $20 is greater than or equal to the price. So it hits this conditional statement because it’s true, and it prints out, buy the hammer. And just to show you that it can work the other way around, let’s redo the same code, but let’s say, it’s $10 that I have instead of 20. Awesome, then it prints out, don’t buy the hammer.
```js
var price = 15.00; // price of our hammer
var money = 20.00 // how much money i have

if (money >= price) {
   console.log("buy the hammer");
} else {
   console.log("don't buy the hammer");
}
```
### If...Else Statements
**If...else statements** allow you to execute certain pieces of code based on a condition, or set of conditions, being met.
```js
if (/* this expression is true */) {
  // run this code
} else {
  // run this code
}
```
This is extremely helpful because it allows you to choose which piece of code you want to run based on the result of an expression. For example:
```js
var a = 1;
var b = 2;

if (a > b) {
  console.log("a is greater than b");
} else {
  console.log("a is less than or equal to b");
}
```
**Prints:** "a is less than or equal to b"

A couple of important things to notice about `if...else` statements.

The value inside the `if` statement is always *converted* to true or false. Depending on the value, the code inside the `if` statement is run or the code inside the `else` statement is run, but not both. The code inside the `if` and `else` statements are surrounded by **curly braces** `{...}` to separate the conditions and indicate which code should be run.

**TIP:** When coding, sometimes you may only want to use an `if` statement. However, if you try to use only an `else` statement, then you will receive the error `SyntaxError: Unexpected token else`. You’ll see this error because `else` statements need an `if` statement in order to work. You can’t have an `else` statement without first having an `if` statement.

### Else If Statements
In some situations, two conditionals aren’t enough. Consider the following situation.

You're trying to decide what to wear tomorrow. If it is going to snow, then you’ll want to wear a coat. If it's not going to snow and it's going to rain, then you’ll want to wear a jacket. And if it's not going to snow or rain, then you’ll just wear what you have on.

![Flowchart 3](img/what-to-wear-cropped.jpg)

In JavaScript, you can represent this secondary check by using an extra if statement called an **else if statement**.
```js
var weather = "sunny";

if (weather === "snow") {
  console.log("Bring a coat.");
} else if (weather === "rain") {
  console.log("Bring a rain jacket.");
} else {
  console.log("Wear what you have on.");
}
```
**Prints:** Wear what you have on.

By adding the extra `else if` statement, you're adding an extra conditional statement.

If it’s not going to snow, then the code will jump to the `else if` statement to see if it’s going to rain. If it’s not going to rain, then the code will jump to the `else` statement.

The `else` statement essentially acts as the "default" condition in case all the other `if` statements are false.

QUESTION 1 OF 2

What will be printed to the console if the following code is run?
```js
var money = 100.50;
var price = 100.50;

if (money > price) {
  console.log("You paid extra, here's your change.");
} else if (money === price) {
  console.log("You paid the exact amount, have a nice day!");
} else {
  console.log("That's not enough, you still owe me money.");
}
```
**Answer:** "You paid the exact amount, have a nice day!"

QUESTION 2 OF 2

Looking at the following code, determine what medal Kendyll received.
```js
var runner = "Kendyll";
var position = 2;
var medal;

if(position === 1) {
  medal = "gold";
} else if(position === 2) {
  medal = "silver";
} else if(position === 3) {
  medal = "bronze";
} else {
  medal = "pat on the back";
}

console.log(runner + " received a " + medal + " medal.");
```
**Answer:** Kendyll received a silver medal.

### Quiz: Even or Odd (3-2)
#### Directions:
Write an if...else statement that:
- prints `"even"` if the number is an even number
- prints `"odd"` if the number is an odd number

**Hint:** Use the `%` ([modulo](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Remainder_())) operator to determine if a number is even or odd. The modulo operater takes two numbers and returns the remainder when the first number is divided by the second one:
```js
console.log(12 % 3);
console.log(10 % 4);
```
**Result:**

0

2

The answer for `12 % 3` is `0` because twelve divided by three has no remainder. `10 % 4` is `2` because ten divided by 4 has a remainder of two.

Make sure to test your code with different values. For example:
- If `number` equals `1`, then `odd` should be printed to the console.
- If `number` equals `12`, then `even` should be printed to the console.

**Your Code:**
```js
/*
 * Programming Quiz: Even or Odd (3-2)
 *
 * Write an if...else statement that prints `even` if the 
 * number is even and prints `odd` if the number is odd.
 *
 * Note - make sure to print only the string "even" or the string "odd"
 */

// change the value of `number` to test your if...else statement
var number = 2;

if (number % 2 === 0) {
    console.log("even");
} else {
    console.log("odd");
}
```
### Quiz: Musical Groups (3-3)
Musical groups have special names based on the number of people in the group.

For example, a "quartet" is a musical group with four musicians. [Barbershop quartets](https://en.wikipedia.org/wiki/Barbershop_quartet) were a popular type of quartet in the early 1900s and featured four singers made up of a lead, tenor, baritone, and bass.

#### Directions:
Write a series of conditional statements that:
- Prints `"not a group"` if `musicians` is less than or equal to `0`
- Prints `"solo"` if `musicians` is equal to `1`
- Prints `"duet"` if `musicians` is equal to `2`
- Prints `"trio"` if `musicians` is equal to `3`
- Prints `"quartet"` if `musicians` is equal to `4`
- Prints `"this is a large group"` if `musicians` is greater than `4`

**TIP:** Test your code with different values. For example:

If `musicians` equals `3`, then `"trio"` should be printed to the console.

If `musicians` equals `20`, then `"this is a large group"` should be printed to the console.

If `musicians` equals `-1`, then `"not a group"` should be printed to the console.

Be sure to watch out for any extra or missing characters (including spaces or punctuation marks) in your output string as well!

**Your Code:**
```js
/*
 * Programming Quiz: Musical Groups (3-3)
 */

// change the value of `musicians` to test your conditional statements
var musicians = 5;

if (musicians == 1) {
    console.log("solo");
} else if (musicians == 2) {
    console.log("duet");
} else if (musicians == 3) {
    console.log("trio");
} else if (musicians == 4) {
    console.log("quartet");
} else if (musicians > 4) {
    console.log("this is a large group");
} else {
    console.log("not a group");
}
```
### Quiz: Murder Mystery (3-4)
#### Directions:
For this quiz, you're going to help solve a fictitious murder mystery that happened here at Udacity! A [murder mystery](https://en.wikipedia.org/wiki/Murder_mystery_game) is a game typically played at parties wherein one of the partygoers is secretly, and unknowingly, playing a murderer, and the other attendees must determine who among them is the criminal. It's a classic case of [whodunnit](https://en.wikipedia.org/wiki/Whodunit).

Since this might be your first time playing a murder mystery, we've simplified things quite a bit to make it easier. Here's what we know! In this murder mystery there are:
- **four rooms:** the ballroom, gallery, billiards room, and dining room,
- **four weapons:** poison, a trophy, a pool stick, and a knife,
- and **four suspects:** Mr. Parkes, Ms. Van Cleve, Mrs. Sparr, and Mr. Kalehoff.

We also know that each weapon corresponds to a particular room, so...
- the `poison` belongs to the `ballroom`,
- the `trophy` belongs to the `gallery`,
- the `pool stick` belongs to the `billiards room`,
- and the `knife` belongs to the `dining room`.

And we know that each suspect was located in a specific room at the time of the murder.
- `Mr. Parkes` was located in the `dining room`.
- `Ms. Van Cleve` was located in the `gallery`.
- `Mrs. Sparr` was located in the `billiards room`.
- `Mr. Kalehoff` was located in the `ballroom`.

To help solve this mystery, write a combination of conditional statements that:
1. sets the value of `weapon` based on the `room` and
2. sets the value of `solved` to `true` if the value of `room` matches the `suspect's` room

Afterwards, use this template to print a message to the console if the mystery was solved:
```js
__________ did it in the __________ with the __________!
```
What goes into the three blank spaces? You can fill in the blanks with the name of the suspect, the room, and the weapon! For example, an output string may look like:
```js
Mr. Parkes did it in the dining room with the knife!
```
Be sure to watch out for any extra or missing characters (including spaces and punctuation marks) in your output string as well!

**TIP:** Test your code with different values. For example:

If `room` equals `gallery` and `suspect` equals `Ms. Van Cleve`, then `Ms. Van Cleve did it in the gallery with the trophy`! should be printed to the console.

**Your Code:**
```js
/*
 * Programming Quiz: Murder Mystery (3-4)
 */

// change the value of `room` and `suspect` to test your code
var room = "dining room";
var suspect = "Mr. Parkes";

var weapon = "";
var solved = false;

if (room === "ballroom" && suspect === "Mr. Kalehoff") {

    weapon = "poison";
    solved = "true";

} else if (room === "gallery" && suspect === "Ms. Van Cleve") {

    weapon = "trophy";
    solved = "true";

} else if (room === "billiards room" && suspect === "Mrs. Sparr") {
    weapon = "pool stick";
    solved = "true";
} else if (room === "dining room" && suspect === "Mr. Parkes") {
    weapon = "knife";
    solved = "true";
}

if (solved) {
    console.log(suspect + " did it in the " + room + " with the " + weapon + "!");
}
```
### More Complex Problems
Sometimes problems are not always as simple as buying something from the store, in fact, most problems are a lot more complex. With most problems, there’s more things to consider before you can actually solve the problem. For example, me deciding what I want to do this weekend. What were you planning on doing this weekend? Well, I was thinking I would hang out with my friend Colt. And if he’s not busy and the weather is nice so I was thinking we could go to the park. That sounds like fun. I think, this is the perfect time for us to transition into more complex logical expressions. It is? Well yeah, think about it. For your plans to happen, there are two conditions that need to be true. Colt has not to be busy and the weather needs to be nice. If both of these things happen, then, you and Colt are going to the park. Okay, I see where you’re going. In JavaScript, we can represent more complex problems by combining logical expressions with special operators called logical operators. Check it out.

### Logical Operators
Here’s the logical expression used to represent Julia’s weekend plans:
```js
var colt = "not busy";
var weather = "nice";

if (colt === "not busy" && weather === "nice") {
  console.log("go to the park");
}
```
**Prints:** "go to the park"

Notice the `&&` in the code above.

The `&&` symbol is the logical AND operator, and it is used to combine two logical expressions into one larger logical expression. If **both** smaller expressions are *true*, then the entire expression evaluates to *true*. If **either one** of the smaller expressions is *false*, then the whole logical expression is *false*.

Another way to think about it is when the `&&` operator is placed between the two statements, the code literally reads, "if Colt is not busy *AND* the weather is nice, then go to the park".

#### Logical expressions
**Logical expressions** are similar to mathematical expressions, except logical expressions evaluate to either *true* or *false*.
```js
11 != 12
```
**Returns:** true

You’ve already seen logical expressions when you write comparisons. A comparison is just a simple logical expression.

Similar to mathematical expressions that use `+`, `-`, `*`, `/` and `%`, there are logical operators `&&`, `||` and `!` that you can use to create more complex logical expressions.

#### Logical operators
**Logical operators** can be used in conjunction with boolean values (`true` and `false`) to create complex logical expressions.

By combining two boolean values together with a logical operator, you create a *logical expression* that returns another boolean value. Here’s a table describing the different logical operators:

| Operator | Meaning | Example | How it works |
| --- | --- | --- | --- |
| `&&`| Logical<br/>AND | `value1 &&<br/>value2`| Returns `true` if **both** `value1` **and** `value2` evaluate<br/>to `true`. |
| `\|\|\` | Logical<br/>OR | `value1 \|\|\<br/>value2` | Returns `true` if **either** `value1` **or** `value2` (**or even<br/>both!**) evaluates to `true`. |
| `!`| Logical<br/>NOT | !value1 | Returns the **opposite** of `value1`. If `value1` is `true`,<br/>then `!value1` is `false`.

By using logical operators, you can create more complex conditionals like Julia’s weekend example. Instead of:
```js
var colt = "not busy";
var weather = "nice";

if (colt === "not busy") {
   if (weather === "nice") {
      console.log("go to the park");
   }
}
```
You can do:
```js
var colt = "not busy";
var weather = "nice";

if (colt === "not busy" && weather === "nice") {
   console.log("go to the park");
}
```
**TIP:** Logical expressions are evaluated from left to right. Similar to mathematical expressions, logical expressions can also use parentheses to signify parts of the expression that should be evaluated first.

QUESTION 1 OF 3

What value of [BLANK] would make the following expression evaluate to `false`. Notice the `!` right at the beginning!
```js
!([BLANK] === 4) && "STRing" === "STRing"
```
**Returns:** false

**Answer:** 4

QUESTION 2 OF 3

Select the operator that would make the following expression evaluate to true.
```js
3 < -10 [BLANK] "James" !== "james"
```
**Returns:** true

**Answer:** ||

QUESTION 3 OF 3

Evaluate the following logical expressions. Check the ones that evaluate to `true`.
```js
true || false // true
false && false // false
!true // false
(13 > -7) || (false == 0) // true
(10 === "10") && (1 <= 2) // false
(3 != 6 % 3) && !(24 > 45) && (!false) // true
```

### Logical AND and OR
### Quiz: Checking your Balance (3-5)
### Quiz: Ice Cream (3-6)
### Quiz: What do I Wear? (3-7)
### Advanced Conditionals
### Truthy and Falsy
### Ternary Operator
### Quiz: Navigating the Food Chain (3-8)
### Switch Statement
### Falling-through
### Quiz: Back to School (3-9)
### Lesson 3 Summary
## Loops
## Functions
## Arrays
## Objects
