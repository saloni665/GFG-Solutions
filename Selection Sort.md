## 01. Selection Sort

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/selection-sort/1)

### Problem Description

**Task:** Given an array arr, use selection sort to sort arr[] in increasing order.Examples :Input: arr[] = [4, 1, 3, 9, 7]

#### Examples

##### Example 1

- **Output:**
```text
[14, 20, 30, 31, 38]
```
- **Explanation:** Maintain sorted (in bold) and unsorted subarrays. Select 1. Array becomes 1 4 3 9 7. Select 3. Array becomes 1 3 4 9 7. Select 4. Array becomes 1 3 4 9 7. Select 7. Array becomes 1 3 4 7 9. Select 9. Array becomes 1 3 4 7 9.Input: arr[] = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-02 18:14:15
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def selectionSort(self, arr):
        n = len(arr)

        for i in range(0, n):
            min_idx = i

            for j in range(i + 1, n):
                if arr[min_idx] > arr[j]:
                    min_idx = j

            arr[i], arr[min_idx] = arr[min_idx], arr[i]

        return arr
```

*Generated on: 02/10/2026, 18:16:09*