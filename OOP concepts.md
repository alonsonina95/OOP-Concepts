

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

## Object Relations
- Has reference to a (Association)
-- Indicates that a class holds a reference to another instance of a class has ownership of a reference to another instance of a class 
- Has Ownership of a (Aggregation): (Has or has many )
-- Denotes that an object has ownership of another object.
-- Each object references is said to be a child of another reference (parent) (1-1) or one to many (1-M)
> Person has a pet : class person { private Animal pet;}
> Person has many pets: class person { private List(Animlal)pets;}
- Uses a dependence
-- Greader uses a Student to obtain a Character representative of grade
> public class Grader { public Character grade(Student student){}}
- Is a (inheritance)
-- This relationship denotes dynamic-polymophism
-- Denotes that a class is a specific type of a more general super class
-- Denotes a class has inherent-members (methods/variables) from super class
-- Inherent-member are not explicitly declared in the inheriting class (sub class)
-- All classes are implicit sub-classes of the Object class
- Has Ownership of a (Composition):
-- We create a field by deriving values from other variables.
-- We compose a field in a class by using external sources being passed to the class
-- Our class implement a functionality that only our class can do with certain values originated in other classes.
> Person has a birdhDate using composition: constructor(x,y,z) {this.birthdate = new Date(x,y,z);}
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk0ODgzMDAxMl19
-->