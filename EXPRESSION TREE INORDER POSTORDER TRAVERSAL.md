# Experiment 9(c): Expression Tree – Inorder and Postorder Traversal

## Aim
To write a Python program to build the following expression tree and print the inorder and postorder traversal.


---

## Algorithm

1. Begin the program.
2. Import the necessary modules (`build`, `Node`) from the `binarytree` package.
3. Define a list `x` representing the binary tree in pre-order format.
4. Use the `build()` function to construct the expression tree from the list.
5. Print the inorder traversal of the expression tree using `.inorder`.
6. Print the postorder traversal of the expression tree using `.postorder`.
7. End the program.

---

## Program

```
REG NO- 212223060120
NAME- KAVIYA PRIYA K
from binarytree import build,Node
x=['*',4,'-',5,'+',2,7]
t=build(x)
print(t.inorder)
print(t.postorder)
```

## OUTPUT
<img width="1203" height="167" alt="image" src="https://github.com/user-attachments/assets/62066c08-e164-46a1-ad22-888882b465c2" />


## RESULT
Thus the Python program to build the given expression tree and print the inorder and postorder traversals was created and executed successfully.
