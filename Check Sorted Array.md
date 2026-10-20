## 01. Check Sorted Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-if-an-array-is-sorted0701/1)

### Problem Description

**Task:** Given an array arr[], check whether it is sorted in non-decreasing order. Return true if it is sorted otherwise false.Examples:Input: arr[] = [10, 20, 30, 40, 50]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** The given array is not sorted.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-14 22:58:58
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def isSorted(self, arr):
        # code here
        n = len(arr)
        for i in range(0,n-1):
            if arr[i] > arr[i+1]:
                return False
               
        return True
```

*Generated on: 20/10/2026, 22:49:28*