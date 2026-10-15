## 01. Sum of Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-all-array-elements/1)

### Problem Description

**Task:** Given an integer array arr[], return the sum of all elements of arr.Examples:Input: arr[] = [1, 2, 3, 4]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** 1 + 2 + 3 + 4 = 10.

##### Example 2

- **Input:**
```text
arr[] = [1, 3, 3]
```
- **Output:**
```text
7
```
- **Explanation:** 1 + 3 + 3 = 7.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-15 21:09:24
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def arraySum(self, arr):
           # code here
        n = len(arr)
        total = 0
        for i in range(0,n):
            
            total = total + arr[i] 
            
        return total
```

*Generated on: 15/10/2026, 21:10:13*