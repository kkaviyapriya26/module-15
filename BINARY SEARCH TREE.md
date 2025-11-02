# Experiment 9(b): Binary Search Tree

## Aim
To write a Python program to build a Binary Search Tree (BST) using a built-in function.

---

## Algorithm

1. Start the program.
2. Import the `Node` class from the `binarytree` module.
3. Define a function `_build_bst_from_sorted_values()` to build a BST recursively from a sorted list.
4. Define a function `left_subtree()` to print the values in the left subtree of the BST.
5. Accept input from the user for the number of elements.
6. Read the elements into a list.
7. Sort the list.
8. Build the BST by calling `_build_bst_from_sorted_values()` with the sorted list.
9. Print the postorder traversal of the BST.
10. Print the left subtree values.
11. Check and print whether the built tree is a Binary Search Tree.
12. End the program.

---

## Program

```
Reg.No:212223060120
Name: KAVIYA PRIYA K
from binarytree import Node
def _build_bst_from_sorted_values(sorted_values):
    if len(sorted_values) == 0:
        return None
    mid_index = len(sorted_values) // 2
    root = Node(sorted_values[mid_index])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right = _build_bst_from_sorted_values(sorted_values[mid_index + 1 :])  
    return (root)

def left_subtree(l):
  print("Left Subtree : ")
  for i in l[1].values:
    print(i,"-->",end="")
  return 

a=[]
size=int(input())
for i in range(0,size):
  val=int(input())
  a.append(val)
x=sorted(a)


l=_build_bst_from_sorted_values(x)
print("Postorder :",l.postorder)
left_subtree(l)
print("\nIs this a Binary Search Tree? ",l.is_bst)


```

## OUTPUT
<img width="1769" height="540" alt="image" src="https://github.com/user-attachments/assets/be51cdf9-674d-4d4b-a7ef-7cbb45522732" />

## RESULT
Thus, the Python program to build a binary search tree using a built-in function is implemented and executed successfully.
