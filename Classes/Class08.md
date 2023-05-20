# Class 08

## Q1. What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.


+ List comprehension is a way to create a new list by applying an expression to each item in an iterable. It provides a more compact and readable alternative to using a for loop to iterate over the iterable and manually append elements to the list, it allows you to create a new list in a single line, eliminating the need for initializing an empty list, writing a for loop, and appending elements manually. It offers a more concise and expressive way to generate a new list based on an existing iterable.

 + Basic syntax:

        [(expression) for item in iterable if (condition)]

 + Example :

        numbers = [1, 2, 3, 4, 5]
        squared_numbers = [x**2 for x in numbers]
        print(squared_numbers)

---

## Q2. What is a decorator in Python?

+ Decorator: a function that takes another function as input and returns a modified version of that function. It provides a convenient way to modify the behavior of functions or classes without modifying their original code.

+ Decorators are denoted by the "@" symbol followed by the name of the decorator function. They are applied to functions or classes by placing the decorator syntax on the line immediately before the function or class definition.

---

## Q3. Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.

+ Decorators in Python are a powerful feature that allows you to modify the behavior of functions or classes without changing their source code. They work by wrapping existing functions or classes with additional functionality, replacing the original with a modified version returned by the decorator. Decorators are defined as regular functions that take a function (or class) as an argument, and they are applied using the @decorator_name syntax.

### Common use cases for decorators:

1. logging
2. timing
3. caching
4. authentication
5. error handling
 

### Example:
      
        def uppercase_decorator(func):
            def wrapper():
                result = func()
                return result.upper()
            return wrapper

        @uppercase_decorator
        def greet():
            return "Hello, world!"

        print(greet())

### Output:

        HELLO, WORLD!

---

## Things I want to know more about:

+ Decorators and how to use them in the right place