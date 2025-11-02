# Experiment 9(e): Expression Tree Evaluation

## Aim
To write a Python program to build and evaluate the given expression tree.

---

## Algorithm

1. Start the program.
2. Create nodes for operators and operands.
3. Build the expression tree by connecting the nodes in the correct hierarchical structure.
4. Define a recursive function `evaluate(root)`:
   - If the node is a number (leaf), return it as a float.
   - Else, recursively evaluate the left and right subtrees.
   - Apply the operator at the current node to the results.
5. Return the final result from the root node.
6. End the program.

---

## Program

```
REG NO- 212223060120
NAME- KAVIYA PRIYA K
from binarytree import Node
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

def isLeaf(node):
    return node.left is None and node.right is None
 
def process(op, x, y):
    if op == '+':
        return x + y
    if op == '-':
        return x - y
    if op == '*':
        return x * y
    if op == '/':
        return x / y
 
def evaluate(root):
    if root is None:
        return 0
    if isLeaf(root):
        return float(root.val)
    x=evaluate(root.left)
    y=evaluate(root.right)
    return process(root.val,x,y)

root=Node('*')
root.left=Node('+')
root.right=Node('+')
root.left.left=Node(7)
root.left.right=Node(6)
root.right.left=Node(2)
root.right.right=Node(6)
print("The value of the expression tree is",evaluate(root))
```

## OUTPUT
<img width="1137" height="151" alt="image" src="https://github.com/user-attachments/assets/0f2064c7-1af2-4cb4-9d60-6b6e2fbffd30" />


## RESULT
Thus the Python program to build and evaluate the given Expression tree was successfully executed.
