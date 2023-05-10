# Lists

## Description
A list is an ordered data structure where each element is separated with a comma and wrapped around square brackets. A list use zero-based numbering.

The time complexity for accessing data within a list is O(N).

Lists can store multiple values under a single variable.
***

## Example Code
```python
school_subjects = ["English", "Maths", "Science", "History"]
my_numbers = [25, 45, 65, 83]
```
Lists can have mixed data types
```python
mixed_list = [25, True, "Something"]
```
***

## Usage
To create a list in Python, you use the square brackets within values separated using commas. Adding values, you use the append method to add values to the end of the list or the insert method by passing the index where to insert.

For accessing data from a list, you would use an index to retrieve a value.

Adding values, you can use this syntax:
```python 
my_numbers.append(15)
```
or
```python
my_numbers.insert(1, 15) # index, value
```
Accessing values, you can use this syntax:
```python
my_numbers[0]
```

Additional documentation can be found at [here](https://python-reference.readthedocs.io/en/latest/docs/list/).