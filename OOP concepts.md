

# Notes of OOP concepts vs Procedural Programming
## Structured programming
- First: identify which algorithm to manipulate data
- Why? Small problems are easily resolved with a procedural implementation (straight down, line by line)
- Why not? Because it scales very poorly
- As the program grows in size, its complexity increases
- Testing a single aspect becomes nearly impossible

## Why do we use OOP?
- Large problems can be more easily scaled using OOP paradigm
- OOP allows users to break problems down into small logical objects
- OOP allows users to view code-details within the context of a specific object
- OOP allows user to more easily debug code
- OOP allows greater testability of code

## An object-oriented program is made of objects
- Each object has specific functionalities, which users access via the object's methods
- The OOP paradigm suggests that a programmer will
	- First; identify which structures (objects) to manipulate data
	- Second; identify what algorithms each structure will use

## 3 Aspects of an object
- Identity: What is the location?
- State = What does it store?
- Behavior = How does it act?

## What are classes?
- Template or blueprint from which objects are made

## What is the difference between reference vs value types?
- Reference types are objects that store references to the actual data -> Class, interfaces, string
- Value Types hold value => Structs, Enums, Boolean, Numeric types

>Linked Lists means insertion-order. Hash means in order by memory location, tree means in order by some comparable value

## What is an interface? (implements)
- They are used to specify methods and properties that a derived class will have access to
- It does not containt daya
- Every property or methods inside the interface must be in the derived class
- You can implement with many interfaces

## What are Abstract classes?
- They are similar to interfaces, but they cannot be instantiated and they can be either partially implemented or not implemented at all
- Abstract classes can contain code or data
- A class can inherit from only one abstract class
- You can specify methods as virtual to force a derived class to create its own implementation

>If you have logic that will be the same for all classes -> use abstract classes instead of interfaces

## What is a static class?
- They cannot be instantiated

## Generics?
- Allows you to force types safely by letting you tailor a method or class to precise data type.
- For example:
````
List<ExampleClass> list 3 = new List<ExampleClass>();
	List<string> list2 = new List<string>();
	
	List 2 will be expecting only string, it will not let you enter another type
````

## What is Polymorphism ? (Many forms)
- Another example could be an Employee class and a contrat class that inherits from the employee class
		
		Employee class has a mehthod called calculateWeeklySalaryu(int weeklyHours, int wage), you can also
		calculate the salary in this function if you multiply 40 * wage.
		
		Contract class inherits from Employee class. It will have the same function signature, but the
		functionality would be different. Now salary would be weeklyHours * wage (OVERRIDE) 

Polymorphism = Classes having different functionality while sharing the same interface


## What is INHERITANCE ??

It is when an object or class is based on a parent object or class, taking on its characteristics
Can you use multiple inheritance ??? NO, you can do interfaces tho

FOUR PILLARS OF OOP ===> ABASTRACTION, ENCAPSULATION, INHERITCANCE, POLYMORPHISM

- Compile-time: the code you enter is converted to executable. A better way to explain it would be compile timer errors. 
These compile timer errors occurred due to typing mistake for instance. These errors won't let your program run a 
single line of code until these errors are fixed

- Runtime: Instance where the executable is running. Run time errors are the errors that are generated when the program
is in running state. Oftenly referred as Exceptions.


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE0MjMzMjY2OCwtMzMxODQwMTEyLDk2ND
EyOTYwNiwxNzk5OTc3MzYwLDE5NDg4MzAwMTJdfQ==
-->