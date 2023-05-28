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































