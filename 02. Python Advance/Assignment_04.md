## PYTHON ADVANCE 4

1. Which two operator overloading methods can you use in your classes to support iteration?<BR>
Ans.<br>
`__iter__` and `__next__`

2. In what contexts do the two operator overloading methods manage printing?<br>
Ans.<br>
`__str__` and `__repr__` are the overloading methods to manage printing.<br>
`__str__` is used for creating output for end user while `__repr__` is mainly used for debugging and development. repr’s goal is to be unambiguous and str’s is to be readable.

3. In a class, how do you intercept slice operations?<br>
Ans.<br>
In a class, use of slice() with `__getitem__` method is used for intercepting slice operation. This slice method is provided with start integer number, stop integer number and step integer number.<br>
Example: `__getitem__(slice(start,stop,step))`<br>

4. In a class, how do you capture in-place addition?<br>
Ans.<br>
`__iadd__` magic method is used to capture in-place addition in a class.

5. When is it appropriate to use operator overloading?<br>
Ans.<br>It is appropriate to use operator overloading of our classes when we want to provide more meaning to an operator than its originally defined.