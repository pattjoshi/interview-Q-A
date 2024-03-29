# NODE.JS interview question 👩‍💻

---

# Differntiate between javaScript and Node.js

## javaScript

- js is Programming Language.
- Use for any **clint-side** activity for web application.
- Running Engine is Spider monkey (FireFox), JavaScript Core (safari),Google chrome(V8)

# Node.js

- Interpeter and envirnoment for JavaScript.
- Used for access of Performing any non-blocking Opertion of any Operation System.
- use JavaScript out side of a browser.
- V8 (Google Chrome)

---

# What is Node.js

- node.js is not javascript Framework , node.js is javaScript Runtime. that run javaScript code outside the browser .
- It's Developed on Chrome's _V8_ JavaScript engine.
- it compile js directly into the machin code.
- Use for Creation **server-side web app**.
- Right pik for the data intensiv real-time applicatin. - Ex:- Chat-app
- it use asynchronous programming.

# List down the mejer Benefits of Using Node.js?

- Open Source.
- Simple & Faster.
- Asynchronous.
- High Scalability.
- Single Threaded.
- No, Boffering.
- Cross Platform.

# What is the difference between Angular and Node.js ?

## Angular

- _OpenSource_ web application development framework
- Written in _TypeScript_.
- Used for Building _Single-page Client-side Web_ application.
- Anguler Itself is a web application _framework_.
- Ideal for Creation _Highle Active and Interactive web-apps_.

- helpful in splitting an app into _MVC Components_.
- Suitable for developing _real-time_ applications.

# Node.js

- _Cross-platform run time enveroment for application_.
- Written in _C,C++,javaScript_ Language.
- Used for Building _fast and Scalable Serve-side networking_ application.
- Node.js has many different frameworks like _Sails.js,Partial.js, and Express.js_
- Ideal for developing _small size_ Project.
- Helpful in generating database quaries.
- faster and Sche

# Why Node.js is a Single threaded?

- Node.js uses a single threaded model in order to support _async_ processing.
- With async Processing, and application can Perform better and is more scalables uder web loades.
- Node.js makes use of a single-threaded model approach rather then tupical thread-based inplementation.

# How to Node.js Work?

- Node.js is a virtual machine that uses javaScript as its Scripting language and runs on a v8 environment.
- it works on a single-threaded event loop and a non-blocking I/O which provides high rate as it can handle a higher number of concurrent requests.
- By making use of the 'HTTP' module, Node.js can run on any stan-alone web server.

# where Node.js can be used?

- Real-time web-applicatin.
- Network Application.
- Distributed System.
- General Purpose Application.

# How Many types Of API functions are there in Node.js?

- Asynchronous, non-blocking functions
- Synchronous, blocking functions

# what is difference between Asynchronous and Non-blocking ?

## Asynchronous

- Using these we can make Asynchronous HTTP requests that do **not wait for the server to respond**.
- These functions continue to respond to the reqest for which it has already received the server response.

## Non-blocking

- Non-blocking functions are used in regards with I/O operations.
- They immediately respond with whatever data is avalable and keeps on running as per the requests.

# What is pakage.json ?

- The pakage.json file in node.js is the heart of the entire application.
- it is a _Intruduction_ of node base project.
- it is basically the manifest file that contains te metadata of the project where we define the properties of a package.
- data store in object.

# What do you understad by Event-drivent Programming?

- In Node.js, event-driven programming means as soon as Node starts its server, it initiates its variables, declares functions and then waits for an event to occur. It is one of the reasons why Node.js is pretty fast compared to other similar technologies.
- it is programming approach that heavily makes use of **events for triggering various functions**.
- This approach mainly follows the _publish-subscribe pattern_.
-

# What is an Event loop in Node.js and how does it works?

- An event loop in Node.js hendels all the asynchronous calbacks in an application.
- This approach mainly follows the publish-subscribe pattern.
- pakage.json
- All callback function that comes through promises or mutation observer will go inside the microtask queue.
- [Event loop vidio](https://www.youtube.com/watch?v=gMtchRodC2I)

# i will add a IMG of event loop in feture

---

# Explain REPL in the context of Node.js? (node shell)

    - Read:- Reads the user's input , Parses it into javaScript data-structure and then stores it in the memory.
    - Eval:- Receives and evaluates the data structure.
    - Print:- Print the final result
    - Loop:- Loops the aprovided command until CTRL+C is pressed twice.

# What are the streams in Node.js?

- `stream.pipe()` the method used to take a readable and connect it to a writable stream.

- he Streams are the objects that facilitate you to **read data from a source and write data to a destination**. There are four types of streams in Node.js:

- Readable:- This stream is used for _reading operations_.
- Writable: This stream is used for _write operations_.
- Duplex:- _reading and write operations._
- Transform: it is a type of duplex stream where the output computes according to input.

---

# What is an error-first callback in Node.js?

- Error-First Callback in Node. js **is a function which either returns an error object or any successful data returned by the function**.

- The first argument in the function is reserved for the error object. If any error has occurred during the execution of the function, it will be returned by the first argument.

<img width="301" alt="image" src="https://user-images.githubusercontent.com/78966839/183675075-aaaedcaa-de2c-4dcc-98ae-46171e241876.png">

---

# What is the purpose of module.exports?

- Module exports are the instructions that tell Node. js which bits of code to export from a given file so that **other files are allowed to access the exported code**.


# What do you understand by reactor Pattern in Node.js?

- Reactor Pattern in Node.js is basically a concept of non-blocking i/o operaction.
- This pattrn provides a handler that is associated with i/o operaction.
- As soon as an i/o request is gentrated, it is then submitted to a demultiplexer.
- This demultiplexer is a notification interface which is capable of handling concurrency in non-blocking i/o module.
- It also helps in collecting each and every request in the form of an event and then place each event in a queue.
- Thus resulting  in the generation of the Event queue.

# what's the difference between 'front-end' and 'back-end' developer?

- ## Front-end
  - use make up and web languages like HTML,CSS,JAVASCRIPT
  - Based on asynchronous requests and AJAX.
  - Batter Accessibility.
  - clint side. SEO
  ## Bake-end
  - Uses programming and scripting languages like python,Ruby,perl,etc.
  - Based on server Architecture
  - Enhanced Security.
  - Used for Backup.

# What do you understand by callback hell?

- it typically contains mltiple nasted callback fuction fuctions which in turn make the code hard to read and debug.
- **A Callback is a function “A” that is passed to another function “B” as a parameter**.
- The function “B” executes the code “A” at some point. The invocation of “A” can be immediate, as in a synchronous callback, or, it can occur later as in an asynchronous callback.

<img width="250" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/73ab6420-4774-4757-a7b9-46c3f4e5651c">

# Explain the concept of middleware in Node.js?

- Middleware is a function receives the request and responce Objects.
- it update or modify the request and the response objects.

# Explain the concept of URL module.

- The URL modue is built-in module that helps in **splitting up the web address into a readable format**.

# Why node.js use google V8 engine?

- Google uses V8 as it is a chrome rentime engine that converts javaScript code into native machine code.
- it speeds up the application exexecution and response Process and give you a fast running applicaton.

# Explain the working of the control flow function.

- The control flow function is basically the code that is exicuted between the asynchronouus function calls.
  - The order of exicution must be controlled.
  - The required data nedds to be collected.
  - The concurrency must be limited
  - The next step of the program must be invoked.

# List down the tow agrument that async.queue take as input ?

- Task function
- Concurrency value

# Difference between spawn() and fok() methods in Node.js?

- Spawn() :- use to lunch a new process whith the provided set of commands.
- fork() :- it is a spacial instance of spawn() that executes a new instance of the V8 engine.

# What do you understand by global in objects in Node.js?

- Globals are the objects which are global in nature and are avilable in all the modules of the application.
- The global objects can be modules, functions, strings, object,etc.

# How assert works in Node.js ?

- Assert is use to write tests.
- it only provides feedback only when any of the running test cases fails.
- This module gives You a set of assertion tasks which are then used for testing inverants.
- it is basically used internally By node.js but using require('assert') code, it can be used in other applications as well.

# Difference bteween Authenticate and Authorize? 

- **Authenticate:** Verify the identity of a user.
- **Authorize:** Determine what actions or resources a user is allowed to access.

# what is JWT?

- JWT stands for JSON Web Token
- JWTs are used to securely transmit information between two parties as a JSON object.
-  They are commonly used for authentication and authorization in web applications.




# Define the concept of the text pyramid. Explain the process to implement then in terms of HTTP APIs.

- The test pyramid is basically a concept that is developed by mike cohn.
- The consept say that, You should have a higher mumber of low-level unit tests as compared to high-lavel end-to-end tests tat running through a GUI.
- In terms of HTTP APIs it may ne defined as 
   - A igher number of low-level usit tests for each module.
   - Lesser integration ests to test model interactions
   - Lesser acceptence tests for testing actual HTTP endpoint.

# Explain the puropse of Expressjs package?

- Expess.js is a framework built on top of node.js that faciltates the **management of the flow of data between server and routes in the server-dide application**.

- it is a lightweight and flexhle framwork that provides a wide range of features for web application.

# Explain the usege of buffer calss in Node.js ?

- uffer class in Node.js is used for storing the row data in a similar manner of an array of integers.
- But it corresponds to a raw memory allocation that is located outside the V8 heap.
- it is a global call that is easily accesible can be accessed in an application without importing a buffer module.
- Buffer calss is used becous pure javaScript in not compatible wtih binary data.

# How dose node.js handle the child threads?

- You can still make use of the child thread using spawn() for some spacific asynchronous I/O tasks.
- if You still want to use the threading concept in Your application you have to includ a module called childprocess explictly.


# What is use of NODE_ENV ?

- if the project is the production state, Node.js promotes the convention of making use of NODE_ENV variable to flage it.
- This helps in taking batter judgement during the development of the project.

# List down the vaious timing features of Node.js.

- setTimeout/clearTimeout
- setInterval/clearInterval
- setImmediate/cleareImmediate
- process.nextTrick

# Explain the concept of punycode in Node.js?

- punycode is an encoding syntax that is used for converting Unicode (UTF-8)  string of charaters into a basic ASCII string characters.
- it is importend as the hostnames can only understand the ASCII characters.
- Node.js version 0.6.2 onwords. it was bundled up with default node package.

# Diff btn Node.js and Ajax?
- **Node.js** is server side technolgy
- Required to develop the server software that are typically executed by the server instead of the web browser.

- **Ajex** is client-side technology
- Required for updating or madifying the webpage contents without having to refresh it.

# What do you understand by an event Emitter in Node.js?

- EventEmitter is node.js class that includes all the objects that are capable of emitting event.

<img width="237" alt="image" src="https://github.com/pattjoshi/interview-Q-A/assets/78966839/dfd09420-4a95-4176-a0e0-42e887382683">


# Explain the reason as to why Express 'app' and 'server' must be kept separate.

- Faster testing execution.
- it allows testing the API in-process without having to perform the network calls.
- Better Separation of conncerns and cleaner code.


# What is the use of middleware in Node.js?

- A middleware in the simple function that has the ability to handle incoming request and outbound response objects.

- middleware is used primarily for the following tasks: 
  - Execution of code (of any type)
  - Updation of request and response objects
  - completion of request-response interactions
  - calling the next middleware.

# why do we use express.js instead of node.js in express

- Express is built on top of Node, so yes, Express adds more features while building apps. 
-  Node is just a Javascript environment with libraries to make it easy to write software, whereas Express extends Node specifically to add middleware, routing.
-   Express.js makes the development process more straightforward and efficient by providing higher-level abstractions for common web application tasks while still leveraging the power and flexibility of Node.js underneath.


---
# [Yotub socse](https://www.youtube.com/watch?v=6WYEmUVhiwQ) 👆
# [youtb](https://www.youtube.com/watch?v=7npkRw7gMRA&t=155s)

---

 















