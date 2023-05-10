# Arrays

## Description
An array is a linear data structure stored in a contiguous memory block. Each value is adjacent to one another. 

The time complexity for accessing data within an array is O(1).

Arrays can store multiple data values under a single variable.
***

## Example Code
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)

print(type(arr))
```
***

## Usage
Creating an array requires using either NumPy or an inbuilt Python array class. NumPy arrays are simple, initiate the array class and pass the values to be stored.

Accessing data from a NumPy array requires an index of the value stored, the same method of accessing a list.

Additional Numpy array documentation is [here](https://numpy.org/doc/stable/reference/arrays.html).

Python array documentation is [here](https://docs.python.org/3/library/array.html).