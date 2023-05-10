# Hash Tables

## Description
Hash tables use arrays to store information behind the scenes. A hashing function is required to generate an index from a key. The hash table uses this index to store the data in an array.

The time complexity for accessing data within a hash table is O(1). Since the data is in an array accessing is quick.

Hash tables are used in databases to generate indexes to locate data quickly without traversing the table again.

In Python, dictionaries use hash tables.
***

## Example Code
```python
car1 = {
    "brand": "McLaren",
    "model": "Senna",
    "year": 2018
}

print(car1["brand"])

car2 = {
    "brand": "Lamborghini",
    "model": "Aventador",
    "year": 2022
}

print(car2["year"])
```
***

## Usage
To create dictionaries in Python, you can use curly braces with a string for the key on the left side, separated by a colon and the value you want to store on the right. Separate each entry with a comma.

Accessing values from a Python dictionary uses the variable name with having a key surrounded by square brackets. The key must be a string.
```python
my_dict["something"]
```

Adding values is the same syntax as above. Assign the value you want to be stored.
```python
my_dict["something"] = 123
```

Additional documentation can be found at [here](https://docs.python.org/3/library/stdtypes.html#dict)