

# Notes of OOP concepts vs Procedural Programming
## Structured programming
- Why? Small problems are easily resolved with a procedural implementation (straight down, line by line)
- Why not? Because it scales very poorly
- As the program grows in size, its complexity increases
- Testing a single aspect becomes nearly impossible

## Why do we use OOP?
- Large problems can be more easily scaled using OOP paradigm
- OOP allows users to break problems down into small logical objects
- Re-usability

## An object-oriented program is made of objects
- Each object has specific functionalities, which users access via the object's methods
- The OOP paradigm suggests that a programmer will
	- First; identify which structures (objects) to manipulate data
	- Second; identify what algorithms each structure will use

## What is Abstraction?

- The idea or concept of something (a person)
- Focus on the essential qualities of my person
- My person **should** have



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

- Generics eliminate unnecessary casts
- With generics, type checking happens at compiler time
- Allows you to force types safely and finding errors at compile time instead of runtime.
- For example:
````
Type parameters Names
E = Element (used extrensively by Java Collections)
K = Key
N = Number
T = Type

GENERIC CLASS:

public class class Person<E>{
	public E e;
	public void setPerson(E e) {
	this.e = e;
	}
	public E getPerson(){
	return this.e;
	}
}

Person<Employee> e1 = new Person<>();
Person<Contact> c1 = new Person<>();
// 2 references pointers that points to nothing so far.
 
Employee e = new Employee("Jhon", "Slattery", "12345"); // creating an employee
Contact c = new Contact("Mrs", "Peggy","Fisher","2020"); // creating a contract
e1.setPerson(e); // this is valid
c1.setPerson(c); // this is valid


2. GENERIC METHOD:
- They introduce their own type parameters
- The same method can be used for different reference types
- static and non-static methods can be generic

public static <E> void print (E[] list) {
	for( E element : list) {
	System.out.println(element);		
	}
}
````

## What is Polymorphism ? (Having Many forms)
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

## Hasseeb explanation

- Does java support multiple inheritance - no

- Abstraction - process of hiding the implementation details from user, only the functionality will be provided 
to the user

- Encapsulation - Keep data from a class protected from other objects. You can only access these data using the methods declared in my class. Restrict data. Reducing dependencies between different parts of the application.

- Inheritance - ability by which one class acquires the properties/attributes and behaviors/methods of another class. It is a great form of code reuse

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI3MTg0NzM4NCwtMjQ2MjI1MzQyLC0xNz
k1MTEwNDEsMTc0OTg0NTIyMSwtMzMxODQwMTEyLDk2NDEyOTYw
NiwxNzk5OTc3MzYwLDE5NDg4MzAwMTJdfQ==
-->