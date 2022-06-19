## PYTHON BASIC ASSIGNMENT 25

1. What is the difference between enclosing a list comprehension in square brackets and parentheses?<BR>
Ans.<br>
Enclosing in square brackets produces a list while enclosing in parentheses produces a generator.

2. What is the relationship between generators and iterators?<br>
Ans.<br>
Generators are another way of creating iterators in a simple way where it uses the keyword “yield” instead of returning it in a defined function. The yield function returns the data without affecting or exiting the function.

3. What are the signs that a function is a generator function?<br>
Ans.<br>
If a function contains at least one yield statement, it becomes a generator function. Both yield and return will return some value from a function.

4. What is the purpose of a yield statement?<br>
Ans.<br>
A yield statement looks much like a return statement, except that instead of stopping execution of the function and returning, yield instead provides a value to the code looping over the generator and pauses execution of the generator function.

5. What is the relationship between map calls and list comprehensions? Make a comparison and contrast between the two.<br>
Ans.<br>
Both list comprehension and map function result in a list produced by applying some function over the elements of an already existing list.<br>
Comparision :<br>
    i. List comprehension is more concise and easier to read as compared to map<br>
    ii. List comprehension allows filtering. In map, we have no such facility For example, to print all even numbers in range of 100, we can write [n for n in range(100) if n%2 == 0]. There is no alternate for it in map<br>
    iii. List comprehension are used when a list of results is required, where as map only returns a map object and does not return any list.<br>
    iv. List comprehension is faster than map when we need to evaluate expressions that are too long or complicated to express<br>
    iv. Map is faster in case of calling an already defined function (as no lambda is required)<br>
