# Class 07

## Q1. Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

It can be described as the visibility and accessibility of variables within different parts of a program. It defines where a variable can be accessed.

+ Local Scope: Variables defined within a specific block or function have local scope. They can only be accessed within that block or function. Local variables are created when the block or function is entered and are deleted when the block or function is exited. Local variables take precedence over variables with the same name in the global scope.

Here's an example on local scope:

    def my_function():
        x = 10  
        print(x)

    my_function()  
    print(x)  


+ Global Scope: Variables defined outside any function or block have global scope. They can be accessed from anywhere in the program, including within functions. Global variables remain in memory throughout the program's execution.

Here's an example on global scope:


    y = 20  

    def my_function():
        print(y)

    my_function()  
    print(y)  


---


## Q2. How do the global and nonlocal keywords work in Python, and in what situations might you use them?

Global Keyword:
The global keyword is used to declare that a variable is a global variable, even if it is assigned a value within a function.

+ Usage:  Global keyword is used to access and modify global variables from within a local scope, such as inside a function

Nonlocal Keyword:
The nonlocal keyword is used to declare that a variable is nonlocal, which means it is not local to the current function but is defined in an enclosing function.

+ Usage: Nonlocal keyword is used to access and modify variables in an outer scope within a nested 

---

## Q3. In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

+ It's an important tool in algorithm analysis, as it allows us to compare and evaluate an algorithm's performance, in addition it gives us information on which algorithm to use when solving a specific problem to optimize the efficiency and performance of our code.

---

## Q4. Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.

+ Define the function roll_dice(): This function will simulate the dice roll and return a random number between 1 and 6 (inclusive) to represent the face of the rolled dice.

+ calculate the probability: rolling a specific number  (1,6), you can perform the it for a large number of trials and count the occurrences of the target number.

+ Determine the target number you want and Specify the number of trials you want, then run a loop for the specified number of trials. Inside the loop, call the roll_dice() function to get a random number representing a dice roll. then check if the rolled number matches the target number. If it does, count++.

+ Calculate the probability: Divide the count of occurrences of the target number by the total number of trials to calculate the probability.


Example :
    import random

    target_number = 6
    num_trials = 1000000
    count = 0

    for _ in range(num_trials):
        result = random.randint(1, 6)
        if result == target_number:
            count += 1

    probability = count / num_trials


## Things I want to know more about:


+ Doubly linkedlists and how to maximize the benifit from using them
+ How to deal with Large scale games logic with python
+ Nonlocal variables and use them in code
