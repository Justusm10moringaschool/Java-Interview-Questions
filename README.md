# Java Technical Interview Questions
## Java
* What is the JVM?
    - Java virtual machine is a java runtime environment with specifications designed that dictate syntax for the code being run and the virtual machine running the code.
* Define code compilation?
    - The process of interpreting java source code into bytecode for use by the JVM - which converts the bytcode to native machine language
* What is a constuctor?
    - A method within a class in which creates an object that is an instance of that class when invoked by defining the attributes of the object.
* What is the naming convention of variables in java?
    - Variable names in java should be short(but not single lettered unless the variable is temporary), meaningful and should not start with an underscore or dollar sign.
* What is an annotation and give an example.
    - Annotations are modifiers that add information to code elements. An example is the `@Override` annotation which check for a method in a class in the parent classes.
* What is the difference between '==' and equals() when comparing Strings?
    - '==' is an operator that points to the memory location of objects being compared while equals is a method that compares the values of the objects undergoing comparison
* What are the 8 primitive types in Java?
    - boolean , byte , char , short , int , long , float and double.
* What is the difference between primitives and wrapper classes and when can we use each?
    - primitives are the most basic data types in java and they contain the reference value, that is, we can't have and empty primitive whereas wrappers are objects to which these primitives belong.
* Define Encapsulation and outline its benefits.
    - The process of bundling or wrapping methods and variables into private fields which helps in hiding and controlling the implementation details from users
* Do objects get passed by reference or value in Java? Elaborate on that.
    - Java passes object references to methods by value.
* Explain the four OOP principles.
    - Abstraction - the process of using objects variables and methods to represent complex code which helps avoid repetition and improve efficiency.
    - Polymorphism - works by referring to an object in the parent class to affect an object in the child class like implementing functions with the same name but different functionality.
    - Encapsulation - the process of keeping fields within a class private while providing public methods to access them. Enabling the reuse and safeguarding of backend implementation code.
    - Inheritance - A feature that enables programmers to create new classes that share the attributes of another class. It helps us build on previous work without re-inventing the wheel
* What is the difference between Abstract classes and Interfaces?
  - As far as their implementation is concerned, abstract classes are applied where objects have similar properties so they inherit from one class that has their common properties while interfaces are applied in situations where you want similar properties implemented differently.
  - A class can inherit from multiple interfaces but not from multiple classes.
  - Interfaces cannot have instantiations or fields while abstracts can.
  - Interface members are public by default and cannot have access modifiers while as abstract members can have access modifiers and are private by default.
* Is it possible to implement multiple inheritance in Java?
  - No, because incase you are inheriting from different classes with the same object being requested - there will be an ambiguity as to which implementation from which class to inherit.
* What is serialization? How do you implement it?
  - The process of converting objects into bytes so it can be transferred or saved elsewhere. It is deserialized after at the destination. Parcelers are used to carry out serialization
* What are anonymous classes?
  - These are local classes without names. They are instantiated and used in the same one location in  a single expression.
* What does it means to say that a String is immutable?
  -
* What is the difference between method overloading and method overriding?
  - Strings that cannot be modified.
* What are the access modifiers you know? What does each one do?
  - Keywords that determine the level of access a method or a variable has in java.
  -public - any class can access this  fields
  -protected - any class in the same package or a subclass can access this class.
  -private -
  -unspecified -
* Do objects get passed by reference or value in Java? Elaborate on that.
  - objects
* What the difference between local, instance and class variables?
  - An instance class is loaded when an object instance is created and it's value is only constant within the objects scope while a Class-variable is created when a class is initially loaded into the JVM for the first time and they are declared using the 'static' keyword.
  - Local variable are only accessed within their defined scope which is within the curly brackets while instance variables availability is determined by the access modifier they are declared with. `public`, `private` or `protected`. Public is accessible from anywhere whereas private and protected variables are accessed from the same class or subclasses.
* What is Dependency Injection?
  -The process by which `dependency container` analyses the dependencies of a class and create an instance of the class and inject the object into the dependency that way that way does not have a hard dependency in order to enable testing. It uses reflection to inject the object instance.
* What does the static word mean in Java? Can a static method be overridden in Java?
  - This denotes the availability of an object to the whole class without having to create a new instance of the class to access it.
* When is a static block run?
  - A static block is run when the JVM loads
* What is reflection?
  - This is code that is capable of inspecting other code and effecting changes on said code. This is mainly done at runtime where injection is involved.
* How does the try{} catch{} finally{}
    - The try block and the finally block(if available) have to be run otherwise the catch bloc is only run if there is an exception in the try block code, otherwise the catch block is skip all together.
* What is garbage collection? How does it work?
  - Garbage collection is the automated process at-least-in-java where unreferenced items in memory are deleted by the garbage collector in the JVM(in java)to prevent memory leaks.
* What is memory leak and how does Java handle it?
  -A memory leak is when unused objects remain in memory and hence the memory available for the running app is reduced.
* What does the keyword synchronized mean?
  - This is when different threads are trying to access and write to the same resource. This can lead to performance and result inconsistencies. So synchronized is keyword that facilitates sequential access of a resource by threads.
* Explain Generics in Java
  - Generics are designed to take any and all data types as arguments and return types.


## Web Development
* What is the difference between a GET and POST request?
  - GET method is used to fetch resources so they can't change the contents of a server while-as POST method are used for posting/sending/modifying data on the specified resource.
  - GET method has length restrictions POST methods don't.
  - GET methods can be cached POST can't.
  - GET methods get be bookmarked in the browser POST methods can't.
* What is a URI?
  - This a uniform resource identifier. They mark logical and physical locations.
* Differentiate between a client and host.
  - Host is a device within a network that can receive and respond to request and send requests. A client can ne able to send requests to the server for resources
* What is the difference between HTTP and HTTPS?
  - http is the set of rules that control the process of resource transfer between clients and hosts over the web while https is the same as http but the more secure due to the encryption of the contents being transferred.
* Point out these components(query, host, port, protocol, path ) in the following URL https://127.0.0.1:4200/login/a=bx?c
  -  https:// is the transfer protocol
  -  127.0.0.1:4200 - is the domain name and/or server id
  -  /login/ is the path or location on the said server.
  - a=bx?c the parameters or name of the resource being accessed
* What is an Internet Protocol?
  - A set of rules governing the format of data sent over the internet.
## Android
* What are the four main components of an Android Application?
  - Activities - dictate the interface and user interaction
  - Services - components that run in the background carrying out long running processes like fetching data over the network or playing music in the background
  - Content Providers - They are responsible for exposing or making data available to other apps on request irrespective of where the data is stored. Content resolvers are used to resolve
  - Broadcasters and Receivers - They are components that are responsible for intercepting notifications from other programs of the system itself.
* What is the purpose of a package name?
  - This is the unique identifier to an app on the app store.
* What is the purpose of Android Virtual Device?
  - An android virtual device is used by the android emulator to simulate the properties of a specific android device be it a smart watch, smart phone etc
