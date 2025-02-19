# What is JS?

JavaScript is the programming language of the web. It can update and change both HTML and CSS. It can calculate, manipulate and validate data. JavaScript was invented by Brendan Eich in 1995 and became an ECMA standard in 1997.

# Where to?

JS can be added inside html doc using script tag in head or in the end of the body. always add it in the end of the body so that it loads after the visible content.

# Output

- Writing into an HTML element, using `innerHTML` or `innerText`.(changes text)
- Writing into the HTML output using `document.write()`.(don’t use)
- Writing into an alert box, using `window.alert()`.(pop up window)
- Writing into the browser console, using `console.log()`.(prints in console)
- The only exception is that you can call the `window.print()` method in the browser to print the content of the current window.

# Important

1. Always use ; at the end of statement
2. JS ignores whitespace.

# JS values

1. Fixed values/literals
2. Variable values

# Comments

1. one line:  // text
2. multiline: /* text */

# Var names

- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter.
- Names can also begin with $ and _ (but we will not use it in this tutorial).
- Names are case sensitive (y and Y are different variables).
- Reserved words (like JavaScript keywords) cannot be used as names.

# Var, let , const

1. Always declare variables
2. Always use `const` if the value should not be changed
3. Always use `const` if the type should not be changed (Arrays and Objects)
4. Only use `let` if you can't use `const`
5. Only use `var` if you MUST support old browsers.
6. Always declare all variables on the top of script,

# Difference Between var, let and const

|  | Scope | Redeclare | Reassign | Hoisted | Binds this |
| --- | --- | --- | --- | --- | --- |
| var | No | Yes | Yes | Yes | Yes |
| let | Yes | No | Yes | No | No |
| const | Yes | No | No | No | No |

# Now the imp things about variables in js

1. var have function scope. and other two have bloack scope.
2. when you do this:
   console.log(a); // ✅ Undefined (not an error)
var a = 5;
but when you do this:
console.log(b); // ❌ ReferenceError (TDZ)
let b = 10;
it enters a temporal dead zone.
3. Closures: A closure is when an inner function remembers variables from its outer function, even after the outer function has executed.
4. shadowing: Below example shows shadowing in JS.
   let x = 10;
{
    let x = 20; // This "shadows" the outer x
    console.log(x); // 20 (inner variable)
}
console.log(x); // 10 (outer variable)

# JS operators

- Arithmetic Operators

| + | Addition |
| --- | --- |
| - | Subtraction |
| * | Multiplication |
| ** | Exponentiation ([ES2016](https://www.w3schools.com/Js/js_2016.asp)) |
| / | Division |
| % | Modulus (Division Remainder) |
| ++ | Increment |
| -- | Decrement |
- Assignment Operators

| Operator | Example | Same As |
| --- | --- | --- |
| = | x = y | x = y |
| += | x += y | x = x + y |
| -= | x -= y | x = x - y |
| *= | x *= y | x = x * y |
| /= | x /= y | x = x / y |
| %= | x %= y | x = x % y |
| **= | x **= y | x = x ** y |
- Comparison Operators

| Operator | Description |
| --- | --- |
| == | equal to |
| === | equal value and equal type |
| != | not equal |
| !== | not equal value or not equal type |
| > | greater than |
| < | less than |
| >= | greater than or equal to |
| <= | less than or equal to |
| ? | ternary operator |
- Logical Operators

| Operator | Description |
| --- | --- |
| && | logical and |
| || | logical or |
| ! | logical not |
- Bitwise Operators

| Operator | Description | Example | Same as | Result | Decimal |
| --- | --- | --- | --- | --- | --- |
| & | AND | 5 & 1 | 0101 & 0001 | 0001 | 1 |
| | | OR | 5 | 1 | 0101 | 0001 | 0101 | 5 |
| ~ | NOT | ~ 5 | ~0101 | 1010 | 10 |
| ^ | XOR | 5 ^ 1 | 0101 ^ 0001 | 0100 | 4 |
| << | left shift | 5 << 1 | 0101 << 1 | 1010 | 10 |
| >> | right shift | 5 >> 1 | 0101 >> 1 | 0010 | 2 |
| >>> | unsigned right shift | 5 >>> 1 | 0101 >>> 1 | 0010 | 2 |
- Type operators

| Operator | Description |
| --- | --- |
| typeof | Returns the type of a variable |
| instanceof | Returns true if an object is an instance of an object type |
- Ternary Operators

# Operator precedence
1. ()
2. **
3. *,/,%
4. +,-

# Taking input from user
1. Noob do this: using prompt
2. Using HTML input and then getting the value the user entered in the textbox. (COOL..Isnt it?)
   
# Data types

String

Number

Bigint

Boolean

Undefined

Null

Symbol

Object: objects are god 

# Function

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

### Syntax

function *name(parameter1, parameter2, parameter3)*{

//*code to be executed*

}

### Return

When JavaScript reaches a `return` statement, the function will stop executing.
