# Ex. No: 15D - Build a Heap Tree Using Python

## AIM:
To write a Python program to build a heap tree using appropriate Python package and function.

---

## ALGORITHM:

1. **Start the program.**
2. Import the `heapq` module.
3. Define a function `heaptree(H)` that takes a list `H` as input.
4. Use `heapq.heapify(H)` to convert the list into a min-heap.
5. Print the created heap.
6. **End the program.**

---

## PROGRAM:

```
from binarytree import heapq,build,Node
def heaptree(L):
    nodes=L
    root=build(nodes)
    for i in root.values:
        print(i,"-->",end="")
    print("\nHeight : ",root.height)
    print("Is max heap? : ",root.is_max_heap)
    print("Is complete tree? : ",root.is_complete)

```

## OUTPUT
``
<img width="789" height="163" alt="{83685B8D-9C1A-42A6-BCEB-7634674EB24E}" src="https://github.com/user-attachments/assets/78f4bb5b-1c4c-4793-a38e-ea5aa92afff6" />

```

## RESULT
```
Thus, the Python program to build a heap tree using appropriate Python package and function was successfully implemented and verified.
