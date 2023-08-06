# [QUS SOURSE](https://github.com/pattjoshi/MERN_QUS/blob/master/react%20and%20js%20qus%20Spandan%20da.txt)

# BASIC JAVASCRIPT

---

# 1. Difference between let, const & var:

- var is function-scoped and can be re-declared and updated throughout the function or globally.

- let and const are block-scoped. let allows re-assignment, while const is used for variables that should not be re-assigned (it's not immutable, just the reference cannot change).

# 2. Scope chaining:

- Scope chaining refers to the process of searching for variables in nested scopes in JavaScript.

- If a variable is not found in the immediate local scope, JavaScript looks for it in the outer (enclosing) scopes until the global scope is reached.

- The process of going one by one to parent and checking for values is called scope chain or Lexcial environment chain.



# 3. Hoisting:

- Hoisting is a concept which enables us to extract values of variables and functions even before initialising/assigning value without getting errors and this is happening due to the 1st phase (memory creation phase) of the Execution Context.

# 4. Closures:

- Function bundled along with its lexical scope is closur

- Closures are functions that have access to variables from their outer (enclosing) function even after the outer function has finished executing.
They "remember" the environment in which they were created.

# 5. Higher-order function:

- Higher-order functions are functions that take one or more functions as arguments or return a function as a result.
- They enable functional programming paradigms and allow for code reuse and composition.

# 6. "this" keyword:

In JavaScript, this refers to the object that the function is bound to and its value depends on how the function is called.
It can be explicitly set using call, apply, or bind.

# 7. NaN property in JavaScript:

NaN stands for "Not a Number" and is a special value of the Number data type in JavaScript.
It is returned when a mathematical operation is performed, but the result is not a valid number.

# 8. Concatenate a string:

- String concatenation is the process of combining two or more strings into one.
- In JavaScript, you can use the + operator or template literals (backticks) for string concatenation.

# 9. How to create an array:

- Arrays can be created in JavaScript using array literals [ ] or the Array constructor: let arr = new Array();.

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

# Difference Between Rest & Spread Operator?

- **Spread Operator (...)**

- Syntax: ...variable
- Used in: **Function calls**, array literals, and object literals.
- Purpose: It spreads or expands the elements of an array or the properties of an object into individual elements or properties.

- **Rest Operator (...)**

- Syntax: ...variable
- Used in **Function parameters** (function arguments) and destructuring assignments.
- Purpose: It collects the rest of the elements into an array when working with function arguments or destructuring arrays or objects.

- In summary, the Spread operator is used to expand elements or properties, while the Rest operator is used to collect the remaining elements or properties into an array or object.


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

# 23. web pack and Bable

### Webpack
- Webpack is a module bundler for JavaScript applications that takes modules with dependencies and generates static assets representing those modules. It's used to package JavaScript files for usage in a browser.

### Bable
- Babel is a compiler (or transpiler) that transforms modern ECMAScript (JavaScript) code into a backward compatible version of JavaScript that can run in older browsers or environments. It's mainly used to convert ECMAScript 2015+ code into a backward-compatible version of JavaScript.

# 24. async await

- async/await is a syntactic feature in JavaScript used to write asynchronous code in a more synchronous-like manner.
-  It allows developers to work with promises using a more familiar and readable syntax.
-  By using the async keyword before a function and await before a promise, developers can write asynchronous code that appears to execute in a sequential and straightforward manner.

# 25 What are promises in j.s?

- Promises in JavaScript are a way to handle asynchronous operations. They are objects that represent the eventual completion (or failure) of an asynchronous operation and allow developers to write more readable and structured code for handling asynchronous tasks.
-  Promises have three states: pending (initial state), fulfilled (operation succeeded), and rejected (operation failed).
- They provide methods like .then() and .catch() to handle the successful and error outcomes of asynchronous operations in a more organized and predictable manner.

# 26.What is curring?

- Currying is a functional programming technique in which a function that takes multiple arguments is transformed into a series of functions, each taking a single argument.
-  Instead of calling the function with all its arguments at once, you call it with one argument at a time, and it returns a new function that takes the next argument, and so on until all arguments are received.

```
// Curried version of the same function
function curriedAdd(a) {
  return function (b) {
    return function (c) {
      return a + b + c;
    };
  };
}

// Usage of the curried function
const result = curriedAdd(1)(2)(3); // result will be 6
```
# 27. what is temporal dead zone js? 

- Temporal Dead Zone (TDZ) in JavaScript refers to the period between the creation of a variable using let or const and the point where it is initialized with a value.
- During this period, accessing the variable will result in a ReferenceError. It helps to catch potential errors and enforce better coding practices.

---

# IIFE :- 
- Immediately Invoked Function Expression (IIFE) is a JavaScript function that is executed immediately after it is defined.
-  It is typically used to create a private scope for variables and avoid polluting the global scope. 

# map() filter() reduxe() :- 

- map(): It creates a new array by applying a callback function to each element of the original array. The callback function can modify the elements and return the new values.

- filter(): It creates a new array containing only the elements that pass a given condition specified in the callback function.

- reduce(): It reduces the elements of an array to a single value by applying a callback function that accumulates the results. It iterates through the array, maintaining an accumulator that stores the intermediate result.

```
// map()
const numbers = [1, 2, 3, 4];
const doubled = numbers.map((num) => num * 2); // Result: [2, 4, 6, 8]

// filter()
const ages = [25, 30, 18, 40];
const adults = ages.filter((age) => age >= 18); // Result: [25, 30, 18, 40]

// reduce()
const nums = [1, 2, 3, 4];
const sum = nums.reduce((acc, num) => acc + num, 0); // Result: 10
```


# REACT.JS

---

# 1. Major features of React:

- Virtual DOM: Efficiently updates and renders changes to the actual DOM.
- Component-based architecture: Encourages building UIs as reusable components.
- One-way data flow: Data flows from parent components to child components.
- JSX: A syntax extension that allows writing HTML-like code in JavaScript.
- Unidirectional data flow: State changes are propagated from parent to child components.
- Reusable components: Components can be composed and reused throughout the application.

# 2. JSX:

- JSX (JavaScript XML) is a syntax extension for JavaScript used in React to describe the structure of the UI components.
- It allows developers to write HTML-like code within JavaScript, making it easier to create and visualize component trees.

# 3. Pure Components:
- Pure Components are a type of React component that extends React.
- PureComponent instead of React.Component. They automatically implement a shouldComponentUpdate method with a shallow prop and state comparison, optimizing performance by avoiding unnecessary re-renders.

# 4. State in React:

- State is a mechanism in React that allows components to maintain and manage their internal data.
- When state data changes, React re-renders the components to reflect those changes in the UI.

# 5. Difference between state and props:

- Props are used to pass data from parent to child components, and they are immutable (cannot be changed within the child component).
- State is used to manage internal component data and can be changed using setState().

# 6. Purpose of the callback function as an argument of setState():

- The callback function provided as an argument to setState() is executed after the state update is complete and the component has re-rendered.
-  It allows performing additional tasks that depend on the updated state.

# 7. Difference between HTML and React event handling:

- In HTML, event handlers are assigned as attributes with inline JavaScript code, like onclick="handleClick()".
-  In React, event handling is done using camelCase event names as props, like onClick={() => handleClick()}.

# 8. "key" prop and its benefit in arrays of elements:
- The "key" prop is a special attribute used by React when rendering arrays of elements.
-  It helps React identify which items have changed, been added, or removed in a list, improving the efficiency of re-rendering and preventing unnecessary re-renders.

# 9. How to bind methods or event handlers in JSX callbacks:

- To bind methods or event handlers in JSX callbacks, you can either use arrow functions like onClick={() => this.handleClick()}, or bind the method in the constructor like this.handleClick = this.handleClick.bind(this).

# 10. Inline conditional expressions:

- Inline conditional expressions in JSX allow rendering different content based on a condition.
-  The syntax involves using the ternary operator, for example: {isLogged? <LoggedInComponent /> : <LoggedOutComponent />}.

# 11. React uses virtual DOM or real DOM?

- React uses a virtual DOM. It is a lightweight copy of the actual DOM that React uses to keep track of changes.
-  When there are updates, React compares the virtual DOM with the actual DOM and efficiently updates only the necessary parts.

# 12. How does virtual DOM work?

- When there are changes in the state or props of a React component, it re-renders the component and creates a new virtual DOM tree.
- React then performs a diffing algorithm to compare the new virtual DOM with the previous one and calculates the minimal changes needed to update the actual DOM efficiently.

# 13. Difference between Shadow DOM and Virtual DOM:

- Shadow DOM is a browser technology that encapsulates the DOM and styles of a component, preventing them from affecting other parts of the page.
- Virtual DOM is a concept used by React to efficiently update the actual DOM by comparing the changes between two virtual DOM trees.

# 14. Different phases of the component lifecycle:
- The component lifecycle in React has three main phases:

- Mounting: When the component is being created and inserted into the DOM.
- Updating: When the component is re-rendered due to changes in props or state.
- Unmounting: When the component is removed from the DOM.

# 15. Higher-Order Components (HOC):
- Higher-Order Components are functions that take a component as an argument and return a new enhanced component with additional props or behaviors.
-  HOCs are used for code reuse and logic sharing among multiple components.

# 16. Why does React use "className" over the "class" attribute?

- React uses "className" instead of the "class" attribute to define CSS classes on HTML elements.
-  This is because "class" is a reserved keyword in JavaScript, and using "className" prevents conflicts and follows the JSX syntax conventions.

# 17. Fragments:

- Fragments allow grouping multiple elements without adding an extra wrapping element.
-  They improve the component's readability and avoid unnecessary DOM nesting.
-   Fragments are represented by the empty tag <> ... </> or the <React.Fragment> ... </React.Fragment> syntax.

# 18. Stateless components & stateful components:

- Stateless components (functional components) are written as pure functions and do not have their own state.
- Stateful components (class components) have their own state, allowing them to manage and update data.

# 19. How to apply validation on props in React?

- You can apply validation on props in React using the propTypes property or the prop-types library.
-  propTypes allow you to define the expected types and requirements for each prop in a component.

# 20. Is it good to use setState() in componentWillMount() method?

- No, it is not recommended to use setState() in the componentWillMount() method.
-  The reason is that it may trigger additional renders, leading to performance issues.
-   It is better to initialize the state in the constructor or use the new static getDerivedStateFromProps() method.

# 21. How to use the React label element?
- To associate a label with an input element in React, use the htmlFor attribute in the label element and provide the id of the corresponding input element.
-  This helps in improving accessibility by allowing screen readers to correctly associate labels with form inputs. Example:


```
<label htmlFor="inputField">Name:</label>
<input id="inputField" type="text" />
```

---
# React router
---

# Purpose of push() and replace() methods of history:
- In React, the push() and replace() methods are part of the history object, which is provided by React Router. They allow you to control the navigation and manipulate the browser's history.

- push(path, [state]): This method adds a new entry to the history stack, pushing the user to the specified path. It is typically used when you want to navigate to a new page or route.

- replace(path, [state]): This method replaces the current entry in the history stack with the new path. It is commonly used when you want to update the URL without creating a new history entry, useful for situations like form submissions or redirects.

# How to perform automatic redirect after login:

- To perform an automatic redirect after login, you can use the history.push() method or leverage React Router's <Redirect> component.

- Assuming you have a login component and want to redirect the user to a dashboard page after successful login, here's a general approach:


```
import React, { useState } from 'react';
import { useHistory } from 'react-router-dom';

const LoginComponent = () => {
  const [isLoggedIn, setLoggedIn] = useState(false);
  const history = useHistory();

  const handleLogin = () => {
    // Perform login logic and set isLoggedIn to true upon successful login
    setLoggedIn(true);

    // After successful login, redirect the user to the dashboard
    history.push('/dashboard');
  };

  return (
    <div>
      {/* Your login form */}
      <button onClick={handleLogin}>Login</button>
    </div>
  );
};

export default LoginComponent;
```

---

# Redux  

---

# 1. What is Redux?
- Redux is a predictable state management library for JavaScript applications, commonly used with React.
- It helps manage the state of an application in a centralized store and enables components to access and modify the state in a predictable manner.

# 2. What are the core principles of Redux?

- The core principles of Redux are:

- Single source of truth: The state of the entire application is stored in a single store, making it easy to manage and debug.
- State is read-only: The state can only be modified through dispatched actions, ensuring predictability and traceability of changes.
- Changes are made by pure functions: To update the state, reducers (pure functions) are used, which take the previous state and an action and return a new state.

# 3. Difference between useDispatch and useSelector:

- useDispatch is a hook provided by React Redux to dispatch actions to the Redux store from functional components.
- useSelector is a hook that allows components to extract and read data from the Redux store state.

# 4. Redux Thunk:
- Redux Thunk is a middleware for Redux that allows writing asynchronous logic and side effects in Redux actions.
-  It enables actions to return functions instead of plain objects, giving more flexibility in handling asynchronous operations like API calls.

# 5. How to dispatch an action on load?

- To dispatch an action on load, you can use the useEffect hook from React.
- Within the useEffect callback, call the dispatch function with the action you want to trigger.

# 6. How to use connect() from React Redux?

- The connect() function is used to connect a React component to the Redux store.
-  It transforms the component into a connected component, allowing it to access state and dispatch actions.
-  In modern React applications, it is more common to use the useSelector and useDispatch hooks to achieve the same result.

# 7. What is the purpose of constants in Redux?
- Constants in Redux are used to define action types.
- They ensure that action types are consistent and easily maintainable throughout the application.
- By defining action types as constants, it helps prevent typos and improves code readability.

# 8. What is Redux Thunk?

- Redux Thunk is a middleware that allows asynchronous operations and side effects to be handled within Redux actions.

-  It enables action creators to return functions instead of plain objects, allowing delayed dispatching and coordination of multiple actions.

- In summary, Redux Thunk allows you to write action creators that return functions instead of action objects, enabling asynchronous operations and side effects within Redux. It helps handle async logic in a more organized and controlled manner.

# 9. What are Redux DevTools?

- Redux DevTools is a browser extension that provides a set of powerful development tools for inspecting, debugging, and time-traveling through Redux state changes. 
- It allows developers to visualize the state and actions, making it easier to track and understand the application's behavior.

# 10. What is an action in Redux?

- An action in Redux is a plain JavaScript object that describes an event or intention to change the state of the application.
- It must have a type property that defines the type of action being performed and can also include additional data required for the state update.

# 12. What is the proper way to access the Redux store?

- In a React component, you can use the useSelector hook from React Redux to access the Redux store state and retrieve the required data. 
- The useSelector hook takes a selector function as an argument and returns the data from the store based on that selector.
