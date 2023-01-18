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










