# BASIC JAVASCRIPT
===========================
## Diff between let ,const & var

### Var :-
- If we declare a veriable from var. then we can also **decleare it again with the same name**. 
- and if we want to **re-assign** it’s value then we can do that to. 
- var has **function scope.**

### let 

- let has **block scope**. It is scoped to the nearest enclosing block, such as a loop or an if statement.
- If we declare a veriable with let, then **we connot declare it again with the same name. but can re-assign its value.**

### const
- const also has block scope like let.
- if we declare variable with const, then we can neither decleare it again, not can re-assign its value Not modified

- It is generally recommended to use let or const over var because they provide block scoping, which helps prevent unintended bugs and makes the code more predictable. Use const when you have a variable that should not be reassigned, and use let for variables that require reassignment.

---

## Scope chaining

- Scope chaining, also known as lexical scoping or scope inheritance,
-  refers to the mechanism in which the variables and functions defined in **one scope can be accessed by an inner scope.**
-   In JavaScript, scope chaining is established through the nested structure of functions or blocks.

## Hoisting js

- Hoisting is a concept which enables us to **extract values of variables and functions even before initialising**/assigning value without getting error and this is happening **due to the 1st phase** (memory creation phase) of the Execution Context.

## Clouser's


df;f;


