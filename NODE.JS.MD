# NODE.JS interview question

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

<img width="301" alt="image" src="https://user-images.githubusercontent.com/78966839/183675075-aaaedcaa-de2c-4dcc-98ae-46171e241876.png">


