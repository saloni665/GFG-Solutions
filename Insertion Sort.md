## 01. Insertion Sort

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/insertion-sort/1)

### Problem Description

**Task:** Given an array arr[] of positive integers.The task is to complete the insertsort() function which is used to implement Insertion Sort. Examples:Input: arr[] = [4, 1, 3, 9, 7]

#### Examples

##### Example 1

- **Output:**
```text
[1, 4, 9]Explanation: The sorted array will be [1, 4, 9].
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n^2)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-06 20:13:35
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def insertionSort(self, arr):
        n = len(arr)
        for i in range (1,n):
            key = arr[i]
            j = i-1
            
            while j >=0 and arr[j] > key:
                arr[j+1] = arr[j]
                j -= 1
        
            arr[j+1] = key
```

*Generated on: 06/10/2026, 20:14:16*