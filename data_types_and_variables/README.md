# Data Types and Variables

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

## Data Types and Variables
### Introduction to Data Types
- Data is everywhere. It helps us understand the world, recognize trends, make educated guesses and inform our future decisions.
- This is no different in programming. Data and data types are the building blocks of any programming language, because they help us organize information and determine how our programs will run. 
- When you look on your Facebook profile, what do you see? Your name, the number of friends you have, the date of your last post, a list of status updates and whether you liked the comment your friend just made. 
- All this information is being gathered, calculated and presented to your friends and family visiting your profile. 
- And when you look at your bank account, what do you see?
- An account number, an account balance, dates of each transaction and the name of the company that you made a purchase from.
- It’s important to be aware of what types of data you’re using and when it’s appropriate to use each type. In this lesson, we’ll start by learning how to define and manipulate the primitive data types of JavaScript. 
- Numbers, strings, Booleans, undefined and null. 
- Once you’re familiar with these data types, you’ll see how you can store data into variables so you can reuse and manipulate data throughout your code.

## Numbers
- Defining a number in JavaScript is actually pretty simple.
- The **Number** data type includes any positive or negative integer, as well as decimals. 
- Entering a number into the console will return it right back to you:
```js
3
```
**Returns:** 3

There, you did it.

### Arithmetic operations
- You can also perform calculations with numbers pretty easily.
- Basically type out an expression the way you would type it in a calculator:
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

### Comparing numbers
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

## Comments
- You can use comments to help explain your code and make things clearer.
- In JavaScript, comments are marked with a double forward-slash //. 
- Anything written on the same line after the // will not be executed or displayed. To have the comment span multiple lines, mark the start of your comment with a forward-slash and star, and then enclose your comment inside a star and forward-slash /* … */.
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

## Quiz: First Expression (2-1)
### Directions:
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

## Strings
- Let’s take a look at the string datatype. 
- You’ve actually used a string before, and maybe just didn’t know it. 
- When you type a message inside console.log, that message is actually just a JavaScript string. 
- So here, Hiya, Friend, is just a string. 
- Strings can be single letters, like the character h, or even contain numbers, like the string 123. 
- The important thing is that you use quotes to signify a string. 
- It doesn’t matter if the quotes are single or double quotes, but they do have to match. 
- I used double quotes here and single quotes here. 
- If I try to pass the string to the console.log but forget to use the quotes, JavaScript will return back an error. 
- I get this reference error, because the JavaScript engine thinks I’m talking about a variable called hello instead of a string with the value of hello. 
- We haven’t talked about variables just yet, but the moral of the story here is to remember to use quotes when using strings.
- If I add the quotes in, then the string gets printed out to the console.

**TIP:** It is correct to either use “ or ‘ quotes with strings, as long as you’re consistent. The [JavaScript Udacity style guide](http://udacity.github.io/frontend-nanodegree-styleguide/javascript.html) for labs and projects suggests using single quotes to define string literals.

## String Concatination
- **Strings** are a collection of characters enclosed inside double or single quotes. 
- You can use strings to represent data like sentences, names, addresses, and more. 
- Did you know you can even add strings together? In JavaScript, this is called **concatenating**. 
- Concatenating two strings together is actually pretty simple!
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

## Variables
- So you have all these numbers, strings and booleans, but what are you supposed to do with them? 
- All this data so far has been for a one time use only. You define the string, Hello, it’s returned and that’s it. 
- That’s the end. 
- The string Hello is now gone. 
- You need a way to be able to store data, so that you can use it or change it later. 
- To do this you can use variables. 
- You’ve probably heard of variables before, maybe in a math class. 
- Let’s say you have a variable called X, and it’s assigned the value 5. 
- And then let’s say we have the expression X + 1. 
- Since X has the value of 5, we can substitute the value of 5 in for X. 
- So the expression becomes 5 + 1 = 6. 
- In JavaScript, variable stored data, much like how the variable you just saw stored the value of 5. 
- And they’re not limited to the storing of just numerical values, you can store any variable in to a variable. 
- To create a variable, use the var keyword followed by the variableName, and the assignment operator. 
- The assignment operator is the equal sign. 
- And then on the right side of the assignment operator, put the value you want to assign to the variable. As an example, here’s my cat Zoe. We can use a variable called name and set it equal to the string Zoe for her name. And for her age, we can create a variable called age, and set that to the number 4, since Zoe’s 4 years old. Eventually, when Zoe has her next birthday, I’ll be able to use the age variable I created to increment Zoe’s age by 1, so the variable age will return Zoe’s updated age of 5. Now, Zoe’s 5 years old.

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

### Naming Conventions
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

## String Index
### Indexing
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

## Escaping Strings
### Escaping strings
There are some cases where you might want to create a string that contains more than just numbers and letters. For example, what if you want to use quotes in a string?
```js
"The man whispered, "please speak to me.""
```
**Uncaught SyntaxError:** Unexpected identifier
If you try to use quotes within a string, you will receive a ```SyntaxError``` like the one above.

- Because you need to use quotes to denote the beginning and end of strings, the JavaScript engine misinterprets the meaning of your string by thinking ```"The man whispered, "``` is the string. Then, it sees the remaining ```please speak to me.""``` and returns a ```SyntaxError```.

If you want to use quotes *inside a string*, and have JavaScript not misunderstand your intentions, you’ll need a different way to write quotes. Thankfully, JavaScript has a way to do this using the backslash character ( \ ).

If you forget to use the backslash to escape characters, then the JavaScript engine can misinterpret your strings.

### Escaping characters
In JavaScript, you use the backslash to **escape** other characters.

*Escaping a character* tells JavaScript to ignore the character's special meaning and just use the literal value of the character. This is helpful for characters that have special meanings like in our previous example with quotes ```"…"```.

Because quotes are used to signify the beginning and end of a string, you can use the backslash character to escape the quotes in order to access the literal quote character.
```js
"The man whispered, \"please speak to me.\""
```
**Returns:** The man whispered, "please speak to me."

This guarantees that the JavaScript engine doesn’t misinterpret the string and result in an error.

By using the backslash to escape characters, the JavaScript engine can understand the meaning of your strings.

### Special characters
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

## Comparing Strings
### Comparing strings
Another way to work with strings is by comparing them. You've seen the comparison operators ```==``` and ```!=``` when you compared numbers for equality. You can also use them with strings! For example, let’s compare the string ```"Yes"``` to ```"yes"```.
```js
"Yes" == "yes"
```
**Returns:** false

When you run this in the console, it returns false. Why is that? ```"Yes"``` and ```"yes"``` are the same string, right? Well not quite.

#### Case-sensitive
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

## Quiz: Favorite Foods (2-3)
### Directions:
Create a string with the name of your favorite food. The first letter of the string should be capitalized.

**Your Code:**
```js
/*
 * Programming Quiz: Favorite Food (2-3)
 */

console.log("Pizza");
```

## Quiz: String Equality for All (2-4)
### Directions:
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

## Quiz: All Tied Up (2-5)
### Directions:
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

## Quiz: Yosa Buson (2-6)
### Directions:
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
