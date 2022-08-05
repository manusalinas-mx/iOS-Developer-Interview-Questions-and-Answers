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

- Terminology:
  - **Process**, An instance of an executing app
  - **Thread**, Path of execution for code
  - **Multithreading**, Multiple threads or multiple paths of execution running at the same time.
  - **Concurrency**, Execute multiple tasks at the same time in a scalable manner.
  - **Queues**, Queues are lightweight data structures that manage objects in the order of First-in, First-out (FIFO).
  - **Synchronous** vs **Asynchronous** tasks


### **Readers-Writers**

Multiple threads reading at the same time while there should be only one thread writing. The solution to the problem is a **readers-writers** lock which allows concurrent read-only access and an exclusive write access.

- Terminology:
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


### **What is the difference Non-Escaping and Escaping Closures?**

- The lifecycle of a **non-escaping closure** is simple:
  - Pass a closure into a function
  - The function runs the closure (or not)
  - The function returns

**Escaping closure** means, inside the function, you can still run the closure (or not); the extra bit of the closure is stored someplace that will outlive the function. 

- There are several ways to have a closure escape its containing function:
  - **Asynchronous execution**: If you execute the closure asynchronously on a dispatch queue, the queue will hold onto the closure for you. You have no idea when the closure will be executed and there’s no guarantee it will complete before the function returns.
  - **Storage**: Storing the closure to a global variable, property, or any other bit of storage that lives on past the function call means the closure has also escaped.


### **Explain `[weak self]` and `[unowned self]`?**

- **unowned** (_non-strong reference_) does the same as **weak** with one exception: The variable will not become `nil` and must not be `optional`.    You can use it:
  - Every time used with **non-optional** types
  - Every time used with **let**

- **weak self** you get to handle the case that it might be `nil` inside the closure at some point and therefore the variable must be an `optional`.  You can use it:
  - In an **asynchronous** network request, is in a view controller where that request is used to populate the view.


### **What is ARC?**

_Automatic Reference Counting_. This means that it **only** frees up memory for objects when there are **zero strong** references/ to them.


### **Difference between `SceneDelegate` and `AppDelegate`**

- **AppDelegate** is part of the UIKit framework. 
- The **SceneDelegate** takes over this roles from the app delegate with **iOS 13**. The concept of a window is replaced by that of a scene. Multiple scenes allow us to build multi-window apps on **iOS** and **iPadOS**.


### **Why is everything in a `do-catch` block?**

In Swift, errors are thrown and handled inside of **do-catch blocks**. 

This allows us to customize our error handling and perform specific actions based on the error. With a `do-catch` statement, we can use **try**. This allows us to check meaningful errors.


### **Explain Swift Package Manager (SPM)**

The **Swift Package Manager** addresses the problem of dependency hell that can happen when using many third party libraries. The Swift Package Manager only supports using the **master branch** and now supports packages with **Swift**, **C**, **C++** and **Objective-C**.


### **How is an `inout` parameter different from a `regular` parameter?**

A **Inout** passes by _reference_ while a **regular** parameter passes by _value_.


### **Explain `View Controller Lifecycle` events order?**

- There are a few different lifecycle events:
  - **loadView** 
    - Creates the view that the controller manages. It’s only called when the view controller is created and only when done programatically. It is responsible for making the view property exist in the first place.
  - **viewDidLoad** 
    - Called after the controller’s view is loaded into memory. It’s only called when the view is created.
  - **viewWillAppear** 
    - It’s called whenever the view is presented on the screen. In this step the view has bounds defined but the orientation is not applied.
  - **viewWillLayoutSubviews**
    - Called to notify the view controller that its view is about to layout its subviews. This method is called every time the frame changes
  - **viewDidLayoutSubviews**
    - Called to notify the view controller that its view has just laid out its subviews. Make additional changes here after the view lays out its subviews.
  - **viewDidAppear**
    - Notifies the view controller that its view was added to a view hierarchy.
  - **viewWillDisappear**
    - Before the transition to the next view controller happens and the origin view controller gets removed from screen, this method gets called.
  - **viewDidDisappear**
    - After a view controller gets removed from the screen, this method gets called. You usually override this method to stop tasks that are should not run while a view controller is not on screen.
  - **viewWillTransition(to:with:)**
    - When the interface orientation changes, UIKit calls this method on the window’s root view controller before the size changes are about to be made. The root view controller then notifies its child view controllers, propagating the message throughout the view controller hierarchy.


### **What is `Class`?**

A **class** defines an object and how it works. In this way, a **class** is like a blueprint of an object.

### **What is `Object`?**

An **object** is an instance of a **class**.


### **When and why do we use an `object` as opposed to a `struct`?**

**Structs** are value types. **Classes** (_Objects_) are reference types.



### **What are the `states` of an iOS App?**

1. **Non-running** — The app is not running.
2. **Inactive** — The app is running in the foreground, but not receiving events. An iOS app can be placed into an inactive state, for example, when a call or SMS message is received.
3. **Active** — The app is running in the foreground, and receiving events.
4. **Background** — The app is running in the background, and executing code.
5. **Suspended** — The app is in the background, but no code is being executed.


### **What is `DispatchGroup`?**

The most basic answer: If we need to wait on a couple of **asynchronous** or **synchronous** operations before proceeding, we can use **DispatchGroup**.

### **Where do we use `Dependency Injection`?**

We use a **storyboard** or **xib** in our iOS app, then we created **IBOutlets**. **IBOutlet** is a property related to a view. These are injected into the view controller when it is instantiated, which is essentially a form of **Dependency Injection**.

- There are forms of dependency injection: 
  - constructor injection
  - property injection
  - method injection


### **Please explain types of notifications**

- There are 2 type of notifications:
  - **Remote notification**
    - requires connection to a server.  
  - **Local notification** 
    - doesn't require server connection. Local notifications happen on device.


### **What kind of `hight order functions` can we use on collection types?**

- **map(_:):** 
  - Returns an array of results after transforming each element in the sequence using the provided closure.
- **filter(_:):** 
  - Returns an array of elements that satisfy the provided closure predicate.
- **reduce(_:_:):** 
  - Returns a single value by combining each element in the sequence using the provided closure.
- **sorted(by:):** 
  - Returns an array of the elements in the sequence sorted based on the provided closure predicate.


### **Explain `Bridging Headers` in iOS project**

**Bridging Headers** allow us to include `Objective-C` files with our `Swift` files.


### **What is `Hashable`?**

**Hashable** allows us to use our objects as keys in a dictionary. 

So we can make our custom types that can be compared for its equality using it’s `hashValue`


### **How many different ways to pass data in Swift?**

There are many different ways such as **Delegate**, **KVO**, **Segue**, **NSNotification**, **Target-Action** and **Callbacks**.


### **What is the difference `Delegates` and `Callbacks`?**

The difference between **delegates** and **callbacks** is that...
- with **delegates**, the NetworkService is telling the delegate “There is something changed.” 
- With **callbacks**, the delegate is observing the NetworkService.


### **What is Pointer?**

A **pointer** is a direct reference to a memory address. **Pointers** remove a layer of abstraction and let you see how that value is stored.


### **What is the difference between `try?` and `try!` ?**

- **try?** allows us to ignore our error to become **nil**. 
- We use **try!** it for our function to never encounter an error.


### **Why do we use `availability` attributes?**

 **Availability Attributes** lets us to support previous version iOS.


### **What is `Encapsulation`?**

**Encapsulation** is an object-oriented design principles and hides the internal states and functionality of objects. That means objects keep their state information **private**.


### **How could we get `device token`?**

1. we must show the user’s permission screen, after we can register for remote notifications.
2. If previous step go well, the system will provide **device token**.

> **_Note:_** If we uninstall or reinstall the app, the device token would change.


### **Explain differences between `service extension` and `content extension`**

- The **service extension** lets us the chance to change content in the notification before it is presented. 
- The **content extension** gives us the tools, we have in an app to design the notification


### **What is `Instruments`?**

**Instruments** is a powerful performance tuning tool to analyze that _performance, memory footprint, smooth animation, energy usage, leaks_ and _file/network activity_.


### **What is `Deep Linking`?**

**Deep linking** is a way to pass data to your application from any platform like, _website_ or _any other application_. By tapping once on link, you can pass necessary data to your application.


### **What is `Optional Binding`?**

We are going to **take optional** value and we are going **to bind it non optional** constant. We used `**If let**` structure or `**Guard**` statement.


### **Explain `Polymorphism`**

**Polymorphism** is the ability of a class instance to be substituted by a class instance of one of its subclasses.


### **Explain `In-app Purchase products and subscriptions`**

- **Consumable products:** can be purchased more than once and used items would have to re-purchase.
- **Non-consumable products:** user would be able to restore this functionality in the future, should they need to reinstall the app for any reason. We can also add subscriptions to our app.
- **Non-Renewing Subscription:** Used for a certain amount of time and certain content.
- **Auto-Renewing Subscription:** Used for recurring monthly subscriptions.


### **What is `Protocol`?**

A **protocol** defines a blueprint of _methods_, _properties_ and _other_ requirements that suit a particular task or piece of functionality.

The **protocol can then be adopted** by a `class`, `structure`, or `enumeration` to provide an actual implementation of those requirements.


### **Explain `JSONEncoder` and `JSONDecoder`**

- **Decodable** protocol, which allows us to take data and create instances of our object, populated with the data passed down from the server.
- **Encodable** protocol to take instances of our object and turn it into data. With that data, we can store it to the files, send it to the server, whatever you need to do with it.


### **What is `NotificationCenter`?**

**NotificationCenter** is an observer pattern, The NSNotificationCenter singleton allows us to broadcast information using an object called NSNotification.

The biggest difference between **KVO** and **NotificationCenter** is...
- **KVO** tracks specific changes to an object.
- **NotificationCenter** is used to track generic events.


### **Explain `subscripts`**

**Subscripts** are analogous to methods. 

`Classes`, `structures`, and `enumerations` can define subscripts, which are **shortcuts for accessing the member elements of** a `collection`, `list`, or `sequence`.


### **Explain `AVFoundation` framework**

We can create, play audio and visual media. 

**AVFoundation** allows us to work on a detailed level with time-based audio-visual data. With it, we can create, edit, analyze, and re-encode media files. 

**AVFoundation** has two sets of API, one that’s **video**, and one that is **audio**.


### **What’s the difference between a `Xib` and a `Storyboard`?**

Both are used in Xcode to layout screens (view controllers).

- A **Xib** defines a single View or View Controller screen
- A **Storyboard** shows many view controllers and also shows the relationship between them.


### **Explain Data Structures**

`Arrays`, `Sets`, `Tuples` and `Dictionaries` are all collections of data structures that store data in one place.


### **Explain `CodingKey` Protocol**

The **CodingKeys** enum (_Protocol_) lets you rename specific properties in case the serialized format doesn’t match the requirements of the API. **CodingKeys** should have nested enum.


### **What is `URLSession`?**

When we want to retrieve contents from a certain URL, we choose to use `URLConnection`. 

There are 3 types of tasks:
1. **Data tasks**: getting data to memory
2. **Download tasks**: downloading file to disk
3. **Upload tasks**: uploading file from disk and receiving response as data in memory


### **How does TestFlight make a difference?**

- Multiple builds distribution
- Testing groups
- Internal auto distribution
- Tester metrics
- Increased to 10,000 test users
- Public Link


### **Explain `@objc` inference**

We can tag a **Swift** declaration with **@objc** to indicate that it should be available to **Objective-C**. 

The most common place for this is any **Swift** method we want to refer to using a **selector**.


### **Explain VIPER Architecture**

**Viper** is an another design patters. It is based on **Single Responsibility Principle.**

It has 5 layers: 
- **V**iew
- **I**nteractor
- **P**resenter
- **E**ntity
- **R**outer

**Advantages** of Viper architecture is c**ommunication from one entity to another is given through protocols**. 

> The idea is to isolate our app’s dependencies, balancing the delegation of responsibilities among the entities.


### **Explain `Queues`**

**Queues** are **_used to store a set of data_**, but are different in that the first item to go into this collection, will be the first item to be removed. Also well known as **FIFO** which means, `first in first out`.


### **Explain `Result` Type**

The **Result** type is implemented as an enum that has 2 cases: **success** and **failure** callbacks. 

**Result** has 4 other methods: 
1. map()
2. flatMap()
3. mapError()
4. flatMapError()

Each of these gives you the ability to transform either **success** or **error**.


### **What is the difference between `UIKit` and `SwiftUI`?**

- **UIKit** is an imperative event-driven framework for building User Interfaces for iOS platform. 
- **SwiftUI** is a declarative framework for building User Interfaces for building User Interfaces for Apple platform.


### **Explain `abs()` function**

You use the **abs() function** to calculate the **_positive difference_** between the one value to another value.


### **Explain how to present a `SwiftUI` view on `UIKit`**

We need to use the class `UIHostingController` passing it the corresponding view

```
let viewController = UIHostingController(rootView: ContentView())
```


### **Explain how to present a `UIKit` ViewController on `SwiftUI`**

We can use `UIViewControllerRepresentable` & `UIViewRepresentable` 

- **UIViewControllerRepresentable:** Allows to use an `UIViewController` on **SwiftUI**.
  - Example:

**UIKit ViewController**
```
struct ImagePicker: UIViewControllerRepresentable {
    @Environment(\.presentationMode) var presentationMode
    @Binding var image: UIImage?
    
    func makeUIViewController(context: UIViewControllerRepresentableContext<ImagePicker>) -> UIImagePickerController {
        let picker = UIImagePickerController()
        picker.delegate = context.coordinator
        return picker
    }
    
    func updateUIViewController(_ uiViewController: UIImagePickerController, context: UIViewControllerRepresentableContext<ImagePicker>) { }
    
    func makeCoordinator() -> Coordinator {
        Coordinator(self)
    }
    
    class Coordinator: NSObject, UIImagePickerControllerDelegate, UINavigationControllerDelegate {
        
        let imagePicker: ImagePicker
        
        init(_ imagePicker: ImagePicker) {
            self.imagePicker = imagePicker
        }
        
        func imagePickerController(_ picker: UIImagePickerController, didFinishPickingMediaWithInfo info: [UIImagePickerController.InfoKey : Any]) {
            if let image = info[.originalImage] as? UIImage {
                imagePicker.image = image
            }
            imagePicker.presentationMode.wrappedValue.dismiss()
        }
    }
}
```

**Usage**

```
struct ContentView: View {
    @State var imageUser: UIImage?
    @State var showPicker = false
    
    var body: some View {
        VStack(spacing: 15) {
            if let imageUser = imageUser {
                Image(uiImage: imageUser)
                    .resizable()
                    .aspectRatio(contentMode: .fit)
                    .frame(height: 300)
            } else {
                Text("No image selected")
            }
            Button("Select image") {
                showPicker.toggle()
            }
        }
        .sheet(isPresented: $showPicker) {
            ImagePicker(image: $imageUser)
        }
    }
}
```


- **UIViewRepresentable:** Allows to use an `UIView` on **SwiftUI**.
  - Example:

**UIKit View**
```
import SwiftUI
import UIKit

struct TextHtml: UIViewRepresentable {
    let html: String?
    
    init(_ html: String?) {
        self.html = html
    }
    
    func makeUIView(context: UIViewRepresentableContext<Self>) -> UILabel {
        let label = UILabel()
        DispatchQueue.main.async {
            if let html = html, let data = html.data(using: .utf8), let attributedString = try? NSAttributedString(data: data, options: [.documentType: NSAttributedString.DocumentType.html], documentAttributes: nil) {
                label.attributedText = attributedString
            }
        }
        label.numberOfLines = 0
        
        return label
    }
    
    func updateUIView(_ uiView: UILabel, context: UIViewRepresentableContext<Self>) { }
}
```

**Usage**
```
struct ContentView: View {
    var body: some View {
        Group {
            TextHtml("<head><style type='text/css'>p { font: 20pt 'AmericanTypewriter'; color: #1a004b; }</style></head><p><strong>HTML text</strong></br> This work fine.</p>")
        }
    }
}
```







