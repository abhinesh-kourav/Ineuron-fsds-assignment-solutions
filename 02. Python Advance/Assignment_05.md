## PYTHON ASSIGNMENT 5

1. What is the meaning of multiple inheritance?<BR>
Ans.<br>
When a class is derived from more than one base class it is called multiple Inheritance. The derived class inherits all the features of the base case.

2. What is the concept of delegation?<br>
Ans.<br>
Delegation refers to evaluating a member (property or method) of one object (the receiver) in the context of another original object (the sender).

3. What is the concept of composition?<br>
Ans.<br>
Composition is a concept that models a has a relationship. It enables creating complex types by combining objects of other types. This means that a class Composite can contain an object of another class Component.

4. What are bound methods and how do we use them?<br>
Ans.<br>
A bound method is the one which is dependent on the instance of the class as the first argument. It passes the instance as the first argument which is used to access the variables and functions.<br>
Example: `func` is a bound method.
```
class A:
    def func(self, arg):
        self.arg = arg
        print("Value of arg = ", arg)
obj = A()
```

5. What is the purpose of pseudoprivate attributes?<br>
Ans.<br>
To avoid conflicts of attribute names between classes.