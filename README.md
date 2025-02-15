# iOS Developer Interview Questions for all Senioritis levels
###### The most complete guide to help those looking to hire a developer for iOS.
![dis-resource-landscape-1260x710](https://github.com/user-attachments/assets/61b8c73b-f618-44c5-bd8c-c14d6564df67)


---

## Content Questions: 
- [Memory Leak exercise](#how-would-you-fix-this-memory-leak)
- [Example between `Reference type` and `Value Type`?](#example-between-reference-type-and-value-type)
- [What is the difference between `self` and `Self`?](#what-is-the-difference-between-self-and-self)
- [How do I use `@State` and `@Binding` in SwiftUI?](#how-do-i-use-state-and-binding-in-swiftui)
- [Difference between `.task()` vs `.onAppear()`](#difference-between-task-vs-onappear)
- [Why SwiftUI uses `struct` for view and not `class`?](#why-swiftui-uses-struct-for-view-and-not-class)
- [What are some advantages of using `SwiftUI` over `UIKit`?](#what-are-some-advantages-of-using-swiftui-over-uikit)
- [What are SwiftUI `Modifiers`? Can you create some of your own and how?](#what-are-swiftui-modifiers-can-you-create-some-of-your-own-and-how)
- [Difference between `declarative` vs `imperative` programming?](#difference-between-declarative-vs-imperative-programming)
- [What are `PreferenceKey` used for?](#what-are-preferencekey-used-for)
- [Explain what is `Grand Central Dispatch` (GCD) in iOS?](#explain-what-is-grand-central-dispatch-gcd-in-ios)
- [What is the difference between `Synchronous` & `Asynchronous` task?](#what-is-the-difference-between-synchronous--asynchronous-task)
- [Why are the asynchronous tasks in iOS development important and how do you handle asynchronous programming in iOS apps?](#why-are-the-asynchronous-tasks-in-ios-development-important-and-how-do-you-handle-asynchronous-programming-in-ios-apps)
- [What is made up of `NSError` object?](#what-is-made-up-of-nserror-object)
- [What is `Enum` or `Enumerations`?](#what-is-enum-or-enumerations)
- [When is recommended to use `weak`, `unowned` and `strong` references?](#when-is-recommended-to-use-weak-unowned-and-strong-references)
- [What’s the difference between the `frame` and the `bounds`?](#whats-the-difference-between-the-frame-and-the-bounds)
- [Why is design pattern very important?](#why-is-design-pattern-very-important)
- [What is Singleton Pattern?](#what-is-singleton-pattern)
- [What is Facade Design Pattern?](#what-is-facade-design-pattern)
- [What is Decorator Design Pattern?](#what-is-decorator-design-pattern)
- [What is Adapter Pattern?](#what-is-adapter-pattern)
- [What is Observer Pattern?](#what-is-observer-pattern)
- [Explain MVC](#explain-mvc)
- [Explain `generics` in Swift?](#explain-generics-in-swift)
- [Explain `lazy` in Swift?](#explain-lazy-in-swift)
- [Explain what is `defer`?](#explain-what-is-defer)
- [How to pass data between view controllers?](#how-to-pass-data-between-view-controllers)
- [What is Concurrency?](#what-is-concurrency)
- [Readers-Writers](#readers-writers)
- [NSOperation — NSOperationQueue — NSBlockOperation](#nsoperation--nsoperationqueue--nsblockoperation)
- [KVC — KVO](#kvc--kvo)
- [Explain `Guard` statement](#explain-guard-statement)
- [What is the difference `Non-Escaping` and `Escaping` Closures?](#what-is-the-difference-non-escaping-and-escaping-closures)
- [Explain `[weak self]` and `[unowned self]`?](#explain-weak-self-and-unowned-self)
- [What is ARC?](#what-is-arc)
- [Difference between `SceneDelegate` and `AppDelegate`](#difference-between-scenedelegate-and-appdelegate)
- [Why is everything in a `do-catch` block?](#why-is-everything-in-a-do-catch-block)
- [Explain Swift Package Manager (SPM)](#explain-swift-package-manager-spm)
- [How is an `inout` parameter different from a `regular` parameter?](#how-is-an-inout-parameter-different-from-a-regular-parameter)
- [Explain `View Controller Lifecycle` events order?](#explain-view-controller-lifecycle-events-order)
- [What is `Class`?](#what-is-class)
- [What is `Object`?](#what-is-object)
- [When and why do we use an `object` as opposed to a `struct`?](#when-and-why-do-we-use-an-object-as-opposed-to-a-struct)
- [What are the `states` of an iOS App?](#what-are-the-states-of-an-ios-app)
- [What is `DispatchGroup`?](#what-is-dispatchgroup)
- [Where do we use `Dependency Injection`?](#where-do-we-use-dependency-injection)
- [Please explain types of notifications](#please-explain-types-of-notifications)
- [What kind of `high order functions` can we use on collection types?](#what-kind-of-high-order-functions-can-we-use-on-collection-types)
- [Explain `Bridging Headers` in iOS project](#explain-bridging-headers-in-ios-project)
- [What is `Hashable`?](#what-is-hashable)
- [How many different ways to pass data in Swift?](#how-many-different-ways-to-pass-data-in-swift)
- [What is the difference `Delegates` and `Callbacks`?](#what-is-the-difference-delegates-and-callbacks)
- [What is Pointer?](#what-is-pointer)
- [What is the difference between `try?` and `try!`?](#what-is-the-difference-between-try-and-try)
- [Why do we use `availability` attributes?](#why-do-we-use-availability-attributes)
- [What is `Encapsulation`?](#what-is-encapsulation)
- [How could we get `device token`?](#how-could-we-get-device-token)
- [Explain differences between `service extension` and `content extension`](#explain-differences-between-service-extension-and-content-extension)
- [What is `Instruments`?](#what-is-instruments)
- [What is `Deep Linking`?](#what-is-deep-linking)
- [What is `Optional Binding`?](#what-is-optional-binding)
- [Explain `Polymorphism`](#explain-polymorphism)
- [Explain `In-app Purchase products and subscriptions`](#explain-in-app-purchase-products-and-subscriptions)
- [What is `Protocol`?](#what-is-protocol)
- [Explain `JSONEncoder` and `JSONDecoder`](#explain-jsonencoder-and-jsondecoder)
- [What is `NotificationCenter`?](#what-is-notificationcenter)
- [Explain `subscripts`](#explain-subscripts)
- [Explain `AVFoundation` framework](#explain-avfoundation-framework)
- [What’s the difference between a `Xib` and a `Storyboard`?](#whats-the-difference-between-a-xib-and-a-storyboard)
- [Explain Data Structures](#explain-data-structures)
- [Explain `CodingKey` Protocol](#explain-codingkey-protocol)
- [What is `URLSession`?](#what-is-urlsession)
- [How does TestFlight make a difference?](#how-does-testflight-make-a-difference)
- [Explain `@objc` inference](#explain-objc-inference)
- [Explain VIPER Architecture](#explain-viper-architecture)
- [Explain `Queues`](#explain-queues)
- [Explain `Result` Type](#explain-result-type)
- [What is the difference between `UIKit` and `SwiftUI`?](#what-is-the-difference-between-uikit-and-swiftui)
- [Explain `abs()` function](#explain-abs-function)
- [Explain how to present a `SwiftUI` view on `UIKit`](#explain-how-to-present-a-swiftui-view-on-uikit)
- [Explain how to present a `UIKit` ViewController on `SwiftUI`](#explain-how-to-present-a-uikit-viewcontroller-on-swiftui)

---

### **How would you fix this memory leak?**

```swift
import Foundation

class Person {
    var name: String
    var dog: Dog?

    init(name: String) {
        self.name = name
        print("\(name) is born.")
    }

    deinit {
        print("\(name) is being deinitialized.")
    }
}

class Dog {
    var name: String
    var owner: Person?

    init(name: String) {
        self.name = name
        print("\(name) is born.")
    }

    deinit {
        print("\(name) is being deinitialized.")
    }
}

var john: Person? = Person(name: "John")
var fido: Dog? = Dog(name: "Fido")

john?.dog = fido
fido?.owner = john

john = nil // release John
fido = nil // release Fido
```

**Solution:**
`owner` Property as **weak**:
- By declaring the owner property as weak, it ensures that it does not hold a strong reference to the Person instance. As a result, when the Person instance is deallocated (set to nil), the weak reference automatically becomes nil, breaking the reference cycle.

```swift
weak var owner: Person? // Changed to weak to break the reference cycle
```



### **Example between `Reference type` and `Value Type`?**

```swift
// Objects
struct Man {
    var name: String
    var lastname: String
}

class Woman {
    var name: String
    var lastname: String

    init(name: String, lastname: String) {
        self.name = name
        self.lastname = lastname
    }
}

// Value type
let hugo = Man(name: "Hugo", lastname: "Garcia")
var juan = hugo
juan.name = "Juan"

print(hugo.name)
print(juan.name)

/** Output
 - Hugo
 - Juan
 */

// Reference type
let maria = Woman(name: "Maria", lastname: "Garcia")
var ana = maria
ana.name = "Ana"

print(maria.name)
print(ana.name)

/** Output
 - Ana
 - Ana
 */

```

### **What is the difference between `self` and `Self`?**

- **self**: 
The self is used to refer to the current instance of a class, structure, or enumeration within its own instance methods or initializers. It is similar to this keyword in other programming languages. For example:

```swift
class MatchScore {

    let value: Int
    
    init(value: Int) {
        self.value = value
    }
}

let cricketScore = MatchScore(value: 325)
print(cricketScore.value) // print: 325
```

- **Self**:
The Self is used to refer to the type of the current class, structure, or enumeration within its own methods or initializers. It is similar to this or typeof in other programming languages. Fro example:

```swift
protocol ScoreCreation {
    static func create() -> Self
}

class MatchScore: ScoreCreation {

    required init() { }

    static func create() -> Self {
        return self.init()
    }
}

let scoreObject = MatchScore.create()
print(type(of: scoreObject)) // print: "MatchScore"
```

### **How do I use `@State` and `@Binding` in SwiftUI?**
**@State** is used to create a state property that can be read and written to, while **@Binding** is used to share a state with another view.

```swift
struct ParentView: View {
    @State private var isOn = false  // Declares and owns the state

    var body: some View {
        ToggleView(isOn: $isOn)  // Passes a binding
    }
}

struct ToggleView: View {
    @Binding var isOn: Bool  // Receives a binding to `isOn`

    var body: some View {
        Toggle("Switch", isOn: $isOn)  // Directly modifies the parent state
    }
}
```

### Difference between `.task()` vs `.onAppear()`

In SwiftUI, both **.task()** and **.onAppear()** are view modifiers that can be used to run some code when a view is shown. 

Modifer `.task()` allows you to use the `async/await` directly to perform asynchronous work. While `.onAppear()` is an older modifier that can only run synchronous code, you need to use `Task` or `DispatchQueue` to bridge to async code.

`.task()` is automatically canceled when the view disappears, helping with memory management.

```swift
struct ContentView: View {
  @State var text: String = "Loading..."

  // Async function
  func asyncGetText() async -> String {
    // Simulate some network request
    await Task.sleep(3_000_000_000)
    return "Hello, world!"
  }

  var body: some View {
    Text(text)
      .padding()
      // Start a task when the view is shown
      .task {
        // Await the result of the async function
        let result = await asyncGetText()
        // Update the state with the result
        text = result
      }
  }
}

// or Using onAppear
struct ContentView: View {
  /* ... */

  var body: some View {
    Text(text)
      .padding()
      // Run some code when the view is shown
      .onAppear {
        // Start a task to call the async function
        Task {
          // Await the result of the async function
          let result = await asyncGetText()
          // Update the state with the result
          text = result
        }
      }
  }
}
```




### **Why SwiftUI uses `struct` for view and not `class`?**

- **No Shared State**: Structs provide value semantics, meaning each instance is a unique value and is passed by value rather than by reference. This eliminates concerns about shared mutable state, making it easier to reason about the app’s behavior and reducing the chances of unexpected side effects.

- **Immutable by Default**: Structs in Swift are immutable by default, encouraging a more functional programming style where changes are made by creating new instances rather than mutating existing ones. This immutability helps maintain a clear and predictable flow of data, which is crucial in SwiftUI’s reactive paradigm.

- **Performance Benefits**: Structs are generally more lightweight than classes, which can lead to performance benefits, especially when creating and managing multiple instances of views, as is common in SwiftUI.

- **Thread Safety**: Since structs are immutable and don’t have shared state, they inherently mitigate some concerns related to thread safety. In SwiftUI, this aligns well with its reactive nature, where changes to the state trigger updates to the UI in a predictable and thread-safe manner.

- **Automatic View Updating**: SwiftUI relies on value types like structs to automatically update views when their associated state changes. The use of structs simplifies this process by ensuring that changes to the state trigger UI updates without the need for explicit handling or observation.

### **What are some advantages of using `SwiftUI` over `UIKit`?**

- **Declarative Syntax**: SwiftUI uses a declarative syntax, allowing developers to describe the UI and its behavior in a concise and easy-to-understand manner. This approach reduces boilerplate code and simplifies the process of creating and maintaining user interfaces.

- **Live Preview and Real-Time Editing**: SwiftUI provides a live preview feature in Xcode, enabling developers to see real-time changes made to the UI code. This instant feedback loop streamlines the development process and facilitates quicker iteration.
  
- **Less Code, More Flexibility**: With SwiftUI, developers can achieve complex layouts and interactions with significantly less code compared to UIKit. The framework’s built-in components and modifiers help create dynamic and adaptive interfaces with ease.
  
- **Unified Codebase for Multiple Platforms**: SwiftUI supports multi-platform development, allowing developers to use a single codebase to create user interfaces for iOS, macOS, watchOS, and tvOS applications. This unified approach simplifies the development and maintenance of applications across Apple platforms.
  
- **Automatic Adaptation to Different Device Sizes and Orientations**: SwiftUI’s layout system automatically adapts to different device sizes and orientations, making it easier to create responsive and adaptive user interfaces without manually handling constraints and size classes.
  
- **Native Integration with Swift**: SwiftUI is built using Swift and takes advantage of its language features, such as type safety, optionals, and closures. This native integration provides a seamless development experience for Swift developers.
  
- **Built-in Animations and Transitions**: SwiftUI simplifies the implementation of animations and transitions with its built-in animation APIs. Developers can easily add smooth and interactive animations to their UI elements using simple modifiers and transitions.
  
- **State Management Simplification**: SwiftUI introduces state management with features like @State, @Binding, @ObservedObject, and @EnvironmentObject, simplifying the handling of data and state changes within views.
  
- **Automatic Accessibility Support**: SwiftUI incorporates accessibility features by default, making it easier for developers to create apps that are accessible to users with disabilities. The framework encourages best practices for accessibility.
  
- **Enhanced Preview Support**: SwiftUI’s preview system in Xcode allows for better testing and visualisation of different states and scenarios of the UI, aiding in rapid prototyping and testing.

### **What are SwiftUI `Modifiers`? Can you create some of your own and how?**

In **SwiftUI**, **modifiers** are methods you use to change the appearance, layout, and behavior of a view. Modifiers allow you to customize views in a declarative, chainable way.

**Creating Custom Modifiers**

You can create **custom modifiers** by conforming to the `ViewModifier` protocol. This allows you to encapsulate common view modifications into a single reusable modifier, making your code cleaner and more readable.

**Let’s say we want to create a reusable style for text, with specific font, padding, and background color.**

1. **Define the Custom Modifier:**

```swift
import SwiftUI

struct CustomTextStyle: ViewModifier {
    func body(content: Content) -> some View {
        content
            .font(.title)
            .padding()
            .background(Color.blue)
            .foregroundColor(.white)
            .cornerRadius(10)
    }
}

struct ColoredBackground: ViewModifier {
    var color: Color

    func body(content: Content) -> some View {
        content
            .padding()
            .background(color)
            .cornerRadius(8)
    }
}
```

2. **Create an Extension for Easier Use:**

```swift
extension View {
    func customTextStyle() -> some View {
        self.modifier(CustomTextStyle())
    }

    func coloredBackground(color: Color) -> some View {
        self.modifier(ColoredBackground(color: color))
    }
}
```


3. **Using the Custom Modifier:**

```swift
struct ContentView: View {
    var body: some View {
        Text("Custom Styled Text")
            .customTextStyle() // Applying our custom modifier

        Text("Dynamic Background Color") 
            .coloredBackground(color: .green)
    }
}

```


### **Difference between `declarative` vs `imperative` programming?** 

**Imperative Programming in Swift:**

In an imperative style, you tell Swift how to achieve a goal, step by step. You control the exact flow, specify each action, and manually manage state changes. Traditional programming in Swift (especially with **UIKit**) is often imperative.

**Key Characteristics:**

- Step-by-step instructions.
- Explicit control over flow and state.
- Typically uses loops, conditionals, and variables to control behavior.

With UIKit, creating a label would require you to manually define and manage its properties and layout.

<details><summary>Imperative Example</summary>
<p>
    
```swift
import UIKit

let label = UILabel()
label.text = "Hello, World!"
label.textColor = UIColor.blue
label.textAlignment = .center
label.frame = CGRect(x: 50, y: 100, width: 200, height: 40)
view.addSubview(label)
```
</p>
</details>

**Declarative Programming in Swift:**

In a declarative style, you describe what the desired result should look like, and Swift handles the underlying steps for you. **SwiftUI**, Swift’s UI framework introduced in 2019, is built around a declarative approach.

**Key Characteristics:**

- Describe what you want rather than how to achieve it.
- Less explicit control over flow; instead, you specify the end result.
- SwiftUI automatically updates the UI based on the state changes, often using state-driven logic.

With SwiftUI, creating a label (Text view) is more concise and describes what the UI should look like.

<details><summary>Declarative Example</summary>
<p>

```swift
import SwiftUI

struct ContentView: View {
    var body: some View {
        Text("Hello, World!")
            .foregroundColor(.blue)
            .frame(width: 200, height: 40)
            .background(Color.yellow)
            .cornerRadius(10)
    }
}

```
</p>
</details>



### **What are `PreferenceKey` used for?**

In **SwiftUI**, a `PreferenceKey` is used to **pass data up** the view hierarchy, allowing child views to communicate information to their parent views. Typically, SwiftUI views pass data down the hierarchy using bindings, but there are scenarios where you need to send data from a child to a parent. This is where PreferenceKey comes in.

**Use Cases:**

- **Passing information from a child to a parent**: When a child view needs to share a value with its parent (such as layout information or a state change), but the parent isn’t directly responsible for managing the state.
- **Layout and Geometry Changes**: It’s often used to propagate layout information, like the size of a child view, back up to a parent view to adjust its layout.
- **Custom Layouts**: In cases where you want to create custom container views that need information from their children to adjust their layout, like calculating a size based on child views.

**Here’s an example of how to use a PreferenceKey to pass a value (like a width) from a child view to its parent:**

<details><summary>Example</summary>
<p>

```swift
import SwiftUI

// Define the PreferenceKey
struct WidthPreferenceKey: PreferenceKey {
    static var defaultValue: CGFloat = 0

    static func reduce(value: inout CGFloat, nextValue: () -> CGFloat) {
        value = max(value, nextValue()) // Combine values (here we take the max width)
    }
}

// Child view that sets the preference
struct ChildView: View {
    var body: some View {
        Text("Hello, World!")
            .padding()
            .background(Color.blue)
            .foregroundColor(.white)
            .overlay(
                GeometryReader { geometry in
                    Color.clear
                        .preference(key: WidthPreferenceKey.self, value: geometry.size.width)
                }
            )
    }
}

// Parent view that receives the preference
struct ParentView: View {
    @State private var childWidth: CGFloat = 0

    var body: some View {
        VStack {
            Text("Child width: \(childWidth)")
            ChildView()
                .onPreferenceChange(WidthPreferenceKey.self) { value in
                    childWidth = value
                }
        }
    }
}
```
</p>
</details>


### **Explain what is `Grand Central Dispatch` (GCD) in iOS?**

  Grand Central Dispatch (**GCD**) is a low-level API that allows users to run concurrent tasks(run simultaneously). It also manages threads in the background. Apple’s solution is to build concurrency and parallelism into iOS applications so different tasks can run concurrently in the background without affecting the main thread.
  
### **What is the difference between `Synchronous` & `Asynchronous` task?**

- **Synchronous**: waits until the task have completed 
- **Asynchronous**: completes a task in the background and can notify you when complete

### **Why are the `asynchronous tasks` in iOS development important and how do you handle asynchronous programming in iOS apps?**

Asynchronous tasks are crucial in iOS development because they allow the app to handle potentially slow or resource-intensive operations without blocking the main thread, which is responsible for the user interface. This helps ensure a smooth user experience by preventing UI freezes and enabling responsive interactions even when the app is performing complex operations in the background.

**Why Asynchronous Tasks are Important in iOS**

1.	**Performance**: Many tasks, such as network requests, file I/O, or heavy computations, take time to complete. Running these tasks synchronously on the main thread can cause the app to appear unresponsive, leading to a poor user experience.
2.	**Smooth UI**: In iOS, the main thread (or UI thread) is dedicated to rendering the user interface and processing user interactions. Blocking this thread with time-consuming operations results in a laggy or frozen UI. Asynchronous programming allows these tasks to run on background threads, keeping the UI responsive.
3.	**Battery Efficiency**: Offloading tasks to run only when necessary, and in the background if possible, helps optimize power consumption, as the system can manage resources better across all apps.

**Choosing the Right Asynchronous Tool**

- For simple, one-off background tasks, **GCD** is generally sufficient.
- For more complex task management, like dependencies and prioritization, **OperationQueue** is ideal.
- For code clarity and simplicity, especially in Swift 5.5+, **async/await** provides a readable and maintainable solution.
- For responding to continuous streams of data or for reactive programming, **Combine** is a good fit.


### **What is made up of `NSError` object?**

There are three parts of **NSError** object a `domain`, an `error code`, and a `user info dictionary`. The domain is a string that identifies what categories of errors this error is coming from.


### **What is `Enum` or `Enumerations`?**

**Enum** is a type that basically contains a group of related values in the same umbrella


### **When is recommended to use `weak`, `unowned` and `strong` references?**

In Swift, the choice between weak, unowned, and strong references depends on the relationship between the objects and their lifetimes:
1. `Strong` references:
- Default reference type.
- The referenced object’s lifetime is extended as long as the strong reference exists.
- Use when you want the reference to own and manage the lifecycle of the object.
- **Example**: Holding a reference to a view model in a view controller.


2.	`Weak` references:
- The referenced object’s lifetime is not extended by the reference.
- Use when you want to avoid retain cycles (where two objects hold strong references to each other) but still need to reference an object that can be deallocated, such as delegates or closures capturing self.
- **Important**: The object being referenced can become nil, so the reference is automatically set to nil when the object is deallocated.
- **Example**: A delegate in a view controller.


3.	`Unowned` references:
- Similar to weak references, but the referenced object is assumed to never be deallocated while the reference exists.
- Use when you are certain the referenced object will outlive the reference (i.e., they have a parent-child relationship where the child doesn’t outlive the parent).
- **Important**: Accessing a deallocated object via an unowned reference causes a runtime crash.
- **Example**: A closure capturing self in a parent object where self is guaranteed to not be deallocated before the closure.


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


### **What is the difference `Non-Escaping` and `Escaping` Closures?**

- **@escaping**: The closure can be executed after the function terminates, either because it is stored or executed in an asynchronous operation.

```swift
// can be called after the function returns
func executeLater(action: @escaping () -> Void) {
    DispatchQueue.main.asyncAfter(deadline: .now() + 1) {
        action() // executing later
    }
}
```

- **@nonescaping**: The closure must be executed within the scope of the receiving function, and cannot be executed after the function terminates.

```swift
// must be called before the function returns
func executeNow(action: () -> Void) {
    action() // immediate execution
}
```


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

![5018abb-b4c-a38d-1d3d-6c2e6000fb8f_View_Controller_Lifecycle](https://github.com/user-attachments/assets/e2036689-d3d7-4a4d-95f3-34d69d435cb2)


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

**There are 3 forms of dependency injection (`Constructor`, `Property` & `Method`) :** 
  - `constructor` injection
  
```swift
// Protocol defining a data service
protocol DataService {
    func fetchData() -> [String]
}

// Concrete implementation of the data service
class RemoteDataService: DataService {
    func fetchData() -> [String] {
        // Fetch data from a remote source
        return ["Data1", "Data2", "Data3"]
    }
}

// ViewModel for processing data
class DataViewModel {
    private let dataService: DataService

    init(dataService: DataService) {
        self.dataService = dataService
    }

    func fetchData() -> [String] {
        return dataService.fetchData()
    }
}

// Usage
let remoteDataService = RemoteDataService()
let dataViewModel = DataViewModel(dataService: remoteDataService)
let data = dataViewModel.fetchData()
print("Fetched Data:", data)
```

  - `property` injection


```swift
// Protocol defining a networking service
protocol NetworkingService {
    func fetchData(completion: @escaping ([String]?) -> Void)
}

// Concrete implementation of the networking service
class APINetworkingService: NetworkingService {
    func fetchData(completion: @escaping ([String]?) -> Void) {
        // Simulate fetching data from an API
        DispatchQueue.main.asyncAfter(deadline: .now() + 2) {
            completion(["Result1", "Result2", "Result3"])
        }
    }
}

// Class that relies on the networking service through property injection
class DataManager {
    var networkingService: NetworkingService?

    func fetchAndProcessData() {
        networkingService?.fetchData { [weak self] data in
            // Process the fetched data
            print("Fetched Data:", data ?? "No data")
        }
    }
}

// Usage
let apiNetworkingService = APINetworkingService()
let dataManager = DataManager()
dataManager.networkingService = apiNetworkingService
dataManager.fetchAndProcessData()
```

  - `method` injection

    
```swift
// Dependency we want to inject
class PrinterService {
    func printMessage(_ message: String) {
        print("Printing: \(message)")
    }
}

// Class where dependency is required
class MessageHandler {
    private var printerService: PrinterService?

    // Method where dependency is gonna be injected
    func setPrinterService(_ service: PrinterService) {
        self.printerService = service
    }

    // Method where dependnecy is needed / used 
    func sendMessage(_ message: String) {
        printerService?.printMessage(message) ?? print("No printer service available")
    }
}

// Usage
let printerService = PrinterService()  // Dependency instance
let messageHandler = MessageHandler()   // Handley instance

// Injecting dependency in the method
messageHandler.setPrinterService(printerService)

// Now we can use the funtionality
messageHandler.sendMessage("Hello, Dependency Injection!")
// Output: "Printing: Hello, Dependency Injection!"    
```

### **Please explain types of notifications**

- There are 2 type of notifications:
  - **Remote notification**
    - requires connection to a server.  
  - **Local notification** 
    - doesn't require server connection. Local notifications happen on device.
  - **Silent notification** 
    - Similar to remote notifications but they are transparent for the user (no visual, no sound) to do something in the background.
   
![1_zOBBVwvZ31FLns_QfaE_AA](https://github.com/user-attachments/assets/0e936d95-8848-4fb1-b702-a3a520bc2c7e)

To send background notifications, create a remote notification payload with apskey containing only the content-available key. This key indicates that the notification is silent and doesn’t require any user interaction.

**Payload Sample**

```json
{
    "aps" : {
        "content-available" : 1
    },
     "data" :{
        "title" : "custom data",
        "body" : "custom data"
     }
}
```



### **What kind of `hight order functions` can we use on collection types?**

**Model Sample:**
```swift
struct Person {
    let name: String
    let age: Int
    let city: String
}

let people = [
    Person(name: "Alice", age: 25, city: "New York"),
    Person(name: "Bob", age: 32, city: "Los Angeles"),
    Person(name: "Charlie", age: 19, city: "Chicago"),
    Person(name: "Diana", age: 40, city: "New York")
]
```

- **map(_:):** 
  - Returns an array of results after transforming each element in the sequence using the provided closure.

 ```swift
let numbers = [1, 2, 3, 4, 5]
let squaredNumbers = numbers.map { $0 * $0 }
print(squaredNumbers) // [1, 4, 9, 16, 25]

let names = people.map { $0.name }
print(names) // ["Alice", "Bob", "Charlie", "Diana"]

let futureAges = people.map { $0.age + 5 }
print(futureAges) // [30, 37, 24, 45]
```

- **filter(_:):** 
  - Returns an array of elements that satisfy the provided closure predicate.

 ```swift
let numbers = [1, 2, 3, 4, 5]
let evenNumbers = numbers.filter { $0 % 2 == 0 }
print(evenNumbers) // [2, 4]

let olderThan30 = people.filter { $0.age > 30 }
print(olderThan30.map { $0.name }) // ["Bob", "Diana"]

let inNewYork = people.filter { $0.city == "New York" }
print(inNewYork.map { $0.name }) // ["Alice", "Diana"]
```

- **reduce(_:_:):** 
  - Returns a single value by combining each element in the sequence using the provided closure.

 ```swift
let numbers = [1, 2, 3, 4, 5]
let sum = numbers.reduce(0) { $0 + $1 }
print(sum) // 15

let totalAge = people.reduce(0) { $0 + $1.age }
print(totalAge) // 116

let allNames = people.reduce("") { $0 + $1.name + ", " }.dropLast(2)
print(allNames) // "Alice, Bob, Charlie, Diana"
```

- **sorted(by:):** 
  - Returns an array of the elements in the sequence sorted based on the provided closure predicate.
 
```swift
let numbers = [3, 1, 4, 1, 5, 9]
let sortedNumbers = numbers.sorted()
print(sortedNumbers) // [1, 1, 3, 4, 5, 9]

let sortedByAge = people.sorted { $0.age < $1.age }
print(sortedByAge.map { $0.name }) // ["Charlie", "Alice", "Bob", "Diana"]

let sortedByName = people.sorted { $0.name > $1.name }
print(sortedByName.map { $0.name }) // ["Diana", "Charlie", "Bob", "Alice"]
```


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

<img width="500" alt="viper" src="https://github.com/user-attachments/assets/89e25b92-68e8-41cf-8f51-d60167fb11be" />


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

```swift
let viewController = UIHostingController(rootView: ContentView())
```


### **Explain how to present a `UIKit` ViewController on `SwiftUI`**

We can use `UIViewControllerRepresentable` & `UIViewRepresentable` 

- **UIViewControllerRepresentable:** Allows to use an `UIViewController` on **SwiftUI**.
 
<details><summary>Example</summary>
<p>
  
**UIKit ViewController**
  
  
```swift
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

```swift
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
</p>
</details>


- **UIViewRepresentable:** Allows to use an `UIView` on **SwiftUI**.
   
<details><summary>Example</summary>
<p>
  
  
**UIKit View**
  
```swift
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
```swift
struct ContentView: View {
    var body: some View {
        Group {
            TextHtml("<head><style type='text/css'>p { font: 20pt 'AmericanTypewriter'; color: #1a004b; }</style></head><p><strong>HTML text</strong></br> This work fine.</p>")
        }
    }
}
```
</p>
</details>







