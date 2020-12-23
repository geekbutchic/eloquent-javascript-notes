# Eloquent Javascript Notes
* ARITHMETIC 

  * `PEMDAS` Parenthesis Equals Multiplication Division Addition Subtraction 
  * `100 + 4 * 11`
  * In this situation multiplication would happen first.
  * `(100 + 4) * 11`
  * In this situation parenthesis would happen first.
  * When multiple operators with the same precedence appear next to each other, as in 1 - 2 + 1, they are applied left to right: `(1 -2) + 1.`
  * The % symbol is used to represent the remainder operation.


* STRINGS 
  * Strings are created using 'quotations' or `backticks` 
  * `\n` interpreted as a new line 
  * "This is the first line\nAnd this is the second line."
```javascript
This is the first line 
And this is the second
```
* CONCATENATION 
  * "con" + "cat" + "e" + "nate"
  * The line above will produce the string "concatenate"
  * `half of 100 is ${100 / 2}`
  * When you write somthing inside ${} in a template literal, it's results will be computed, converted to a sting, and included at that position.
  * `"half of 100 is 50"`

* UNARY OPERATORS
  * `console.log (typeof 4.5) -> number`
  * `console.log (typeof "x") -> string`
  * Operators that use two values are called binary operators, while those that take one care called unary operators.

* BOOLEAN VALUES 
  * Only two possible values "yes" or "no" 

COMPARISON 

* `>= (greater than or equal to)`
* `<= (less than or equal to)`
* `=== (equal to)`
* `!= (not equal to)`

LOGICAL OPERATORS 

* There are also some operations that can be applied to Boolean values themselves.  JavaScript supports three logical operators: `and, or and not.`
* The `||` operator denotes logical or. It produces true if either of the vales given to it is true.  


`console.log(false || true) --> true`

`console.log(false || false) --> false`

// ============================================

* `NOT` is written as an exclamation mark (!).  It is a 
unary operator that flips the value given to it - 

`!true produces false, and false gives true.`

// ============================================

* The && operator represents logical and.  It is a binary operator, and it's result is true only if both the values given to it are true.

`console.log(true && false) --> false`

`console.log(true && true) --> true`

* The rules for converting strings and numbers to Boolean values state that O, NaN, and the empty string ("") count as false, while all the other values count as true.  So `0 || -1 produces -1, and "" || "!?" yields "!?"`

### Order of Precedence

* In practice you can usually get by with knowing that of the operators we have seen to date, || or is the lowest precedence, then comes &&, then the comparison operators `(>, ===, and so on)`.
* This order has been chosen such that, in typical expressions, as few parentheses as possible.

### Ternary
* The last logical operator I will discuss is not unary, not binary, but ternary operating on the three values.
* The logical operators && and || handle values of different types in a peculiar way.  They will convert the value on their left side to Boolean type in order to decide what to do, but depending on the operator and the result of that conversion, they will return either the original left-handed value or the right-hand value.

### Summary
* Looked at four types ov JavaScript values: numbers, strings, Booleans, and undefined values.

# Chapter 2

### Program Structure

*   Expressions and Statements
*   Bindings 
    *   To catch and hold values, JavaScript provides a thing called a binding or variable.
    *   `let caught = 5 * 5;`
    *   The special word (keyword) let indicates that this sentence is going to define a variable.  It is followed by the name the variable and, if we want to immediately give it a value, by an = operator and an expression.
    *   let + keyword = operator

* When a binding points at a value, that does not mean it is tied to that value forever.  The `=` operator can be used at any time on existing bindings to disconnect them from their current value and have them point to a new one.

```javascript 
let mood = "light";
console.log(mood);
// -> light
mood = "dark";
console.log(mood);
// -> dark
```
* A single let statement may define multiple bindings.  The definitions must be separated by commas.
  * `let one = 1, two = 2;`

* The word const can also be used to create bindings, in a way similar to let.
* The word const stands for constant.  It defines a constant binding, which points at the same value for as long as it lives.  This is useful for bindings that give a name to a value so that you can easily refer to it later.

### Functions
  * Executing a function is called invoking, calling, or applying it.  You can call a function by putting parentheses after an expression that produces a function value.

Return Values

* For example, the function Math.max takes any amount of number arguments and gives back the greatest.
* `console.log(Math.max(2, 4));`

When a function produces a value, it is said to return that value.  Anything that produces a value is an expression in JavaScript.

* `console.log(Math.min( 2, 4) + 100);`

### Control the Flow 
*  The function `Number` converts a value to a number.  Which is needed since the conversion is a string value.
* `let theNumber = Number(prompt("Pick a number"));`

### Conditional Execution
* Conditional execution is created with the `if` keyword in JavaScript.  In the simple case, we want some code to be executed if, and only if, a certain condition holds.
```javascript
let theNumber = Number(prompt("Pick a number"));

if (!Number.isNAN(theNumber)) {
    console.log("Your number is the square root of " + theNumber * theNumber);
}
```
* the `Number.isNaN` function is a standard JavaScript function that returns `true` only if the argument it is given is NaN.

