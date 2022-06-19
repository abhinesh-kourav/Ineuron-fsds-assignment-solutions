## PYTHON ADVANCE 1

1. What is the purpose of Python&#39;s OOP?<BR>
Ans.<br>
It aims to implement real-world entities like inheritance, polymorphisms, encapsulation, etc. in the programming. The main concept of OOP is to bind the data and the functions that work on that together as a single unit so that no other part of the code can access this data.

2. Where does an inheritance search look for an attribute<?BR>
Ans.<br>
A tree of linked objects.

3. How do you distinguish between a class object and an instance object?<br>
Ans.<br>
A class is a code template for creating objects. Objects have member variables and have behaviour associated with them. In python a class is created by the keyword class. An object is created using the constructor of the class. This object will then be called the instance of the class.

4. What makes the first argument in a class’s method function special?<br>
Ans.<br>
The first argument of every class method is always a reference to the current instance of the class. By convention, this argument is always named self. In the init method, self refers to the newly created object; in other class methods, it refers to the instance whose method was called.

5. What is the purpose of the `__init__` method?<br>
Ans.<br>
`__init__` method initializes the attributes defined in the class when an object of the class is created.

6. What is the process for creating a class instance?<br>
Ans.<br>
To create instances of a class, you call the class using class name and pass in whatever arguments its __init__ method accepts.<br>
`instance_name = Class_name(arg1, arg2)`

7. What is the process for creating a class?<br>
Ans.<br>
The class statement creates a new class definition.
```
class ClassName:
   class_suite
```
The class_suite consists of all the component statements defining class members, data attributes and functions including the `__init__` method.

8. How would you define the superclasses of a class?<br>
Ans.<br>
When a class inherits some or all of the behaviors from another class, that another class is known as superclass.