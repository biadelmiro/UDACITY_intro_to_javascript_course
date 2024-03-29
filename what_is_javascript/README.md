# What is JavaScript?

1. [Introduction to JavaScript](#introduction-to-javascript)
2. [History of JavaScript](#history-of-javascript)
3. [The JavaScript Console](#the-javascript-console)
4. [Developer Tools on Different Browsers](#developer-tools-on-different-browsers)
5. [Console Log](#console-log)
6. [JavaScript Demo](#javascript-demo)
7. [Summary](#summary)

## Introduction to JavaScript
- JavaScript is a programming language for the web.
- It is the final piece needed to make your websites come to life.
- The language was created to make it easier to add interactive and dynamic elements to websites.
- Today it can also be used to program a robot, write a game script or build a code editor.
- Since it's conception, JavaScript has grown to be one of the most popular languages in the world.

## History of JavaScript
- JavaScript was created in just 10 days by Brendan at Netscape back in 1995.
- Prior to JavaScript, websites existed as pages of HTML and CSS with the occasional plug-in or Java applet.
- Originally called LiveScript, JavaScript changed it's name due to Java's popularity at the time.
- As the language grew, competing versions emerged which was when it was taken to Ecma International to be standardized.
- Recent versions are referenced by their version number, such as, ES5 or ES6 and even more recent versions now use a year-based number to promote a more consistent release cycle with ES2016, ES2017, etc.

## The JavaScript Console
- With Chrome, you can use the shortcut Cmd+Option+J (Mac) or Ctrl+Shift+J (Windows) to directly access the JavaScript Console.
- Alternatively, you can use the shortcut Cmd+Option+I (Mac) or Ctrl+Shift+I (Windows) to access the Developer Tools panel and navigate to the JavaScript Console.

Type the following into the console and see what happens:

```js 
"Your Name"
```

```js
alert("Hi there! How are you?!");
```

```js
alert("Hello");
alert(":(");
```

```js
alert("Hello");
alert("This is great!");
alert("JavaScript is fun!");
```


## Developer Tools on Different Browsers
- Every modern web browser has a built-in JavaScript engine and includes its own set of Developer Tools.
- Developer Tools are used as a sandbox to test code without any consequences.
- The Console informs you of any warnings or errors and prints any output with console.log (warnings and errors are very common). 
- The main browsers used today are; Google Chrome, Mozilla Firefox, Opera, Safari, Microsoft Edge and Internet Explorer 8 to 11.
- You can use the shortcuts; Cmd+Option+I (Mac) or Ctrl+Shift+I (Windows).
- With Safari you need to first enable the Developer Tools in the Advanced Preferences.
- With Windows you can simply press the F12 key on the keyboard.

## Console Log
console.log is used to print content to the JavaScript console.

In the following example, the **string** data type is used where you will see the difference between simply writing a string and printing a string with console.log:

```js
"hiya friend!"
```

```js
console.log("hiya friend!");
```

### Optional demo example
console.log can also be used inside of a loop.

Here is a **loop** that loops through from 0 to 9 and prints them to the console:

```js
for (var i = 0; i < 10; i++) {
  console.log(i);
}
```
**Prints:** 0 1 2 3 4 5 6 7 8 9

Based on this loop's settings you will see that any code written inside the curly brackets {...} which will be repeated 10 times and console.log prints out the value of i each time the loop runs. You'll learn more about how and when to use loops later.

## JavaScript Demo
So you saw how to use console.log to print a message to the JavaScript console. Now, let’s see how you can use the console as a sandbox to test a new line of JavaScript in the browser

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
- All major browsers come with built-in JavaScript engines allowing browsers to run and execute JavaScript code.
- The JavaScript console allows you to print strings and execute lines of JavaScript code right inside of your browser.
- The exercises highlight some of the possibilities that JavaScript can do with added styles and animations to a web page.
