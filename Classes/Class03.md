# FileIO & Exceptions

## Q1. What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?



+ It makes sure that the file is automatically closed when the block of with statement is excuted, therefore it contributes to avoid file corrcuption that can happen if the file is not closed properly.

---

## Q2. Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

### 1. readline()
+ It reads a single line everytime of the file, therefore it's better to use it when dealing with large sized files

### Example: 

    with open('file.txt', 'r') as f:
        line = f.readline()
        while line:
            print(line)
            line = f.readline()
    
### 2. read()
+ It reads all the contents (lines) of the file, so its useful when trying to read a small sized file

### Example:

    with open('file.txt', 'r') as f:
        data = f.read()
        print(data)
    
---

## Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.

 Exception handling is a way to handle errors that may occur during the execution of a program. They are raised when the interpreter encounters an error that it can't handle, such as a syntax error, a division by zero, or a file that does not exist. Without exception handling, it's necessary to use exceptions because otherwise it would cause the program to crash if any of these errors occur.
  

### Example:

    try:
        x = 1 / 0
    except zero_division_error:
        print("Error: Division by zero!")
    finally:
        print("This code always runs.")

In the example above:

+ (try) block: contains the code that may raise an exception (Devision by Zero)

+ (except) block: is used to catch and handle the exception 

+ (finally) block: is used to execute the code that should run at all times, regardless of whether an exception is raised or not.


---

## Things I want to know more about:
Exceptions and how to use them on a real life example code.

