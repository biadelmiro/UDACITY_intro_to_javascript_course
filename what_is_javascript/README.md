# What is JavaScript?

1. [Introduction to JavaScript](#introduction-to-javascript)
2. [History of JavaScript](#history-of-javascript)
3. [Developer Tools and the JavaScript Console](#developer-tools-and-the-javascript-console)
4. [The JavaScript Console](#the-javascript-console)
5. [Console Log](#console-log)
6. [JavaScript Demo](#javascript-demo)
7. [Summary](#summary)

## Introduction to JavaScript
JavaScript is a programming language for the web and is the the final piece needed to make your websites come to life. The language was created to make it easier to add interactive and dynamic elements to websites, however, it can also be used to program a robot, write a game script or build a code editor. Since it's conception, JavaScript has grown to be one of the most popular languages in the world.

## History of JavaScript
JavaScript was created in just 10 days by Brendan Eich back in 1995. Prior to JavaScript, websites existed as pages of HTML and CSS with the occasional plug-in or Java applet. Originally called LiveScript, JavaScript changed it's name due to Java's popularity at the time. As the language grew, competing versions emerged which was when it was taken to Ecma International to be standardized. Recent versions can be referenced by their version number, such as, ES5 or ES6 and even more recent versions now use a year-based number to promote a more consistent release cycle with ES2016, ES2017, etc.

## Developer Tools and the JavaScript Console
### Developer Tools
Every modern web browser includes its own set of developer tools that are often used as a sandbox you can mess around in without any consequences. The console informs you of any warnings or errors written in JavaScript as well as prints any output with console.log. Note, warnings and errors are very common when visiting sites and will not affect your code. The main browsers used today are; Google Chrome, Mozilla Firefox, Opera, Safari, Microsoft Edge and Internet Explorer 8 to 11. You can generally access the developer tools with a right-click on the page and then selecting Inspect Element. Alternatively, you can use the shortcuts; Command + Option + i (Mac) or Ctrl + Shift + i (Windows). With Safari you need to first enable them in the Advanced Preferences and with Windows you can just press the F12 key on the keyboard.

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
- [Microsoft Edge on GitHub](https://github.com/MicrosoftDocs/edge-developer)

### The JavaScript Console
You can access the console by either using the instructions or shortcuts previously mentioned in the Developer Tools and navigating to the console tab. Alternatively, if using Chrome, you can use the shortcut Cmd+Option+J (Mac) or Ctrl+Shift+J (Windows). You can write and test JavaScript code directly in the console. For more Chrome developer tools keyboard shortcuts [click here](https://developers.google.com/web/tools/chrome-devtools/shortcuts).

### Examples
Type the following into the console to test and see what happens:

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

## Console Log
console.log is used to print content to the JavaScript console. In the following example, the **string** data type is used

### Example
Here you will see the difference between simply writing a string and printing a string with console.log:

```js
console.log("hiya friend!");
```

### Optional demo example
console.log can also be used inside of a loop. Here is a **loop** that loops through from 0 to 9 and prints them to the console:

```js
for (var i = 0; i < 10; i++) {
  console.log(i);
}
```
**Prints:** 0 1 2 3 4 5 6 7 8 9

Based on this loop's settings you will see that any code written inside the curly brackets {...} will be repeated 10 times and console.log prints out the value of i each time the loop runs. Don't about what the syntax means for now - you'll learn more about how and when to use loops later.

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
- All major browsers come with built-in JavaScript engines
- This allows browsers to run and execute JavaScript code
- Next, you got practice using the JavaScript console
- The JavaScript console allows you to print strings and execute lines of JavaScript code on the fly, right inside of your browser
- And finally, you wrapped up with some exercises where you use JavaScript to add styles and animations to a web page.
