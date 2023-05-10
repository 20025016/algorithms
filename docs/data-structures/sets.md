# Sets

## Description
Sets data structures are unordered and require values stored within to be unique, but there are no restrictions on how many data values are present.

Sets in Python use hash tables, so the time complexity for accessing elements would be the access time complexity would be O(1) as finding the location of the stored value is constant time.

Sets are for removing duplicated values.
***

## Example Code
```python
# Code from https://www.programiz.com/python-programming/set
# create a set of integer type
student_id = {112, 114, 116, 118, 115}
print('Student ID:', student_id)

# create a set of string type
vowel_letters = {'a', 'e', 'i', 'o', 'u'}
print('Vowel Letters:', vowel_letters)

# create a set of mixed data types
mixed_set = {'Hello', 101, -2, 'Bye'}
print('Set of mixed data types:', mixed_set)
```
***

## Usage
To create a set, use curly braces with the data separated by commas. But using empty curly braces will
create an empty dictionary. Creating an empty set without using the set class isn't possible.

Python sets come with all the needed methods for accessing and inserting new data. The update method can add data from lists, tuples, and sets quickly and easily.

Additional documentation for set methods is [here](https://python-reference.readthedocs.io/en/latest/docs/sets).