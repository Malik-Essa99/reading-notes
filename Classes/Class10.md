# Class 10

## Q1. What are the key features and benefits of Jupyter Lab, and how does it differ from Jupyter Notebook?


+ Jupyter Lab offers a more versatile and flexible environment compared to Jupyter Notebook, with a powerful user interface, advanced layout options, integrated text editor, extensibility through extensions, command palette for quick access to commands, an integrated terminal, and improved cell tools. These features make Jupyter Lab a highly productive and customizable environment for interactive computing and data exploration.

---

## Q2. What are the main functionalities provided by the NumPy library, and how can it be useful in Python programming, particularly for scientific computing and data manipulation tasks?

NumPy is a fundamental library for scientific computing and data manipulation in Python. Its multi-dimensional arrays, mathematical functions, broadcasting capabilities, array indexing and slicing, integration with other libraries, efficient data storage, and performance optimization features make it a valuable tool for a wide range of tasks, including numerical simulations, data analysis, machine learning, image processing, and more.

Main functionalities provided by the NumPy:

+ Multi-dimensional Arrays
+ Mathematical Operations
+ Broadcasting
+ Array Indexing and Slicing
+ Integration with other Libraries
+ Efficient Data Storage
+ Performance Optimization

---

## Q3. Explain the basic structure and properties of NumPy arrays, and provide examples of how to create, manipulate, and perform operations on them.

NumPy array is a grid of elements, all of the same data type, indexed by a tuple of nonnegative integers. The number of dimensions of the array is known as its rank, and the shape of the array is a tuple of integers that specifies the size of each dimension


Creating NumPy Arrays Example: 

        import numpy as np

        arr1 = np.array([1, 2, 3, 4, 5])


        

Manipulating and Performing Operations on NumPy Arrays:

        import numpy as np
        # Manipulating arrays
        arr = np.array([1, 2, 3, 4, 5])

        # Accessing elements
        print(arr[0])  # Output: 1
        print(arr[1:4])  # Output: [2, 3, 4]

        # Modifying elements
        arr[2] = 10
        print(arr)  # Output: [1, 2, 10, 4, 5]

        # Performing mathematical operations
        arr = np.array([1, 2, 3, 4, 5])

        # Element-wise addition
        result = arr + 2
        print(result)  # Output: [3, 4, 5, 6, 7]

        # Element-wise multiplication
        result = arr * 3
        print(result)  # Output: [3, 6, 9, 12, 15]

        # Matrix multiplication
        matrix = np.array([[1, 2], [3, 4]])
        result = np.matmul(matrix, matrix)
        print(result)  # Output: [[7, 10], [15, 22]]


