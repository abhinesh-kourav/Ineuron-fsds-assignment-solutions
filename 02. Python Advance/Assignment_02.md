## PYTHON ADVANCE 2

1. What is the relationship between classes and modules?<BR>
Ans.<br>
Both class and modules have their own attributes that define them. In addition, both of them can have their own methods, variables and classes.

2. How do you make instances and classes?<br>
Ans.<br>
The class statement creates a new class definition.<br>
`class ClassName:`<br>
`   class_suite`<br>
The class_suite consists of all the component statements defining class members, data attributes and functions including the `__init__` method.<br>
To create instances of a class, you call the class using class name and pass in whatever arguments its `__init__` method accepts.<br>
`instance_name = ClassName(arg1, arg2)`

3. Where and how should be class attributes created?<br>
Ans.<br>
Class attributes are the variables defined directly in the class that are shared by all objects of the class.<br>
`class ClassName():`<br>
`    attri = 0`<br>
In the above example, `attri` is an attribute in the `ClassName` class.

4. Where and how are instance attributes created?<br>
Ans.<br>
Instance attributes are defined inside the `__init__` method when the class is defined.<br>
`class ClassName():`<br>
`   def __init__(self,a,b,c):`<br>
`        self.a = a`<br>
`        self.b = b`<br>
`        self.c = c`<br>
`instanceName = ClassName(1,'abc',True)`<br>
Instance attributes are created when an object of the class is created with attributes passed as arguments.

5. What does the term &quot;self&quot; in a Python class mean?<br>
Ans.<br>The first argument of every class method is always a reference to the current instance of the class. By convention, this argument is always named self. In the init method, self refers to the newly created object; in other class methods, it refers to the instance whose method was called.

6. How does a Python class handle operator overloading?<br>
Ans.<br>
To handle operator overloading, Python provides some special function or magic function that is automatically invoked when it is associated with that particular operator. For example, when we use + operator, the magic method `__add__` is automatically invoked in which the operation for + operator is defined. There by changing this magic method’s code, we can give extra meaning to the + operator.

7. When do you consider allowing operator overloading of your classes?<br>
We comsider allowing operator overloading of our classes when we want to provide mpre meaning to an operator than its originally defined.

8. What is the most popular form of operator overloading?<br>
Ans.<br>
The most popular and convenient example is the Addition (+) operator. Just think how the '+' operator operates on two numbers and the same operator operates on two strings. It performs “Addition” on numbers whereas it performs “Concatenation” on strings. It can also 'merge' two lists. It is achievable because ‘+’ operator is overloaded by int class and str class.

9. What are the two most important concepts to grasp in order to comprehend Python OOP code?<br>
Ans<br>
Inheritance and Polymorphism.