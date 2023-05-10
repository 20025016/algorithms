# Stack

## Description
A stack is a linear data structure, defined by the last node entering a stack is the first one popped from a stack. 

You can access elements of a stack in the total time O(1). Requires traversing the stack.

A stack data structure is for functionality that requires going back and forth. In your browser, forward and back navigation buttons work on a stack.
***

## Example Code
```python
class Stack:
    stack = []

    def is_empty(self) -> bool:
        return self.length() == 0

    def length(self) -> int:
        return len(self.stack)

    def pop(self) -> None:
        count = self.length()
        if count == 0:
            return

        item = self.stack[-1]

        self.stack.pop()

        return item

    def push(self, value: any) -> None:
        if value is None:
            return

        if type(value) is not int:
            return

        self.stack.insert(0, value)

    def peek(self) -> any:
        if self.is_empty():
            return

        return self.stack[-1]

    def list(self) -> any:
        return self.stack

    def clear(self) -> any:
        self.stack = []

    def __str__(self) -> str:
        return f"The length of the stack is {self.length()}. The number on top is {self.peek()}."
```
***

## Usage
Adding new nodes in the stack, you would use the push method to add the node you've provided.

To remove the last node in the stack, you can use the pop method to remove the end node and return it.

To view the top node without popping a node from the stack, you can use the peek method will return the last node in the stack.