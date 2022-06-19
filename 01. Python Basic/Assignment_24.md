## PYTHON BASIC ASSIGNMENT 24

1. What is the relationship between def statements and lambda expressions?<br>
Ans.<br>
A lambda function is a small anonymous function. A lambda function can take any number of arguments, but can only have one expression. 

2. What is the benefit of lambda?<br>
Ans.<br>
i. Lambda functions reduce the number of lines of code when compared to normal python function.
ii. They are generally used when a function is needed temporarily for a short period of time.
iii. Using lambda function, you can define a function and call it immediately at the end of definition.

3. Compare and contrast map, filter, and reduce.<br>
Ans.<br>
map creates a new list by transforming every element in an iterable individually.<br>
filter creates a new list by removing elements from an iterable that fail a condition.<br>
reduce takes all of the elements in an iterable and reduces them into a single value.

4. What are function annotations, and how are they used?<br>
Ans.<br>
Function annotation is the standard way to access the metadata with the arguments and the return value of the function. These are nothing but some random and optional Python expressions that get allied to different parts of the function. They get evaluated only during the compile-time and have no significance during the run-time of the code. They do not have any significance or meaning associated with them until accessed by some third-party libraries. They are used to type check the functions by declaring the type of the parameters and the return value for the functions. The string-based annotations help us to improve the help messages.
Syntax:
```
    def func(a: 'int') -> 'int':
        pass
```
Annotations for simple parameters:
```
    def func(x: 'float'=10.8, y: 'argument2'):
        In the above code the argument, ‘x’ of the function func, has been annotated to float data type and the argument ‘y’ has a string-based annotation. The argument can also be assigned to a default value using a ‘=’ symbol followed by the default value. These default values are optional to the code.
```
Annotations for return values:
```
    def func(a: expression) -> 'int':
        The annotations for the return value is written after the ‘->’ symbol.
```

5. What are recursive functions, and how are they used?<br>
Ans.<br>
Recursion means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result.
```
def fact(x):
    if x == 1 :
        return 1
    else :
        return x * fact(x-1)
    
fact(3)
```
Output:<br>
`6`

6.  What are some general design guidelines for coding functions?<br>
Ans.<br>
i. Use 4-space indentation and no tabs.<br>
ii. Use docstrings<br>
iii. Wrap linethat they don’t exceed 79 characters<br>
iv. Use of regular and updated comments are valuable to both the coders and users<br>
v. Use of trailing commas : in case of tuple -> ('good',)<br>
vi. Use Python’s default UTF-8 or ASCII encodings and not any fancy encodings<br>
vii. Naming Conventions<br>
viii. Characters that should not be used for identifiers : ‘l’ (lowercase letter el), ‘O’ (uppercase letter oh), ‘I’   (uppercase letter eye)<br>
ix. Don’t use non-ASCII characters in identifiers<br>
x. Name your classes and functions consistently while naming of function of methods always use self for the first argument<br>

7. Name three or more ways that functions can communicate results to a caller.<br>
Ans.<br>
i. Function can return single value<br>
ii. Can return multiple values, tuple<br>
iii. can return list,dictionary<br>
iv. can return function object<br>
v. can return class object<br>