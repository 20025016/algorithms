# Queues

## Description
A queue is a linear data structure where the first node is the first to leave.

The time complexity for accessing elements is 0(N). Traversing the queue is necessary to access a node.

A queue data structure multi-threading relies on queues to ensure operations are successful.
***

## Example Code
```python
# Code example from https://www.geeksforgeeks.org/queue-in-python/
# Python program to 
# demonstrate queue implementation
# using list
  
# Initializing a queue
queue = []

# Adding elements to the queue
queue.append('a')
queue.append('b')
queue.append('c')
  
print("Initial queue")
print(queue)
  
# Removing elements from the queue
print("\nElements dequeued from queue")
print(queue.pop(0))
print(queue.pop(0))
print(queue.pop(0))
  
print("\nQueue after removing elements")
print(queue)
  
# Uncommenting print(queue.pop(0))
# will raise and IndexError
# as the queue is now empty
```
***

## Usage
In the example code, you can use a list to provide the storage functionality for the queue. 

Lists provide the functionality required to add and remove nodes from a queue.