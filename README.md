description of this code i maintain in program in commments please read comments and understand the code and try write code.
below i write a why and when we can use which type of dependecny injections.

When to use Property Dependency Injection over Constructor Injection and vice versa?
The Constructor Dependency Injection in C# is the standard for Dependency Injection.
It ensures that all the dependency objects are initialized before we are going to invoke
any methods or properties of the dependency object, as a result, it avoids the Null Reference Exception.

The Setter/Property Dependency Injection in C# is rarely used in Real-Time applications.
For example, if I have a class that has several methods but those methods do not depend on any other objects.
Now, I need to create a new method within the same class but that new method now depends on another object. 
If we use the constructor dependency injection here, then we need to change all the existing constructor calls where we created this class object. 
This can be a very difficult task if the project is a big one. Hence, in such scenarios, the Setter or Property Dependency Injection can be a good choice.
