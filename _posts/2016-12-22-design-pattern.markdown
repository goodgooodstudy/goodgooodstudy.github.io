---
layout:     post
title:      "Design Pattern"
subtitle:   " \"I love sleeping\""
date:       2016-10-02 12:00:00
author:     "Chengyang"
header-img: "img/post-bg-2015.jpg"
tags:
    - design
---

> “Yeah It's on. ”
>
## design pattern
	software design pattern is a general reusable solution to a commonly occurring problem within a given context in software design.
	It is a description or templatefor how to solve a problem that can be used in many different situations. Design patterns are formalized best practices that the programmer can use to solve common problems whendesigning an application or system. software architectural pattern for implementing user interfaces on computers.


## benefits
	• They give the developer a selection of tried and tested solutions to work with
	• They are language neutral and so can be applied to any language that supports object-orientation
	• They aid communication by the very fact that they are well documented and can be researched if that is not the case.
	• They have a proven track record as they are already widely used and thus reduce the technical risk to the project
	• They are highly flexible and can be used in practically any type of application or domain


###	Creational Patterns
1.	Builder

		Definiation:
		The Builder Creational Pattern is used to separate the construction of a 		complex object from its representation so that the same construction 		process can create different objects representations.

		Problem:
		We want to construct a complex object, however we do not want to have a 		complex constructor member or one that would need many arguments.

		Solution: 
		Define an intermediate object whose member functions define the desired 		object part by part before the object is available to the client. Builder 		Pattern lets us defer the construction of the object until all the options 		for creation have been specified.

2.	Factory
	1.	Abstract Factory

			Definition: A utility class that creates an instance of several families of classes. It can also return a factory for a certain group.

			The Factory Design Pattern is useful in a situation that requires the creation of many different types of objects, all derived from a common base type. The Factory Method defines a method for creating the objects, which subclasses can then override to specify the derived type that will be created. Thus, at run time, the Factory Method can be passed a description of a desired object (e.g., a string read from user input) and return a base class pointer to a new instance of that object. The pattern works best when a well-designed interface is used for the base class, so there is no need to cast the returned object.
			Problem 
			We want to decide at run time what object is to be created based on some configuration or application parameter. When we write the code, we do not know what class should be instantiated.
			Solution 
			Define an interface for creating an object, but let subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses.
			In the following example, a factory method is used to create laptop or desktop computer objects at run time.

3.	Prototype
4.	Singleton

			• Ensure a class has only one instance, and provide a global point of access to it.
			• Encapsulated "just-in-time initialization" or "initialization on first use".

			i. The Singleton pattern ensures that a class has only one instance and provides a global point of access to that instance. It is named after the singleton set, which is defined to be a set containing one element. This is useful when exactly one object is needed to coordinate actions across the system.
			Check list
			• Define a private static attribute in the "single instance" class.
			• Define a public static accessor function in the class.
			• Do "lazy initialization" (creation on first use) in the accessor function.
			• Define all constructors to be protected or private.
Clients may only use the accessor function to manipulate the Singleton.

###	Structural Patterns
1.	Adapter
2.	Bridge
3.	Composite
4.	Decorator
5.	Facade
6.	Flyweight
7.	Proxy

###	Behavioral Patterns
1.	Chain of Responsibility
2.	Command
3.	Interpreter
4.	Mediator
5.	Memento
6.	Observer
7.	State
8.	Strategy
9.	Template Method
10.	Visitor
11.	Model-View-Controller(MVC)

		Components
		A typical collaboration of the MVC components.
		• The model directly manages the data, logic and rules of the application.
		• A view can be any output representation of information, such as a chart or a diagram. Multiple views of the same information are possible, such as a bar chart for management and a tabular view for accountants.
		• the controller, accepts input and converts it to commands for     the model or view.

		Advantage: Display and Processing are separated. Being able to tease these components apart makes the code easier to re-use and independently test.
