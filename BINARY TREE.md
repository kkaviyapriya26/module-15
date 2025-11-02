# Experiment 9(a): Binary Tree (Float Values)

## Aim
To write a Python program to build a binary tree with a root, left, and right node using float values.

---

## Algorithm

1. Start the program.
2. Import the `Node` class from the `binarytree` module.
3. Create a root node using the `Node` class and input a floating-point value for the root.
4. Create left and right child nodes for the root using floating-point values.
5. Convert the binary tree to a list.
6. Print the list of nodes.
7. End the program.

---

## Program

```
Reg.no:212223060120
name: KAVIYA PRIYA K

from binarytree import Node
l=[]
for i in range(0,3):
   a=float(input())
   l.append(a)
root=Node(l[0])
root.left=Node(l[1])
root.right=Node(l[2])
print("List of nodes :",list(root))
```

### OUTPUT
<img width="731" height="133" alt="image" src="https://github.com/user-attachments/assets/46f17582-0678-4d14-93d3-ac1dddfff0f2" />

## RESULT
Thus the Python program to build a binary tree with a root, left, and right node using floating-point values has been implemented and executed successfully.
