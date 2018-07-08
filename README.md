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
JavaScript is a programming language for the web and is the the final piece needed to make your websites come to life. It was created by Brendan Eich in 1995 to make it easier to add interactive and dynamic elements to websites. Today, the language is used for all sorts of applications, from programming a robot with an Arduino to writing a game script in Unity or even building a code editor. The opportunities with JavaScript truly are endless.

### History of JavaScript
JavaScript was created in just 10 days by Brendan Eich back in 1995, while Eich was working on Netscape Navigator. Netscape Navigator was one of the Internet’s first web browsers. Nowadays, Google Chrome, Mozilla Firefox, Apple Safari, and Microsoft Edge are used to surf the web. Prior to Eich’s creation of JavaScript, websites just existed as pages of HTML and CSS with the occasional plug-in or Java applet (Java is not related to JavaScript in any way). JavaScript was originally called LiveScript, but it was changed to JavaScript as a marketing decision in order to cash in on the popularity of Java at the time. As the language evolved, competing versions of the language emerged, so JavaScript was eventually taken to Ecma International so that an official standard could be formed. Today, the language itself is still referred to as JavaScript, however, recent versions are referenced by their ECMAScript version number, such as, ES5 or ES6. Even more recently, the standards body has transitioned to a year-based number to promote a more consistent release cycle. So we now have ES2016, ES2017, etc. All things considered, JavaScript has grown to be one of the most popular languages in the world and is considered one of the three foundational pillars of front end web development.

**Note:**
- HTML and CSS are markup languages. Markup languages are used to describe and define elements within a document. 
- JavaScript is a programming language. Programming languages can be used to control the behavior of a machine and to express algorithms.

### The JavaScript Console

In Google Chrome, you can access the console by opening the developer tools, which can be done by right clicking the page and selecting inspect. Once open, navigate to the console tab. Alternatively, the keyboard shortcut is Cmd+Option+J on a Mac or Ctrl+Shift+J on Windows. For more Chrome developer tools keyboard shortcuts, [click here](https://developers.google.com/web/tools/chrome-devtools/shortcuts).

You can write and test JavaScript code directly in the console. For example, to write your first line of code you could start by writing your name. As you will see, just writing your name will actually result in an error. To be able to actually write your name in JavaScript without an error you need to format your name as a data type called a string put inside quotes. 

Why don’t we try something else? Here’s some code that creates an alert that says, Hello, Julia, how are you? And it pushes it to the browser. Now writing code directly in your browser is something you can do to test out new code snippets where you’re not really sure what they do. But it could actually get pretty annoying once you start writing larger and larger programs. For example, if you wanted to create two alerts instead of just one, it may seem simple at first, but each time you need to go to the next line, you would have to type Shift+Return instead of just the Return key. This is going to get pretty annoying pretty fast. Eventually, you’ll learn about other ways to run JavaScript files. But for now we recommend using a text editor like Atom or Sublime Text and then pasting your code in the console once you’re ready to test it.

### Developer Tools on Different Browsers
Every modern web browser includes its own set of developer tools. Below is a guide to the various web browsers and their respective developer tools.

Instructions
- [Google Chrome](#google-chrome)
- [Mozilla Firefox](#mozilla-firefox)
- [Internet Explorer](#internet-explorer)
- [Microsoft Edge](#microsoft-edge)
- [Safari](#safari)
- [Opera](#opera)

#### Google Chrome
The Chrome DevTools are a set of web authoring and debugging tools built into Google Chrome. Use the DevTools to iterate, debug and profile your site. To learn more, [click here](https://developers.google.com/web/tools/chrome-devtools/).

To open Chrome DevTools, either right-click on any page element and select Inspect or open the Chrome settings menu in the top-right corner of your browser window and select More Tools > Developer Tools. Alternatively, you can use the shortcuts:
- Command + Option + i (Mac)
- Ctrl + Shift + i (Windows/Linux).

#### Mozilla Firefox
Firefox Developer Tools allow you to examine, edit, and debug HTML, CSS, and JavaScript on the desktop and on mobile. Also, you can download a version of of Firefox called Firefox Developer Edition that is tailored for developers, featuring the latest Firefox features and experimental developer tools. To learn more, [click here](https://developer.mozilla.org/en-US/docs/Tools).

To open Firefox Developer Tools, either right-click on any page element and select Inspect Element or open the Firefox settings menu in the top-right corner of your browser window and select Developer. Alternatively, you can use the shortcuts:
- Command + Option + i (Mac)
- Ctrl + Shift + i (Windows/Linux).

#### Internet Explorer
If you use Internet Explorer, then you can access F12 developer tools by simply pressing F12. The features vary between versions, but starting at Internet Explorer 8 remain pretty consistent. Below, we've linked to documentation for each version, but if you've upgraded to Microsoft Edge, then check the next section.
- [Internet Explorer 8](https://msdn.microsoft.com/en-us/library/dd565628.aspx)
- [Internet Explorer 9](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/samples/gg589512(v=vs.85))
- [Internet Explorer 10](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/dev-guides/hh673549(v=vs.85))
- [Internet Explorer 11](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/dev-guides/bg182636(v=vs.85))

#### Microsoft Edge
Microsoft Edge introduces great new improvements to the F12 developer tools seen in Internet Explorer. The new tools are built in TypeScript, and are always running, so no reloads are required. In addition, F12 developer tools documentation is now fully available on [GitHub](https://github.com/MicrosoftDocs/edge-developer).

Just like Internet Explorer, to open developer tools in Microsoft Edge simply press F12.

To learn more, [click here](https://docs.microsoft.com/de-de/microsoft-edge/devtools-guide).

#### Safari
For any Mac users, Safari includes Web Inspector, a powerful tool that makes it easy to modify, debug, and optimize a website for peak performance and compatibility on both platforms. To learn more, [click here](https://developer.apple.com/safari/tools/).

To access Safari's Web Development Tools, enable the Develop menu in Safari’s Advanced preferences. Once enabled, you can right-click on any page element and select Inspect Element to open Web Development Tools or use the shortcut Command + Option + i.

#### Opera
Fast, lean and powerful, Opera comes pre-packed with a fully-featured suite of developer tools. Named Opera Dragonfly, it is designed to make your job easier. To learn more, [click here](https://www.opera.com/dragonfly/).

Launch Opera Dragonfly with the following keyboard shortcuts:
- Command + Option + i (Mac)
- Ctrl + Shift + i (Windows/Linux).

Alternatively, you can target a specific element by right-clicking in the page and selecting Inspect Element.

### Console Log
Developer tools allow you to debug and test out your ideas directly in the browser. If your familiar with HTML or CSS, you may have used developer tools to experiment with the style of a webpage. But you can also use it with JavaScript. Developer tools are often used as a sandbox. In other words, a place to mess around with any code without any long-term consequences. You can use developer tools to debug problems you run in to or to test a piece of code you’ve just learned. If you open any website that uses JavaScript, the console will tell you if there are any warnings or errors on the page and will also display any output and print it with console.log. Note that anytime you’re using the console on this course, you might see some errors or warnings from the site you’re visiting. That’s okay, this is very common and will not affect the code that you write in this course.

console.log is used to display content to the JavaScript console. Run the following code in the console:
```
console.log("hiya friend!");
```
**Prints:** "hiya friend!"

Congratulations! You performed the log action on the debugging console.

The message you’ve logged is "hiya friend!". hiya friend! is a string (a sequence of characters).

#### Optional demo example
Let’s use console.log to do something a little more interesting. Here’s a block of JavaScript code that loops through the numbers 0 through 9 and prints them out to the console:
```
for (var i = 0; i < 10; i++) {
  console.log(i);
}
```
**Prints**

0

1

2

3

4

5

6

7

8

9

This is called a loop.
### JavaScript Demo

### Summary

## Data Types and Variables
### Introduction to Data Types

### Numbers

### Comments

### Quiz: First Expression (2-1)

### Strings

### String Concatination

### Variables

### Quiz: Converting Temperatures (2-2)

## Conditionals
## Loops
## Functions
## Arrays
## Objects
