# Object Orianted Programming Interviev qus and Ans

# [Object Orianted Programming Love Babber](https://whimsical.com/object-oriented-programming-cheatsheet-by-love-babbar-YbSgLatbWQ4R5paV7EgqFw)


---

# What is OOP?

- Object-oriented programming (OOP) is about crating objects that contain both data and function.

- OOP provides a clear structure for the programs.

- OOP helps to keep the java code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug.


# [Object Oriented Programming With Real world Example](https://fdhgjhjhukj.medium.com/object-oriented-programming-with-real-world-example-63f69f917d62)

Basically why we are write coding ,to solve our real world problem right. In OOP a logic is right base on the object with this features
1.abstraction
2.encapsulation
3.inheritance
4.polymorphism

- There are a lot of Car,bike,ATM and coffee machine.and there brands and name also different. In OOP those are called object .

- Objects logic are done by classes and Class is a blue print of Object. for example ,by phone we can call,Bluetooth ,take photo etc. those every logic will be divide as classes.

--- 

# [Why Study Oops ?](https://www.c-sharpcorner.com/forums/why-we-need-oops-in-programming-language)

- **Why we need OOPs in Programming language?**

- OOP helps to keep the JAVA code DRY "Don't Repeat Yourself"
- OOPs provides code reusability which reduce the duplication of code because once you have duplicate code, you have make changes everywhere which leads to performance.
- Code can be changed anytime as per our requirement  in the application, OOPs makes it easier.


#  Disadvantages of Object-Oriented Programming (OOP)

- **Larger program size:** Object-oriented programs typically involve **more lines of code than procedural programs.**

- **Slower programs:** Object-oriented programs are typically slower than procedure-based programs, as they typically require **more instructions to be executed.**

- **Not suitable for all types of problems:** The problems like functional-programming style, logic-programming style, or procedure-based programming style, and applying object-oriented programming in those situations will not result in efficient programs.


# when we say X is oop language. what dose it mean ?

- If a language is designed with the facilities specifically to support object-oriented programming having 4 features that is abstraction, encapsulation, inheritance, polymorphism then it is an Object-oriented programming language.
-  It's the code that is object-oriented not the language.

---
# Piller of oops
---
# [What is class?]()

- It is a basic concept of Object-Oriented Programming which revolve around the real-life entities. 

- Class are a blueprint of Object.

```
class car {  
    color;  
    Model;  
  }
```
# Structure vs class

<img width="750" alt="image" src="https://user-images.githubusercontent.com/78966839/212488323-65b4c801-26b9-4a08-8800-8c6dba7383d0.png">

# Similarity between structure and class?

- Both are container types, meaning that they contain other types as members.
- Both have members, which can include constructors, methods, properties, fields, constants, enumerations, events, and event handlers.
- Both can implement interfaces.
- Both can have shared constructors, with or without parameters.

- Both can expose a default property, provided that property takes at least one parameter.

# when to use structure over class?
- If the size of the instance is below 16 bytes.
- Structures are preferred for object design for data storage like array.

# [Access Modifiers](https://www.javatpoint.com/access-modifiers)

- The access modifiers in Java specifies the accessibility or scope of a method, constructor, or class

- **Private:** The access level of a private modifier is **only within the class.** It cannot be accessed from outside the class.

- **Default:** The access level of a default modifier is **only within the package.** It cannot be accessed from outside the package. If you do not specify any access level, it will be the default.

- **Protected:** The access level of a protected modifier is within the **package and outside the package through child class.** If you do not make the child class, it cannot be accessed from outside the package.

- **Public:** The access level of a public modifier is **everywhere.** It can be accessed from within the class, outside the class, within the package and outside the package.

<img width="530" alt="image" src="https://user-images.githubusercontent.com/78966839/213174782-7c86c83b-0441-4d4f-95c2-8f2858c98c49.png">

# Member functions

Member functions are the functions, which have their declaration inside the class definition and works on the data members of the class.

- The definition of member functions can be inside or outside the definition of class.

- If the member function is defined inside the class definition it can be defined directly, but if its defined outside the class, then we have to use the scope resolution :: operator along with class name alng with function name.

# [Constructors](https://www.javatpoint.com/java-constructor)

- A constructor in Java is a **special method**  that is invoked automatically at the time of object creation.

- Note that the constructor name must match the class name, and it cannot have a return type (like void).

## Rules for creating Java constructor

- Constructor name must be the same as its class name
- A Constructor must have no explicit return type
- A Java constructor cannot be abstract, static, final, and synchronized

# Default Constructor

- A constructor is called "Default Constructor" when it doesn't have any parameter.

- If there is no constructor in a class, compiler automatically creates a default constructor.

### Q) What is the purpose of a default constructor?

- The default constructor is used to provide the default values to the object like 0, null, etc., depending on the type.

# Parameterized Constructor

- A constructor which has a specific number of parameters is called a parameterized constructor.

### Why use the parameterized constructor?

- The parameterized constructor is used to provide different values to distinct objects. However, you can provide the same values also.

# Constructor Overloading in Java

- Constructor Overloading in Java **Same name but Different parameter**

# How constructors are different from a normal member function?

- A constructor is different from normal functions in following ways:

- Constructor has same name as the class itself

- Constructors don’t have return type

- A constructor is automatically called when an object is created.

- If we do not specify a constructor, C++ compiler generates a default constructor for us (expects no parameters and has an empty body).

<img width="536" alt="image" src="https://user-images.githubusercontent.com/78966839/213197340-cdb9f691-9f9a-4706-9fe5-ae607d5f1bbc.png">

# Java Copy Constructor
- There is no copy constructor in Java. However, we can copy the values from one object to another like copy constructor in C++.

- There are many ways to copy the values of one object into another in Java. They are:

     - By constructor
     - By assigning the values of one object into another
     - By clone() method of Object class


# Can we have more then one constructer in a class

- Yes, a class can have multiple constructors. These constructors can have different parameters, allowing for multiple ways to initialize an object of the class. They are often called "overloaded constructors."


# [What is the destructor / garbage collector?](https://www.javatpoint.com/javadestructor#:~:text=What%20is%20the%20destructor%20in,memory%20occupied%20by%20the%20object.)

- It is a special method that automatically gets called when an object is no longer used.

- **there is no concept of destructor in Java.** In place of the destructor, Java provides the **garbage collector** that works the same as the destructor.

-  When an object completes its life-cycle the garbage collector deletes that object and deallocates or releases the memory occupied by the object.


# [What is an object in Java](https://www.javatpoint.com/object-and-class-in-java)

- An object is a real-world entity.
- An object is an instance of a class.
- An object is a runtime entity.
- The object is an entity which has state and behavior.
- The object is an instance of a class.


# [Difference between object and class](https://www.javatpoint.com/difference-between-object-and-class)

<img width="531" alt="image" src="https://user-images.githubusercontent.com/78966839/213239852-f9157f9d-e532-434f-8113-2a82323e0079.png">


# [Real Life Examples of Object Oriented Programming](https://www.c-sharpcorner.com/blogs/real-life-examples-of-object-oriented-programming1)


# Important Keywords

# [wat is the use of a static keyword](https://www.youth4work.com/Talent/Core-Java/Forum/119567-wat-is-the-use-of-a-static-keyword)

- The static keyword belongs to the class than an instance of the class.
- The static keyword in Java is used for memory management mainly.
- The static can be:
    1) Variable (also known as a class variable)
    2) Method (also known as a class method)
    3) Block
    4) Nested class
- static methods can be called without creating an object of the class.
- A static variable is one that's associated with a class, not instance (object) of that class.
- They are initialized only once , at the start of the execution .

# What are virtual keywords?

- The virtual keyword is used to modify a method, property, indexer, or event declaration and allow for it to be overridden in a derived class.

- The virtual keyword is not used in Java.

# [why virtual keyword is used](https://www.codeproject.com/Questions/270054/why-virtual-keyword-is-used)

- Marking a method as virtual means you can override it in derived classes, but you don't have to.
-  If you mark a method as abstract, you are subsequently forced by the compiler to override it in any derived classes.

# [abstract keyword](https://www.tutorialspoint.com/abstract-keyword-in-Java)

- 'abstract' keyword is used to declare the method or a class as abstract.

- Abstract classes may or may not contain abstract methods, i.e., methods without a body ( public void get(); )

- But, if a class has at least one abstract method, then the class must be declared abstract.

- **If a class is declared abstract, it cannot be instantiated.**

- To use an abstract class, you have to inherit it from another class, provide implementations for the abstract methods in it.

- If you inherit an abstract class, you have to provide implementations to all the abstract methods in it.

# [Final Keyword](https://www.javatpoint.com/final-keyword)

- The final keyword in java is **used to restrict the user.**
- Final can be:
    - variable
    - method
    - class
- If we declare a variable as final then we can not change it value.
- If we declare a method as final then we can not override it.
- If we declare a class as final then we can not inherit it.

# [this keyword](https://www.javatpoint.com/this-keyword)

- this keyword. In Java,  **reference variable that refers to the current object.**

<img width="440" alt="image" src="https://user-images.githubusercontent.com/78966839/214581793-c61eb397-18c0-47e5-8f99-53eb8b5d55a1.png">

# [Java new Keyword](https://www.javatpoint.com/new-keyword-in-java)

- It is used to create the object.
- It allocates the memory at runtime.
- All objects occupy memory in the heap area.
- It invokes the object constructor.
- It requires a single, postfix argument to call the constructor


# [const keyword](https://stackoverflow.com/questions/7428358/why-const-keyword-is-not-used-in-java)
- there is no concept of const keyword in java.
- **why**     Java allows us to declare constants by using final keyword

# [Super keyword](https://www.javatpoint.com/super-keyword)

- super keyword in Java is a reference **refer immediate parent class object.**

- super can be used to invoke immediate parent class method.

- super() can be used to invoke immediate parent class constructor.

# [Polymorphism](https://www.javatpoint.com/runtime-polymorphism-in-java)

- it is a combinaton of 2 towd Poly and morphism 
- Poly means :- many  and morphism :- forms = manyforms
- whose meaning is **Same object having different behavior**

- **Ex**:- let us consider i as an example, In my home, office and friend-circle i act as different. Hear,object is same that is  I but behaviour is different.

- There are two types of polymorphism in Java: **compile-time polymorphism and runtime polymorphism**

# Need

- We can perform polymorphism in java by method overloading and method overriding.

# Overloading

- **having the same name but different in number  of parameter.**

- we can overload:

   - methods,
  - constructors, and
   - indexed properties

# Compile-time polymorphism
- Compile-time polymorphism is obtained through method overloading.

- Since this process is executed during compile time, that's why it is known as Compile-Time Polymorphism.

# Operators that cannot be overloaded in C++
- In C++ we can overload some operators like +, -, [], -> etc. But we cannot overload any operators in it. Some of the operators cannot be overloaded. These operators are like below

    - ? “.” Member access or dot operator
    - ? “? : ” Ternary or conditional operator
    - ? “::” Scope resolution operator
    - ? “.*” Pointer to member operator
    - ? “sizeof” The object size operator
    - ? “typeid” Object type operator
- These operators cannot be overloaded because if we overload them it will make serious programming issues.

- For an example the sizeof operator returns the size of the object or datatype as an operand. This is evaluated by the compiler. It cannot be evaluated during runtime. So we cannot overload it.

# [Overriding](https://www.javatpoint.com/method-overriding-in-java)

- If subclass (child class) has the same method as declared in the parent class, it is known as method overriding in Java.
- Method overriding is used to provide the specific implementation of a method which is already provided by its superclass.
- Method overriding is used for runtime polymorphism

# Functions that cannot be overloaded in C++
1) Function declarations that differ only in the return type.
2) Member function declarations with the same name and the name parameter-type-list cannot be overloaded if any of them is a static member function declaration.
3) Parameter declarations that differ only in a pointer * versus an array [] are equivalent.
4) Parameter declarations that differ only in that one is a function type and the other is a pointer to the same function type are equivalent. 
5) Parameter declarations that differ only in the presence or absence of const and/or volatile are equivalent. That is, the const and volatile type-specifiers for each parameter type are ignored when determining which function is being declared, defined, or called.

# [Runtime polymorphism](https://www.javatpoint.com/runtime-polymorphism-in-java)

- Runtime polymorphism, also known as the Dynamic Method Dispatch, is a process that resolves a call to an overridden method at runtime. The process involves the use of the reference variable of a superclass to call for an overridden method

## 9) What Does Derived Class Mean?
- A derived class is a class created or derived from another existing class. The existing class from which the derived class is created through the process of inheritance is known as a base class or superclass.

- Derived classes are used for augmenting the functionality of base class by adding or modifying the properties and methods to suit the requirements of the specialization necessary for derived class. This allows for defining virtual methods that form the means to implement polymorphism, which allows a group of objects to work in uniform manner. Thus, the inherent advantages of inheritance and polymorphism like code reuse, faster development, easy maintenance, etc., are realized.

- A derived class is also known as subclass or child class.

## 10) Can Virtual Functions be Private in C++?
- A virtual function can be private as C++ has access control, but not visibility control. As mentioned virtual functions can be overridden by the derived class but under all circumstances will only be called within the base class.

# [inline virtual functions](https://stackoverflow.com/questions/733737/are-inline-virtual-functions-really-a-non-sense)

# Abstraction
- A class which is declared with the abstract keyword is known as an abstract class in Java. It can have abstract and non-abstract methods.
- Abstraction in Java
- Abstraction is a process of hiding the implementation details and showing only functionality to the user.
- Another way, it shows only essential things to the user and hides the internal details, for example, sending SMS where you type the text and send the message. You don't know the internal processing about the message delivery.

# Pure Virtual Functions
- A pure virtual function (or abstract function) in C++ is a virtual function for which we can have implementation, But we must override that function in the derived class, otherwise the derived class will also become abstract class.
- https://www.geeksforgeeks.org/pure-virtual-functions-and-abstract-classes/

# [pure virtual destructor](https://stackoverflow.com/questions/1219607/why-do-we-need-a-pure-virtual-destructor-in-c)

---

# [Inheritence](https://www.javatpoint.com/inheritance-in-java)

- Inheritance in Java is a mechanism in which **one object acquires all the properties and behaviors of a parent object.**

- The idea behind inheritance in Java is that you can create **new classes that are built upon existing classes.**

- Inheritance represents the **IS-A relationship** which is also known as a **parent-child relationship.**

   - subclass (child) - the class that inherits from another class
   - superclass (parent) - the class being inherited from


## Sub Class/Child Class:
- Subclass is a class which inherits the other class. 
- It is also called a derived class, extended class, or child class.


## Super Class/Parent Class:
- Superclass is the class from where a subclass inherits the features. It is also called a base class or a parent class.

## Reusability:
- As the name specifies, reusability is a mechanism which facilitates you to reuse the fields and methods of the existing class when you create a new class. You can use the same fields and methods already defined in the previous class.


# Why/ need of inheritance?
- For Method Overriding (so runtime polymorphism can be achieved).
- For Code Reusability.
- Inheritance is used to declare characteristics of classes inheriting it,without giving its implementation.
- It is one of the most important concept of OOPS.

# can oop exist without inheritance?(NOT DONE)

---
# [Type of Inheritence](https://www.javatpoint.com/inheritance-in-java)

## Single Inheritance

- When a class inherits another class, it is known as a single inheritance.

## Multilevel Inheritance

- **includes the involvement of at least two or more than two classes**

- When there is a chain of inheritance, it is known as multilevel inheritance. 

## Hierarchical Inheritance

- When **two or more classes inherits a single class,** it is known as hierarchical inheritance

- Single Base class multiple Derive class.

## Hybrid Inheritance

- **hybrid inheritance is the composition of two or more types of inheritance.**

## Multiple inheritence

- In this type of inheritance a single sub class may inherit from two or more than two super classes.

- **java dose not have Multiple inheritence.it have Interfaces.**

# The Real world example of multiple inheritance
- Imagine a Classes called as “MARUTI” and “SUZUKI” 
- when both collab made a Child Car called as “Ertiga” .So Ertiga have characterstic of Maruti as well as Suzuki .
- Child Class (Ertiga) acquared Properties of 2 Parent Classes / Or can say Inherit Properties from Multiple Parents so Its a Multiple Inheritance 

# Limitation of inheritance?
- The inheritance relationship is a, tightly coupled relationship , there will be tight bonding between parent and child. If we change code of parent class it will get affects to the all the child classes which is inheriting the parent code.

## What is sealed modifier?
- sealed is a keyword which is used to seal a class or function and prevent it to get inherited from any other classes.
- In other words, a sealed class cannot be inherited. similarly function can't be used by the other class.

## [How can we call a base/PARENT method without creating instance](https://stackoverflow.com/questions/10173827/how-to-invoke-parent-class-method-without-creating-object-of-it)


# Why multiple inheritance is not supported in java?

- To reduce the complexity and simplify the language, multiple inheritance is not supported in java

- But we can achive multiple inheritance useing Interfaces.

<img width="563" alt="image" src="https://user-images.githubusercontent.com/78966839/214851829-60f36a54-5de2-44cc-b1a3-bf189acbe561.png">

# [DIFFERENCE BETWEEN NEW AND OVERRIDE](https://stackoverflow.com/questions/6576206/what-is-the-difference-between-the-override-and-new-keywords-in-c)

- The difference between override and new is that override extend the method of base class with new definition but new hides the method of base class.

# [What all is inherited from parent class](https://www.geeksforgeeks.org/g-fact-4/)

Following are the things that a derived class inherits from its parent. 
1) Every data member that is defined in the parent class 
2) Every ordinary member function of the parent class 
3) The same initial data layout as of the base class. 

Following are the properties which a derived class doesn’t inherit from its parent class : 
1) The base class’s constructors and destructor. 
2) The base class’s friend functions.
3) Overloaded operators of the base class.


# Inline function
- C++ provides an inline functions to reduce the function call overhead.
- Inline function is a function that is expanded in line when it is called. 

# friend class
- A friend class can access private and protected members of other classes in which it is declared as a friend. 

# Friend Function
- Like a friend class, a friend function can be granted special access to private and protected members of a class in C++.
- 
# Nested class 
- Writing a class within another is allowed in Java. 
- The class written within is called the nested class

# Local class
- Local classes are classes that are defined in a block, which is a group of zero or more statements between balanced braces.


# [Difference between Inheritance and Polymorphism](https://www.geeksforgeeks.org/difference-between-inheritance-and-polymorphism/)

<img width="491" alt="image" src="https://user-images.githubusercontent.com/78966839/214883002-9592ce84-376b-44f7-8680-b821ff0d9bd5.png">

# [Aggregation, Composition, Generalization](https://javapapers.com/oops/association-aggregation-composition-abstraction-generalization-realization-dependency/)

---

# [Encapsulation in Java](https://www.javatpoint.com/encapsulation)

- Encapsulation in Java is a process of wrapping code and data together into a single unit.

- for example, a capsule which is mixed of several medicines.

- The Java Bean class is the example of a fully encapsulated class.

# Need  

- In Java, encapsulation helps us to **keep related fields and methods together, which makes our code cleaner and easy to read.**

- The encapsulate class is **easy to test.** So, it is better for unit testing.

# Advantage

- It is a way to achieve **data hiding** in Java because other class will not be able to access the data through the private data members.

- The class will maintain its data members and methods as read-only.

- Data hiding prevents the user from the complex implementations in the code.


- The variables of the class can be read-only or write-only as per the programmer's requirement.

# Encapsulation in Java can be achieved by:

- Encapsulation is achieved in java language by class concept.

- Declaring the variables of a class as private.

# [Encapsulation code/implimentation example](https://beginnersbook.com/2013/05/encapsulation-in-java/)


# [Real world example of encapsulation](https://www.sitesbay.com/java/java-encapsulation)

---

# Abstraction

- hiding the Internal details and shows only the required one to user

- We cannot create an instance of Abstract Class.

- It reduces the duplication of code.

# Whent to use ? (NOT DONE)

# [How to achieve abstration using abstract class and interface](https://www.javatpoint.com/how-to-achieve-abstraction-in-java)

## Abstration vs Encapsulation

 ![image](https://user-images.githubusercontent.com/102239780/214894598-52d3ea1e-095e-4539-8b06-5aa92400f794.png)

# Difference between Abstract class and interface

 ![image](https://user-images.githubusercontent.com/102239780/214895627-ffdda30a-4bcd-4981-812b-57ec8c8e6678.png)


# [Static Binding and Dynamic Binding](https://www.javatpoint.com/static-binding-and-dynamic-binding)
 ![image](https://user-images.githubusercontent.com/102239780/214897130-f02a9d26-4a34-41fa-b87a-0d328fb8ef4d.png)

# Message Passing
- Object-oriented programming as a programming paradigm is based on objects. Objects are a representation of real-world and objects communicate with each other via messages.

- When two or more objects communicate with each other that means that those objects are sending and receiving messages. This is often called method calling.

- Sending object (Object A) knows which method of receiving object (Object B) is being called, so it knows more details than needed. With this, we create code which is not loosely coupled. Changes in one object will lead to changes in others too.















