# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

---

## PROGRAM:

```
from binarytree import Node

def _build_bst_from_sorted_values(sorted_values):
    if (len(sorted_values))==0:
        return None
    mid = len(sorted_values)//2
    root = Node(sorted_values[mid])
    root.left = _build_bst_from_sorted_values(sorted_values[:mid])
    root.right = _build_bst_from_sorted_values(sorted_values[mid+1:])
    return (root)


def right_subtree(l):
    print("Right Subtree :")
    for i in l[2].values:
        print(i,"-->",end="")
    return 


a=[]
n = int(input())
for i in range (n):
    x = int(input())
    a.append(x)
p = sorted(a)
l = _build_bst_from_sorted_values(p)
print("Postorder :",l.postorder)
right_subtree(l)
print("\nIs this a Binary Search Tree? ",l.is_bst)
```

## OUTPUT
``
<img width="738" height="343" alt="{2362561F-FEB7-4B1C-9AF2-FB8EB2A3741F}" src="https://github.com/user-attachments/assets/5bb2c07c-bc22-49c1-9cdc-ddbbf8c555c1" />

```

## RESULT
```
Thus, the Python program to build a binary search tree using a built-in function was successfully implemented and verified.
