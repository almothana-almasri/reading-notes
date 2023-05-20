[Back to Home](../README.md)

1. **Python List Comprehension:**

    List comprehension is a concise way to create lists in Python. It is a syntactic construct which creates a new list by applying an expression to each element in an iterable. It's often used for its readability and speed.

    Here's the basic syntax:
    ```
    [expression for item in iterable]
    ```
    If you want to square the elements in a given list of integers, here's how you could do it with list comprehension:
    ```
    numbers = [1, 2, 3, 4, 5]
    squares = [n**2 for n in numbers]
    ```

    This is equivalent to the following for loop:
    ```
    numbers = [1, 2, 3, 4, 5]
    squares = []
    for n in numbers:
        squares.append(n**2)
    ```
    The main difference between list comprehension and a for loop is that list comprehension is more concise and readable when you want to create a new list based on an existing one. It can also be more efficient in some cases.

2. **Decorators in Python:**

    A decorator in Python is a callable that takes another function as input and extends or modifies its behavior without explicitly modifying it. It's a powerful tool for wrapping or decorating functions or classes.

    Here's a simple decorator function example:
    ```python
    def simple_decorator(function):
        def wrapper():
            print("Before function execution")
            function()
            print("After function execution")
        return wrapper

    @simple_decorator
    def hello_world():
        print("Hello, world!")
    ```

    In this example, when you call `hello_world()`, it will print "Before function execution", then "Hello, world!", and finally "After function execution". 

    Decorators allow us to wrap another function in order to extend the behavior of the wrapped function, without permanently modifying it. Decorators are commonly used for logging, enforcing access control and authentication, instrumentation and timing functions, rate-limiting, and caching; among other things.