# [QUS SOURSE](https://github.com/pattjoshi/MERN_QUS/blob/master/react%20and%20js%20qus%20Spandan%20da.txt)

# BASIC JAVASCRIPT

---

# 1. Difference between let, const & var:

- var is function-scoped and can be re-declared and updated throughout the function or globally.

- let and const are block-scoped. let allows re-assignment, while const is used for variables that should not be re-assigned (it's not immutable, just the reference cannot change).

# 2. Scope chaining:

Scope chaining refers to the process of searching for variables in nested scopes in JavaScript.
If a variable is not found in the immediate local scope, JavaScript looks for it in the outer (enclosing) scopes until the global scope is reached.

# 3. Hoisting:

Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their containing scope during the compilation phase.
However, only the declarations are hoisted, not the initializations.

# 4. Closures:

Closures are functions that have access to variables from their outer (enclosing) function even after the outer function has finished executing.
They "remember" the environment in which they were created.

# 5. Higher-order function:

Higher-order functions are functions that take one or more functions as arguments or return a function as a result.
They enable functional programming paradigms and allow for code reuse and composition.

# 6. "this" keyword:

In JavaScript, this refers to the object that the function is bound to and its value depends on how the function is called.
It can be explicitly set using call, apply, or bind.

# 7. NaN property in JavaScript:

NaN stands for "Not a Number" and is a special value of the Number data type in JavaScript.
It is returned when a mathematical operation is performed, but the result is not a valid number.

# 8. Concatenate a string:

String concatenation is the process of combining two or more strings into one.
In JavaScript, you can use the + operator or template literals (backticks) for string concatenation.

# 9. How to create an array:

Arrays can be created in JavaScript using array literals [ ] or the Array constructor: let arr = new Array();.

# 10. Create an object in JavaScript:
- Objects can be created using object literals { } or the Object constructor: let obj = new Object();.

# 11. Normal function vs. arrow function:
- Normal functions have their own this context, which is dynamically determined at runtime based on how the function is called.
- Arrow functions do not have their this context, and instead, they lexically inherit the this value from their enclosing scope.

# 12. Difference between == and ===:
- == is the equality operator and performs type coercion, meaning it converts operands to the same type before comparison.
- === is the strict equality operator and does not perform type coercion, comparing both value and type.

# 13. Spread operator:
- The spread operator (...) allows an iterable (like an array or string) to be expanded into individual elements.
- It is commonly used for creating shallow copies of arrays, merging arrays, and passing function arguments.

# 14. Object destructuring:
- Object destructuring is a way to extract properties from an object and assign them to variables in a more concise manner.

# 15. Callback:
- A callback is a function that is passed as an argument to another function and is executed after the completion of that function.

# 16. Callback hell:
- Callback hell refers to the situation where multiple nested callbacks make the code difficult to read and maintain.
- This can happen when dealing with asynchronous operations.

# 17. Recursion:
- Recursion is a programming technique where a function calls itself to solve a problem.
- It is essential to have a base case that stops the recursive calls.

# 18. Difference between synchronous & asynchronous:
- Synchronous operations block the program's execution until the operation is completed.
- Asynchronous operations allow the program to continue executing while waiting for the operation to complete.

# 19. Nonblocking I/O operation:
- Nonblocking I/O allows the program to continue executing other tasks while waiting for I/O operations to complete.
- This is commonly used in asynchronous programming.

# 20. Where we can use Node.js:
- Node.js is commonly used for building server-side applications and APIs.
- It excels in handling concurrent connections, making it suitable for real-time applications, chat applications, and streaming services.


# 22. What is the difference between "null" and "undefined" in JavaScript?

- "Null" represents the intentional absence of a value and is usually assigned by the programmer.
- "Undefined" means a variable has been declared but hasn't been assigned any value yet.

# Explain the use of the "this" keyword in JavaScript.

- "this" refers to the current context or object within a function or method.
- Its value is determined by how a function is called, and it can change based on the context of the execution.



# Redux  

---
# Redux thunk 

- Redux Thunk middleware is used to handle asynchronous actions in Redux.
- It enables dispatching of functions as actions, allowing for async operations such as API calls, fetching data, and handling side effects.

- In summary, Redux Thunk allows you to write action creators that return functions instead of action objects, enabling asynchronous operations and side effects within Redux. It helps handle async logic in a more organized and controlled manner.


# What is the purpose of the constants in Redux?

- Clear identification: Constants provide a clear and unique identifier for each action type in Redux.

- Preventing errors: By using constants, typos and syntax errors in action types can be caught at compile-time, minimizing bugs and runtime issues.

- Code consistency: Constants ensure that the same action type is consistently used across the application, promoting code clarity and reducing confusion.

- Refactoring ease: Constants make it easier to refactor and maintain code by centralizing action type definitions, allowing for easy updates and modifications.

# What is Redux DevTools?

- Redux DevTools is a browser extension and development tool that enhances the debugging and monitoring capabilities of Redux applications.

- Redux DevTools greatly simplifies the process of debugging Redux applications by providing a visual representation of actions, state changes, and middleware effects. It offers powerful capabilities for inspecting, replaying, and analyzing the application's state and behavior, ultimately improving productivity and reducing development time.

# What is an action in Redux?

- In Redux, an action is a plain JavaScript object that represents an event or intention to change the state of an application.

- actions serve as a standardized way to communicate changes and interactions in a Redux application, enabling predictable state updates.









