# Topic: Binary Search

## Overview

Binary Search is an efficient algorithm for finding an item in a sorted array...

## Key Points

- O(log n) complexity
- Requires sorted input
- Divide-and-conquer method

## Example (Python)

```python
def binary_search(arr, x):
    l, r = 0, len(arr) - 1
    while l <= r:
        mid = (l+r)//2
        if arr[mid] == x:
            return mid
        elif arr[mid] < x:
            l = mid+1
        else:
            r = mid-1
    return -1
