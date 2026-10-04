## 01. Bubble Sort

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/bubble-sort/1)

### Problem Description

**Task:** Given an array arr[]. Sort the array using bubble sort algorithm.

#### Examples

##### Example 1

- **Input:**
```text
arr[] = [4, 1, 3, 9, 7]
```
- **Output:**
```text
[1, 3, 4, 7, 9]Explanation: After Sorting the array in ascending order of their values is [1, 3, 4, 7, 9].
```

##### Example 2

- **Input:**
```text
arr[] = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]
```
- **Output:**
```text
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]Explanation: Sort the array in ascending order of their values.
```

##### Example 3

- **Input:**
```text
arr[] = [1, 2, 3, 4, 5]
```
- **Output:**
```text
[1, 2, 3, 4, 5]Explanation: An array that is already sorted should remain unchanged after applying bubble sort.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-04 15:28:25
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def bubbleSort(self,arr):
        # code here
        n = len(arr)
        for i in range(n-2, -1, -1):
            for j in range(0, i+1):
                if arr[j] > arr[j+1]:
                    arr[j],arr[j+1] = arr[j+1], arr[j]
```

*Generated on: 04/10/2026, 15:29:02*