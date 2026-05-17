# MSCS532_Assignment1
Data Structure and Algorithm - Insertion Sort Algorithm that sorts in monotonically decreasing order

## Code
 
```python
def insertion_sort(arr: list) -> list:
    for i in range(1, len(arr)):
        key = arr[i]        # Element to be positioned
        j = i - 1           # Compare with element just before key
 
        # Shift smaller elements right to make room
        while j >= 0 and arr[j] < key:
            arr[j + 1] = arr[j]
            j -= 1
 
        arr[j + 1] = key    # Drop key into its correct spot
 
    return arr
```
 
---
 
## What It Does
 
Iterates through the list, taking each element (`key`) and sliding it leftward past any elements smaller than itself. The result is a **monotonically decreasing** sequence.
