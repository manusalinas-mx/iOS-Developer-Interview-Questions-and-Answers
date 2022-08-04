# iOS Developer Interview Questions for all Senioritis levels
###### The most complete guide to help those looking to hire a developer for iOS.
![top-10-ios-developer-interview-questions](https://user-images.githubusercontent.com/110424672/182920874-03ae4ffc-7ec4-44d9-ad16-1170d924ac70.png)

---


### **Explain what is `Grand Central Dispatch` (GCD) in iOS?**

  Grand Central Dispatch (**GCD**) is a low-level API that allows users to run concurrent tasks(run simultaneously). It also manages threads in the background. Apple’s solution is to build concurrency and parallelism into iOS applications so different tasks can run concurrently in the background without affecting the main thread.
  
### **What is the difference between `Synchronous` & `Asynchronous` task?**
     - **Synchronous**: waits until the task have completed 
     - **Asynchronous**: completes a task in the background and can notify you when complete


### **What is made up of `NSError` object?**

There are three parts of **NSError** object a `domain`, an `error code`, and a `user info dictionary`. The domain is a string that identifies what categories of errors this error is coming from.


### **What is `Enum` or `Enumerations`?**

**Enum** is a type that basically contains a group of related values in the same umbrella


### **What’s the difference between the `frame` and the `bounds`?**
  - **The bounds** of a UIView is the rectangle, expressed as a location (x,y) and size (width, height) _relative to its own coordinate system (0,0)_. 
  - **The frame** of a UIView is the rectangle, expressed as a location (x,y) and size (width, height) _relative to the superview it is contained within_.


### **Why is design pattern very important?**

Design patterns are reusable solutions to common problems in software design. They’re templates designed to help you write code that’s easy to understand and reuse.
  - **Most Common:**
    - **Creational**: Singleton.
    - **Structural**: Decorator, Adapter, Facade.
    - **Behavioral**: Observer


### **What is Singleton Pattern?**

The **Singleton** design pattern ensures that only one instance exists for a given class and that there’s a global access point to that instance.



### **What is Facade Design Pattern?**

The **Facade** design pattern provides a single interface to a complex subsystem. Instead of exposing the user to a set of classes and their APIs, you only expose one simple unified API.



### **What is Decorator Design Pattern?**

The **Decorator** pattern dynamically adds behaviors and responsibilities to an object without modifying its code. It’s an alternative to subclassing where you modify a class’s behavior by wrapping it with another object.

In **Objective-C** there are two very common implementations of this pattern: **Category** and **Delegation**. 

In **Swift** there are also two very common implementations of this pattern: **Extensions** and **Delegation**.



### **What is Adapter Pattern?**

An **Adapter** allows classes with incompatible interfaces to work together. It wraps itself around an object and exposes a standard interface to interact with that object.



### **What is Observer Pattern?**

In the **Observer** pattern, one object notifies other objects of any state changes.

**Cocoa** implements the observer pattern in two ways: **Notifications** and **Key-Value Observing** (KVO).



### **Explain MVC**

  - **Models** — responsible for the domain data or a data access layer which manipulates the data, think of ‘Person’ or ‘PersonDataProvider’ classes.
  - **Views** — responsible for the presentation layer (GUI), for iOS environment think of everything starting with ‘UI’ prefix.
  - **Controller/Presenter/ViewModel** — the glue or the mediator between the Model and the View, in general responsible for altering the Model by reacting to the user’s actions performed on the View and updating the View with changes from the Model.



### **Explain `generics` in Swift?**

**Generics** create code that does not get specific about underlying data types. **Generics** allow us to know what type it is going to contain.



### **Explain `lazy` in Swift?**

An initial value of the **lazy** stored properties is calculated only when the property is called for the first time.


### **Explain what is `defer`?**

**defer** keyword which provides a block of code that will be executed in the case when execution is leaving the current scope.


### **How to pass data between view controllers?**

There are **3 ways** to pass data between view controllers.

1. **Segue**, in prepareForSegue method (Forward)
2. **Delegate** (Backward)
3. **Setting variable directly** (Forward)


### **What is Concurrency?**

**Concurrency** is dividing up the execution paths of your program so that they are possibly running at the same time. 

The common terminology: **process**, **thread**, **multithreading**, **and** **others**. 

Terminology:
- **Process**, An instance of an executing app
- **Thread**, Path of execution for code
- **Multithreading**, Multiple threads or multiple paths of execution running at the same time.
- **Concurrency**, Execute multiple tasks at the same time in a scalable manner.
- **Queues**, Queues are lightweight data structures that manage objects in the order of First-in, First-out (FIFO).
- **Synchronous** vs **Asynchronous** tasks


### **Readers-Writers**

Multiple threads reading at the same time while there should be only one thread writing. The solution to the problem is a **readers-writers** lock which allows concurrent read-only access and an exclusive write access.

Terminology:
- **Race Condition** A race condition occurs when two or more threads can access shared data and they try to change it at the same time.
- **Deadlock** A deadlock occurs when two or sometimes more tasks wait for the other to finish, and neither ever does.
- **Readers-Writers problem** Multiple threads reading at the same time while there should be only one thread writing.
- **Readers-writer lock** Such a lock allows concurrent read-only access to the shared resource while write operations require exclusive access.
- **Dispatch Barrier Block** Dispatch barrier blocks create a serial-style bottleneck when working with concurrent queues.


### **NSOperation — NSOperationQueue — NSBlockOperation**
- **NSOperation** adds a little extra overhead compared to GCD, but we can add dependency among various operations and re-use, cancel or suspend them.
- **NSOperationQueue**, It allows a pool of threads to be created and used to execute NSOperations in parallel. Operation queues aren’t part of GCD.
- **NSBlockOperation** allows you to create an NSOperation from one or more closures. NSBlockOperations can have multiple blocks, that run concurrently.


### **KVC — KVO**
- **KVC** adds stands for **_Key-Value Coding_**. It’s a mechanism by which an object’s properties can be accessed using string’s at runtime rather than having to statically know the property names at development time.
- **KVO** stands for **_Key-Value Observing_** and allows a controller or class to observe changes to a property value. In KVO, an object can ask to be notified of any changes to a specific property, whenever that property changes value, the observer is automatically notified.


### **Explain `Guard` statement**
There are 3 big benefits to guard statement.

1. Avoids the pyramid of doom, as others have mentioned — lots of annoying if let statements nested inside each other moving further and further to the right. 
2. Provides an early exit out of the function using `break` or using `return`.
3. **guard** statement is another way to safely **unwrap** **optionals**.


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****


### ****
