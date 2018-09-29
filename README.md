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
   7. [Summary](#summary)
2. [Data Types and Variables](#data-types-and-variables)
   1. [Introduction to Data Types](#introduction-to-data-types)
   2. [Numbers](#numbers)
   3. [Comments](#comments)
   4. [Quiz: First Expression (2-1)](#quiz-first-expression-2-1)
   5. [Strings](#strings)
   6. [String Concatination](#string-concatination)
   7. [Variables](#variables)
   8. [Quiz: Converting Temperatures (2-2)](#quiz-converting-temperatures-2-2)
3. [Conditionals](#conditionals)
4. [Loops](#loops)
5. [Functions](#functions)
6. [Arrays](#arrays)
7. [Objects](#objects)

## What is JavaScript?
### Introduction to JavaScript
JavaScript is a programming language for the web and is the the final piece needed to make your websites come to life. It was created to make it easier to add interactive and dynamic elements to websites. Today, the language is used for all sorts of applications, from programming a robot with an Arduino to writing a game script in Unity or even building a code editor. It has grown to be one of the most popular languages in the world and is considered one of the three foundational pillars of front end web development.

### History of JavaScript
JavaScript was created in just 10 days by Brendan Eich back in 1995 while he was working on Netscape Navigator which was one of the Internet’s first web browsers. Nowadays, mostly Google Chrome, Mozilla Firefox, Apple Safari, and Microsoft Edge are used to surf the web. Prior to Eich’s creation of JavaScript, websites just existed as pages of HTML and CSS with the occasional plug-in or Java applet. JavaScript was originally called LiveScript, but was changed to JavaScript as a marketing decision in order to ride on the coattails of Java's popularity at the time. As the language evolved, competing versions of the language emerged. So JavaScript was eventually taken to Ecma International to be standardized. Today, the language itself is still referred to as JavaScript, however, recent versions are referenced by their ECMAScript version number, such as, ES5 or ES6. Even more recently, the standards body has transitioned to a year-based number to promote a more consistent release cycle with ES2016, ES2017, etc.

### The JavaScript Console

In Google Chrome, you can access the console by opening the developer tools, which can be done by right clicking the page and selecting inspect. Once open, navigate to the console tab. Alternatively, the keyboard shortcut is Cmd+Option+J on a Mac or Ctrl+Shift+J on Windows. For more Chrome developer tools keyboard shortcuts, [click here](https://developers.google.com/web/tools/chrome-devtools/shortcuts).

You can write and test JavaScript code directly in the console. For example, to write your first line of code you could start by writing your name. As you will see, just writing your name will actually result in an error. To be able to actually write your name in JavaScript without an error you need to format your name as a data type called a string put inside quotes:
``` 
"Michael"
```
Why don’t we try something else? Here’s some code that creates an alert that says, Hello, Julia, how are you? And it pushes it to the browser:
```
alert("Hello, Michael! How are you?!");
```
Now writing code directly in your browser is something you can do to test out new code snippets where you’re not really sure what they do. But it could actually get pretty annoying once you start writing larger and larger programs. For example, if you wanted to create more than just one alert, it may seem simple at first, but each time you need to go to the next line, you would have to type Shift+Return instead of just the Return key.
```
alert("Hello");
alert(":(");
```
```
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
```
console.log("hiya friend!");
```
**Prints:** "hiya friend!"

The message logged is a data type called a **string** (a sequence of characters).

#### Optional demo example
Let’s use console.log to do something a little more interesting. Here’s a block of JavaScript code that loops through the numbers 0 through 9 and prints them out to the console:
```
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
```
document.getElementsByTagName("h1")[0].style.color = "#ff0000";
```
As you can see, the heading changed red. Styling elements on the page is great, but you could also do that by just modifying the CSS. What makes JavaScript so special in this case? Refresh the page, then paste this line of code in the JavaScript console.
```
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
```
3
```
**Returns:** 3

There, you did it.

#### Arithmetic operations
You can also perform calculations with numbers pretty easily. Basically type out an expression the way you would type it in a calculator:
```
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
```
5 > 10
```
**Returns:** false

### Comments
You can use comments to help explain your code and make things clearer. In JavaScript, comments are marked with a double forward-slash //. Anything written on the same line after the // will not be executed or displayed. To have the comment span multiple lines, mark the start of your comment with a forward-slash and star, and then enclose your comment inside a star and forward-slash /* … */.
```
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
```
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

**Tip:** It is correct to either use “ or ‘ quotes with strings, as long as you’re consistent. The [JavaScript Udacity style guide](http://udacity.github.io/frontend-nanodegree-styleguide/javascript.html) for labs and projects suggests using single quotes to define string literals.

### String Concatination
**Strings** are a collection of characters enclosed inside double or single quotes. You can use strings to represent data like sentences, names, addresses, and more. Did you know you can even add strings together? In JavaScript, this is called **concatenating**. Concatenating two strings together is actually pretty simple!
```
"Hello," + " New York City"
```
**Returns:** "Hello, New York City"

You will see other ways to concatenate and do even more with strings later in this course. But for now, practice using the addition + operator.
### Variables

### Quiz: Converting Temperatures (2-2)

## Conditionals
## Loops
## Functions
## Arrays
## Objects
