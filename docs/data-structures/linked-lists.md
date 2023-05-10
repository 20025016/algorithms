# Linked Lists

## Description
Linked lists, linear data structure, use nodes with pointer references to the next node. Linked lists are dynamically sizeable, unlike arrays which have a fixed size.

The time complexity for accessing data within a linked list is O(√N)

GPS navigation systems can use linked lists to store the locations and routes.
***

## Example Code
```python
# Code from https://www.tutorialspoint.com/python_data_structure/python_linked_lists.htm
class Node:
   def __init__(self, dataval=None):
      self.dataval = dataval
      self.nextval = None

class SLinkedList:
   def __init__(self):
      self.headval = None

   def listprint(self):
      printval = self.headval
      while printval is not None:
         print (printval.dataval)
         printval = printval.nextval

list1 = SLinkedList()
list1.headval = Node("Mon")
e2 = Node("Tue")
e3 = Node("Wed")
# Link first Node to second node
list1.headval.nextval = e2

# Link second Node to third node
e2.nextval = e3

list1.listprint()
```
***

## Usage
To add new elements to a linked list, you must create a node object with the data you would want to be stored.
Adding to the linked list would be setting the last node's next reference pointer to the new node.

Traversing a linked list can be completed by having a variable for tracking what node you are currently up to with the linked list
to start the process, set the variable to the head node. 

Telling whether you are at the end of the linked list is done by checking if the node's next reference pointer is none. If it is not, you can set the tracking variable to the node's next reference pointer and choose to print out the data value contained within the stored node.