# Trees

## Description
The data structure represents a tree. Organising data in this way makes it easy to navigate and search through. The tree consists of nodes and branches. Each node can only have one parent.

The time complexity for accessing elements is 0(N). Traversing the tree is necessary to access a node.

Data compression uses binary trees to provide efficient storage space optimisation.
***

## Example Code
```python
# Code example from https://www.tutorialspoint.com/python_data_structure/python_binary_tree.htm 
class Node:
    def __init__(self, data):
        self.left = None
        self.right = None
        self.data = data

    # Insert Node
    def insert(self, data):
        if self.data:
            if data < self.data:
                if self.left is None:
                    self.left = Node(data)
                else:
                    self.left.insert(data)
            elif data > self.data:
                if self.right is None:
                    self.right = Node(data)
                else:
                    self.right.insert(data)
        else:
            self.data = data

    # Print the Tree
    def PrintTree(self):
        if self.left:
            self.left.PrintTree()
        print(self.data)
        if self.right:
            self.right.PrintTree()

    # Inorder traversal
    # Left -> Root -> Right
    def inorderTraversal(self, root):
        res = []
        if root:
            res = self.inorderTraversal(root.left)
            res.append(root.data)
            res = res + self.inorderTraversal(root.right)
        return res


root = Node(27)
root.insert(14)
root.insert(35)
root.insert(10)
root.insert(19)
root.insert(31)
root.insert(42)
print(root.inorderTraversal(root)) 
```
***

## Usage
Creating a tree requires a starting point node. You can use the insert method for adding additional nodes, which will check whether the data should go on the left or right.

Printing out values uses the inorder traversal way of navigating a tree once done, it will print out an array with the data stored in the nodes.