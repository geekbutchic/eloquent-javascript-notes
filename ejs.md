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

* The || operator denotes logical or. It produces true if either of the vales given to it is true.


`console.log(false || true) --> true`
`console.log(false || false) --> false`

// ============================================

* `NOT` is written as an exclamation mark (!).  It is a 
unary operator that flips the value given to it.

// ============================================

### Order of Precedence

* In practice you can usually get by with knowing that of the operators we have seen to date, || or is the lowest precedence, then comes &&, then the comparison operators `(>, ===, and so on)`.
* This order has been chosen such that, in typical expressions, as few parentheses as possible.

### Ternary
* The last logical operator I will discuss is not unary, not binary, but ternary operating on the three values.
* The logical operators && and || handle values of different types in a peculiar way.  They will convert the value on their left side to Boolean type in order to decide what to do, but depending on the operator and the result of that conversion, they will return either the original left-handed value or the right-hand value.

### Summary
* Looked at four types ov JavaScript values: numbers, strings, Booleans, and undefined values.

# Chapter 2



