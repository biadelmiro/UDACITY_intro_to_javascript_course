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
Defining a number in JavaScript is actually pretty simple. The **Number** data type includes any positive or negative integer, as well as decimals. Entering a number into the console will return it right back to you:
```js
3
```
**Returns:** 3

There, you did it.

### Arithmetic operations
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
Let’s take a look at the string datatype. You’ve actually used a string before, and maybe just didn’t know it. When you type a message inside console.log, that message is actually just a JavaScript string. So here, Hiya, Friend, is just a string. Strings can be single letters, like the character h, or even contain numbers, like the string 123. The important thing is that you use quotes to signify a string. It doesn’t matter if the quotes are single or double quotes, but they do have to match. I used double quotes here and single quotes here. If I try to pass the string to the console.log but forget to use the quotes, JavaScript will return back an error. I get this reference error, because the JavaScript engine thinks I’m talking about a variable called hello instead of a string with the value of hello. We haven’t talked about variables just yet, but the moral of the story here is to remember to use quotes when using strings. If I add the quotes in, then the string gets printed out to the console.

**TIP:** It is correct to either use “ or ‘ quotes with strings, as long as you’re consistent. The [JavaScript Udacity style guide](http://udacity.github.io/frontend-nanodegree-styleguide/javascript.html) for labs and projects suggests using single quotes to define string literals.
