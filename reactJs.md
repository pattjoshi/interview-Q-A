# REACT ,REDUX 

# What is the difference between Shadow DOM and Virtual DOM?


### Shadow DOM:
- The Shadow DOM is a browser technology that allows for encapsulation and scoping of DOM elements within a component. It provides a way to create isolated DOM subtrees with their own styles and behavior. The key features of the Shadow DOM include:
- Encapsulation: The styles, structure, and behavior defined within the Shadow DOM are contained within the component and do not affect the rest of the page.
- Scoped CSS: Styles defined within the Shadow DOM are scoped to the component, preventing conflicts with styles from the main document.
- DOM Tree Structure: The Shadow DOM creates a separate DOM subtree that can be attached to an HTML element, providing encapsulation and separation from the main DOM.

### Virtual DOM:

- The Virtual DOM is a concept implemented by certain JavaScript libraries and frameworks, such as React, to improve performance when updating the actual DOM. It is an abstraction of the real DOM, maintained in memory, and used for efficient diffing and updating of the actual DOM. The key features of the Virtual DOM include:
- Reconciliation: The Virtual DOM allows for efficient comparison and update of changes between previous and current states of the UI.
- Batch Updates: The Virtual DOM can perform batch updates to minimize the number of actual DOM manipulations, improving performance.
- Declarative Rendering: Libraries like React use a declarative approach, where the Virtual DOM is updated based on the desired UI state, and the library takes care of efficiently updating the real DOM.


- In summary, the Shadow DOM focuses on encapsulating and scoping DOM elements within a component, while the Virtual DOM is a technique used by certain JavaScript libraries to efficiently update the real DOM based on changes in the UI state. They serve different purposes but can be used together in web applications.

---

# Differentiate between Virtual DOM and Real DOM ?

### Virtual DOM :-
- changes can be made easily.
- minimal memory wastage.
- JSX element is updated if the element exist
- Can not update HTML directly
- Faster updates

### Real DOM 
- Change can be expensive
- High demand for memory and more wastage
- Creates a new DOM every time and EFEMENT GET Updated.
- Able to directly namipulate HTML.
- slow Updates

# What is React ?
- React is widelu ised javaScript library that was lanched in 2011.it was created by developers at Facebook, adn it is prmarily used for frontend development.
- React uses the companent-based approach, which ensure to help you build componets that possess high reusablity.
- React is well Know for developing and designing complex mobile user interfaces and web application.

# What is the meaning of Virtual Dom ?
- A Virtual Dom is a simple JavaScript Object that is the exect copy of the corresopnding real Dom.

- it can be condsidered as a node tree that consists of elements,their attributes,and other propertes.

- Using the render function in react, it creates a node tree and updates it based on the changes that occur in the data model

- These changes are usually triggered by users or the actions caused by the system.

# What are some of the important Features of React.js ?

- React has multiple Features that are used for unique puroses.The important ones are as mentioned below :- 

- React Make use of a single-directonal data flow mode.
- it deals with complete sever-side data processing and handling.
- React uses Virtual DOM that has many advantage of its own.

# What is the meaning of JSX ?

- JSX is the abbrevation of JavaScript xml .
- it is file that is used in React.js to bring out the essence of javaScript to react and use it for its advantages.

- it even includes bringing out HTML and the easy system of javaScript this ensure that tha resuting HTML file will have high readability, thereby relatively increasing the performance of the application.

# Can Browsers read a JSX file ?

- No, Browser cannot read JSX files directly.
- it can only read the objects provided by javaScript.
- Now, it make a browser read a JSX file, it has to be transformed to a javaScript object using JSX transformres,and only then it can be fed into browser for furthdr use in the pipleine.

# Why is React widely used today ?

- React Provides users with an ample number of advantage when building an application. some of them are as follows 
- With React, UI testing becomes very easy.
- React can intergrate with angular and other framwork easily.
- The high readability index ensures easy understanding.
- RReact can be used for both client-side andserver-side requirments.
- it boosts application performance and overall efficiency.

# Are they any disadvantages to use React.js ?

- There are some limitations when useing React as mentioned below 👎
- Writing code is complicated as it uses JSX and inline template framatting.
- Beginners might find it tougto cope with it syntaxes and methods.
- **The library contains a huge repository of information, which might be over whelming.**
- React is a simple library and not a complete fremework hence call for depandencies.

# Differentatiate btn Angular and React

### Angular 
- Google create
- real Dom
- Render Suppory Client side
- Architacture Full MVC support
- Data binding Unidiractional binding

### React 

- Facebook Created
- Virtual Dom
- server Side
- only the view aspect of MVC
- Two-way data binding

---

# What is the meaning of the component-based architecture of React ?

- In react, Components are foundations used to build user interfaces for applications.
- With the component-based system in place, all of the individual entites becomes completely reusable and independed of each other.
- This means that rendering the application is easy and not depended on the other components of the UI.

# How does rendering work in React ?

- Rendering is an important aspect of react as every single component must be rendered.This is done using the render() function.

- Once the function is called,it return an element that represents a DOM component.

- it is alsopossible to render more then one HTML element at a time by enclosing the HTML tegs and passiing it through the render function.

# What are states in React ?

- States form to be once of the vital aspects of react. it considered as a source of data or objects that control aspects such as component behavior and rendering.

- in react, states are used to easily create dynamic and interactive component.

# What are props in React?

- Props are the shothand name given to properties in React.js
- Props are read-only components that are immutable in nature.
- in an application,props follow a hierachy that is passed down from parents to child components.
- However, the reverse is not supported.This is done to ensure that there is only a single directioal flow in data at all times.

# What is the use of an arrow function in react?

- An arrow function is used to write an expession in react.
- it allows user to Manualy bind components easyly.The functionality of arrow functions can be very usefull when you are working with higher-order functioins particulariy.

# What is higher-order component in react ?

- Higer-order components (HOCS) area awidely used techique in react for applying concepts that involve the component reusablity logic.
- They are not a native part of the React API and allow  users to easily reuse the code and bootstrap abstraction.
- HOCs are also used to allow simple sharing of behaviours across all of the compontts in react, adding more advantage to the efficeny and functing of the application.

# wHAT IS THE MEANING OF REDUX ?

- Redux is used to store the state of the application in a single entity
- This simple entity is usually a javaScript object.Changing states can be done by pushing out actions from the application and writing corresponding objects for them that are used to modify the states.

# Difference between props and states ?

### Props
- Changes in child components yes.
- Parent compontnt changing values Yes.
- Change inside components No.
### States
- Changes in child components No.
- Parent compontnt changing values No.
- Change inside components Yes.

# What are the threee phases of a component life cycle in React ?

- **Initial rendering**: This is the phase that involves the begining of the jorney of the component ot the DOM.
- **Update:-** Hear, the component can be updated and render again of required after it gets added to the DOM.
- **Unmounting:-** The final phase involves the destruction of the component and its eventual removal from the DOM.

# What are events in React ?

- When ever there are actions performed in React,sucha s hovering of the mouse or pressing a key on the key board, thes actions trigger events.
- **Events** then perform set activities as a response to these triggers.
- Handling an event in React is very similar to the DOM architecture.

# How is routing in react different from coventional routing ?

- **Pages:** Each view is considered as a new file in convernional routing which it is considered as a single HTML entity in React.

-**Navigation:-** in convention routing, user have to move across web Page for viewing. In React, the views are not refreshed as objects are re-issued to create new views.

# what is the meaning of synthetic events in React?

- **synthetic events** in React are objects that act as cross-browser wrappers,allowing for the use of  native events.

theis is done to ensure that a variety of browser can run the API and that the event contains all properites.

# What are statefull components in React ?

- **statefull components** are entities that store the changes that happen and place them into the memory.
- Here, the state can be changed, alongside string information such as past,current, and future changes.

# What are **refs** in React?

- **Refs** is short for references in React.
- refs are used to store a reference to a single react element or a react component.This is later returned using the render function.
- They are maninly used in the following senarios:- 
- To initiate imperative animations.
- To join third-party DOM libraryes.
- To manages focus and apply media playback.

# What are controlled components in React?

- controlled components in React fefer to the components that have the ability to maintain their state.
- The data is completely controlled by the parent component,and the current value is fetched by making use of props.
- This is done to natify about any change that occurs when using callbacks.

# Why is a router required in react ?

- A router is very much necessary in react as it  is used to manage multuple routes whenever a user type in URL. if the router is  present in the router for the corresponding URL,then user is taken to the particular route.
- To do this,the router libary needs to be added in React.

# What are the components of redux in React ?

- Redux consists of **four** main components as shown below:-
- **Action:** an object that describes the call
- **Reducer** the state change storeage unit
- **Store** the state and object tree store 
- **view** displays data provided by the store

# What are the advantage of using Redux ?

- Organized Approch :- Redux requires code to be organized,thereby making it consistent and easy to work with.
- Testing Ability :- Redux fuctions are small and isolated,making the code more independent and taskable.
- Tools :- Developers can track actions and all of the tools in React using Redux easily.
- Community :- Redux has a large community, helping user with efficient and easy-to-use libraries.

# What are the disadvantages of using MVC in React?

- Among a plethore of advantages of using MVC in React, there are **minor** problems as stated below 👎
- A lot of menory wastage occurs
- DOM manipulation costs a lot
- the application becomes slow
- lots of dependencies are created
- The complexity of models increases

# What are pure componets in React?

- Pure components are singular entites that written in React.
- They are fast and simple to write and have athe ability to replace a component that has only the render() function.
- This is done to ensure that the performance of the application is good and that the code is kept simple at the same time.

# what is higher-order components (HOCs) used for?

- HOCs are used for a veriety of tasks such as 
- Manipulation of props.
- State mainpulation and abstraction.
- Render high jacking.
- Code reusing.
- Bootstrap abstraction.

# What are keys in React?

- Keys are used in react to check all items and to track changes actively.
- They are used to directly check if an item has been added or removed from a list.

# Diff Controlled component and uncontrolled component in react?

- A **Controlled component**, as the name suggests, is a component over which  react has compoete control.
- it is the singular point of data for the froms.

- An **uncontrolled component** is one where the form data gets handled by DOM and not the react component.
- This is usullyh done using refs on React.

# What is the use of the second argument that is passed to setState? is it optional?

- When setState is finished a callback function is invoked,and the components get re-render in React.
- **yes,it is an optional argument** since setState is asynchronous, it takes in another callback function.
- However,in programming practics, it is always good to use another ife cycle method instead of this.

# What is the Strictmode component use in React?

- The strictMode component when used would beefit user immensely while creating new code base to understand the components being used.
- However,it can fit well in debugging as well becouse it will help solve the problem faster when it is wrapped with other components, which could be causing the problem.

# What would you do if your react application is rendering slowly?

- The cause of slow rendering in react i smostly becaouse of number of re-render opctions. which are somtimes unnessary.
- There are two main tools provided by react tohelp used hear
- React.memo():- this used to prevent all of the unnecessary re-rendering carried out by the function componrnts.
- PureComponent : this is used to ensure that the unnecessory re-redering of class components are avoided.

# Why is props passed to the super() function in React?

- props gets passed onto the super() function if a user wishes to access this.props in the constructor.

# What is the difference btn using getlnitialstate and constructors in react?

- when using ES6 user must initialize the state in the constructor and the getlinitialState menhod is defined.

- This is done using React.createClass.

# What is React fiber ?

- React fiber is a new engine in react, it is the reimplacmentation core algorithm in react 16.
- The main goal of react fiber is to ensure that there are incremental rendering facilities for the virtual DOM.
- This increases effciency when reddering animations, gestures, etc. and also helps in assigning priority to updates based on the requirement, there by increasing overall effciency.

# What are hooks in react ?

- Hooks are used to make use of the state and other feature without having to explicitly  write a class. hooks were added to react version 16.8.
- The statefull login can be extracted from a component easily,alongside testing and reusing it.
- All of this is done with out making any changes to the conponent hierarchy.


# Why does React use className over class attribute?

- React uses className instead of the traditional HTML class attribute for styling elements to avoid conflicts with JavaScript's class keyword.

# What are fragments?

- Fragments in React.js are a way to group multiple elements together without adding an extra wrapper element to the DOM.

-  Fragments are denoted using the <React.Fragment> syntax or the shorthand syntax <>


# What is the purpose of push() and replace() methods of history?

- The push() and replace() methods in the history object serve the following purposes:

- push(): Adds a new entry to the browser's history stack, allowing navigation forward and backward through history. It renders the corresponding component or route associated with the new URL.

- replace(): Replaces the current entry in the browser's history stack with a new URL. It updates the URL without creating a new entry in the history stack.

- Both methods facilitate programmatic navigation within a React application, enabling dynamic URL changes and rendering different components based on user interactions or application logic.

# difference between Use dispatch use silector ? 

- useDispatch: Purpose: Used to dispatch actions to the Redux store.
Usage: It returns a reference to the dispatch function, which is used to send actions to update the state in the Redux store.

- useSelector: Purpose: Used to access the state from the Redux store.
Usage: It allows you to extract and use specific parts of the state stored in the Redux store.

- In summary, useDispatch is used to dispatch actions to update the state in the Redux store, while useSelector is used to extract specific parts of the state from the Redux store and use them within components.

---

# Redux  

---
# Redux thunk 

- Redux Thunk middleware is used to handle asynchronous actions in Redux.
- It enables dispatching of functions as actions, allowing for async operations such as API calls, fetching data, and handling side effects.

- In summary, Redux Thunk allows you to write action creators that return functions instead of action objects, enabling asynchronous operations and side effects within Redux. It helps handle async logic in a more organized and controlled manner.











