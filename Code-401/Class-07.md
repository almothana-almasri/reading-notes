[Back to Home](../README.md)

1. **Variable Scope in Python (Local vs Global Scope):** The scope of a variable refers to the places in your code where you can access that variable. If a variable is defined inside a function, it's a local variable and it can only be used within that function. If it's defined outside all functions, it's a global variable and it can be used by any function in the script. For example:
```python
x = 10  # This is a global variable

def my_func():
    y = 5  # This is a local variable
    print(x)  # This will print 10
    print(y)  # This will print 5

my_func()
print(x)  # This will print 10
print(y)  # This will raise an error because y is local to my_func
```

2. **Global and Nonlocal Keywords:** The `global` keyword in Python is used to indicate that a variable is a global variable, even if it's being used inside a function. The `nonlocal` keyword is used in nested functions to indicate that a variable is in the nearest enclosing scope that is not global. You might use `global` if you need to modify a global variable from within a function, and `nonlocal` if you need to modify a variable in an outer (but not global) scope.

3. **Big O Notation:** Big O notation is used in computer science to describe the performance of an algorithm. Specifically, it describes how the run time or memory requirements of an algorithm grow as the size of the input grows. This helps us to understand the worst-case scenario for an algorithm's performance, which is crucial when dealing with large datasets. For example, an algorithm with a time complexity of O(n) will have its runtime increase linearly with the size of the input, while an algorithm with a time complexity of O(n²) will see its runtime increase quadratically.

4. **Simulating a Dice Roll:** To simulate a dice roll in Python, you can use the `random` module's `randint` function, which returns a random integer between the two arguments you pass to it. For a six-sided dice, you'd use `random.randint(1, 6)`. To calculate the probability of rolling a specific number over a large number of trials, you'd count the number of times you roll that number and divide by the total number of trials. For example:
```python
import random

rolls = 1000000
six_count = 0

for _ in range(rolls):
    if random.randint(1, 6) == 6:
        six_count += 1

print(f"Probability of rolling a 6: {six_count / rolls}")
```
This code will give an estimate of the probability of rolling a 6, which should be close to the theoretical probability of 1/6.