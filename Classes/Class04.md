# Class 04

## Q1. What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

They key differences are:

+ A Class is a template for creating objects, and an object is an instance of a class that has its own unique state and behavior

+ Properties and Methods: A class defines a set of properties (also called attributes) and methods that are common to all instances of the class. An object can access and modify its own properties, and can call its own methods.

+ Initialization: When a new object is created, the init() method of the class is called to initialize the object's attributes. The init() method is not required, but it is commonly used to initialize the object's state.

+ Scope: Classes are defined at the module level and can be used anywhere within the module, while objects are created within the scope of a function or method.

+ Inheritance: Classes can inherit properties and methods from other classes, creating a hierarchy of related classes. Objects cannot inherit from other objects.

+ Memory Allocation: Each object created from a class is allocated its own space in memory, while the class definition is stored in the program's code memory.

---

## Q2. Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

Recursion is a programming technique where a function calls itself one or more times in order to solve a problem by breaking it into smaller subproblems. By solving the subproblems recursively, the original problem can be solved.

Here is an example of recursion to find the fibonacci of a number:

    def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

the best practices to follow when implementing recursion:
1. Test with small inputs
2. Set a base case
3. Pass parameters correctly
4. Use the call stack wisely(to avoid infinite loops)
5. Documentation

---

## Q3. What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.

+ Pytest Fixtures are used to:
1. set up preconditions
2. create objects
3. perform common to multiple tests.
4. writing more modular and reusable tests
5. Avoiding code duplication across different test cases.

+ Code coverage is used to:
1. measure of how much of the code is executed during testing.
2. Code coverage tools analyze the source code and track which lines, branches, or functions are executed during the tests.
3. identify which parts of the code are not being tested and which parts are covered by the tests. 

They can be used together to improve the quality and maintainability of a projectby :

Improved test coverage: By using fixtures to set up preconditions and provide test data, you can write more comprehensive and efficient tests. 

Better code organization: By using fixtures to encapsulate common functionality and resources, you can improve the organization and modularity of your test code.

Reusability: Fixtures can be used across multiple test cases or even across multiple test suites, making them a powerful tool for reusability.

Easier debugging: When used together with code coverage tools, fixtures can help you identify which parts of the code are not being tested or are being tested inefficiently. This can make it easier to debug errors or identify potential issues with the code.

---

## Things I want to know more about:

pytest fixtures and code coverage and how are they done in code.

