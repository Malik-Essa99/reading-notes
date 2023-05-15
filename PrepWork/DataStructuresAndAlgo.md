## Introduction :
 Understanding data structures and Big O notation can help us write more efficient and optimized code, which can have a significant impact on the performance of our programs. Python has many built-in data structures, such as lists, tuples, sets, and dictionaries, as well as libraries for more specialized data structures such as arrays and trees. By understanding the characteristics and time complexities of these data structures, we can choose the best one for a particular task and optimize our program's performance.

---

## Q. What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

 An important factor to pay attention to when choosing which data structure to use with a specific problem is efficiency. Each data structure is suitable for problems more than others, therefore choosing the right structure can greatly impact the performance of the solution for the problem.

 Another thing to consider is the space complexity of the structure, as some structures may have smaller memory usage than others but may come at the cost of slower operations or increased complexity.

---

## Q. How can we ensure that we’ll avoid an infinite recursive call stack?

 By setting a base case, it's a condition that stops the recursion. It's important to have a base case that can be reached eventually, or else the recursion will continue infinately.

---

## Summary:
Recursion is a programming technique where a function calls itself repeatedly until a certain condition is met. When a function is called, it executes its code and can call itself to repeat the process. The function continues to call itself until it reaches a base case, which is a condition that stops the recursion. 

pseudocode is a high level description of the problem you are trying to solve in code, it's written like code but it's meant to be closer to human language.

compound Data: data items taht are grouped together in a meaningful way, they are stored in a data structure.

BigO notation : Measurement of how well an operation scales.


## Data structures
No data structure is perfect, each one has it's uses

### Linked List:

Each list item has a value and a pointer and are called (Nodes).
pros:

+ adding new items
+ deleting items

cons:
- getting items
- searching items

### Array: []

Is a coninious block of cells in computer memory.
pros:

+ getting items

cons:
- adding items (sometimes)

### Hash Tables: {}

like objects, tuples, sets, and dictionaries...

pros:

+ adding items
+ getting items

cons:
- Collisions which is two keys hashing to the same memory location


### Stacks and Queues:

Stacks: Last in first out
Queues: First in first out

pros:

+ Efficient addition and removal

cons:
- limited use cases

### Groups & Trees:

It's shaped like a tree of nodes taht are pointing at each other in one direction from parent to child, they have rules though:
1. they can only have from 0 to 2 children
2. left < right 
3. right > left

pros:

+ Indicators to where specific data might be

cons:
- could become unbalanced easily

---

## Things I want to know more about

+ Recursion in action
+ Digging deep into BigO Notation
+ Groups and trees
