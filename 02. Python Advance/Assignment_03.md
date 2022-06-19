## PYTHON ADVANCE 3

1. What is the concept of an abstract superclass?<BR>
Ans.<br>
An abstract class can be considered as a blueprint for other classes. It allows you to create a set of methods that must be created within any child classes built from the abstract class. A class which contains one or more abstract methods is called an abstract class. An abstract method is a method that has a declaration but does not have an implementation. While we are designing large functional units we use an abstract class. When we want to provide a common interface for different implementations of a component, we use an abstract class. 

2. What happens when a class statement&#39;s top level contains a basic assignment statement?<br>
Ans.<br>
When top level of class contains a basic assignment statement, it means that a class attribute has been defined.

3. Why does a class need to manually call a superclass&#39;s `__init__` method?<br>
Ans.<br>
When a class is defined with inheritance, it inherits all methods from the superclass including `__init__` method from super class. However, when the new class is initialized with its own `__init__` function, it overrides the superclass `__init__` method. Therefore, to access the properties defined in superclass's `__init__` method, we need to manually call it.

4. How can you augment, instead of completely replacing, an inherited method?<br>
Ans.<br>
We can define the same method in the base class, which has it own properties and inherit the methods of the superclass' method using `super().method_name()`. This way we will be able to augment instead of completely replacing an inherited method.

5. How is the local scope of a class different from that of a function?<br>
Ans.<br>
The local variable defined in a function cannot be accessed outside the function. However, the local variable defined in  a class can be accesed outside the class as the class' attribute.