# Class 09

## Q1. What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method.

+ methods, also known as special or magic methods, in Python provide a way to define the behavior of built-in operations or functionalities for objects of a class. They are enclosed within double underscores on both sides of the method name.

One commonly used dunder method is __str__(), which allows customization of the string representation of an object. By implementing this method, you can define how an object should be represented as a string when using functions like str() or when the object is printed.

Dunder methods serve the purpose of making objects more intuitive and compatible with Python's built-in functionalities. They can be used to define behaviors for mathematical operations, container operations, comparison operations, and more. These methods enable you to tailor the behavior of objects to suit your specific needs and make your code more expressive and readable.

---

## Q2. In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?

+ plagiarism, the main ethical is the potential misuse of developers' work without proper attribution or compensation. The AI Guru in question appears to have used the work of developers to create a paid course, misleadingly presenting it as their own original content.

---

## Q3. Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.

+ Python statistics module is a built-in module that provides functions for performing various statistical operations. It allows you to calculate measures such as mean, median, mode, variance, standard deviation, and more. One example of a function within the module is statistics.mean(), which calculates the mean (average) of a list of numbers.

### Here's an example:

    import statistics

    data = [2, 4, 6, 8, 10]
    mean_value = statistics.mean(data)
    print(mean_value)

