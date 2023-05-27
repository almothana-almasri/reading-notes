[Back to Home](../README.md)

## **Jupyter Lab**

Jupyter Lab is an enhanced interactive development environment (IDE) that provides a flexible and powerful environment for working with Jupyter Notebooks, as well as other computational workflows.

- **Multiple Document Interface (MDI)**: Unlike Jupyter Notebook, Jupyter Lab supports a multiple document interface where you can open multiple notebooks and files simultaneously, making it easier to work on different tasks at once.

- **Enhanced Text Editor**: Jupyter Lab provides a text editor with features like syntax highlighting, code folding, and line numbering, making it more convenient for writing and editing code.

- **Integrated Terminal**: Jupyter Lab includes an integrated terminal that allows you to run shell commands and interact with the underlying system directly from the interface.

- **Drag-and-Drop Functionality**: Jupyter Lab allows you to drag and drop files and notebooks, making it easier to organize and manage your files within the environment.


While Jupyter Lab offers a more advanced interface and additional features, Jupyter Notebook remains a popular choice for simpler workflows or for those who prefer the classic interface.

## **NumPy library**

NumPy (Numerical Python) is a powerful library for numerical computing in Python. It provides an efficient way to work with large, multi-dimensional arrays and perform mathematical operations on them.

- **Array Manipulation**: NumPy provides functions for reshaping, splitting, joining, and manipulating arrays. You can change the shape of an array, extract specific elements or subarrays, and concatenate arrays along different axes.

- **Random Number Generation**: NumPy has a random module that allows you to generate random numbers with various probability distributions. This is useful for simulations, generating random data, or testing algorithms.

- **Performance Optimization**: NumPy is implemented in C and provides efficient, optimized functions for numerical operations. It leverages the underlying hardware capabilities and allows you to perform computations much faster compared to pure Python loops.

NumPy is widely used in scientific computing, data analysis, machine learning, and other fields where efficient numerical operations and array manipulation are required.

## **NumPy arrays**

NumPy arrays, represented by the `ndarray` object, are the fundamental data structure in the NumPy library.

- **Shape**: The shape of an array refers to the dimensions and sizes of each dimension. It is represented as a tuple of integers. For example, a 1D array of size 5 has a shape of `(5,)`, a 2D array of size 3x4 has a shape of `(3, 4)`, and a 3D array of size 2x3x4 has a shape of `(2, 3, 4)`.

- **Data Type**: NumPy arrays are homogeneous, meaning all elements must have the same data type. The data type of an array is specified when it is created and can be accessed using the `dtype` attribute. Common data types include `int`, `float`, `bool`, and `complex`, with different bit sizes available.

- **Size**: The size of an array refers to the total number of elements in the array. It can be calculated by multiplying the sizes of all dimensions together.

```python
import numpy as np

# Creating arrays
a = np.array([1, 2, 3])                # 1D array
b = np.array([[1, 2, 3], [4, 5, 6]])  # 2D array

# Array properties
print(a.shape)      # Output: (3,)
print(b.shape)      # Output: (2, 3)
print(b.dtype)      # Output: int64
print(b.size)       # Output: 6
```