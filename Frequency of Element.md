## 01. Frequency of Element

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/find-the-frequency/1)

### Problem Description

**Task:** Given an array arr of positive integers and an integer x. Return the frequency of x in the array.Examples : Input: arr = [1, 1, 1, 1, 1], x = 1

#### Examples

##### Example 1

- **Output:**
```text
2
```
- **Explanation:** Frequency of 2 is 2.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-29 19:54:04
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def findFrequency(self, arr, x):
        # code here
        hash_map = {}
        n = len(arr)
        for num in arr:
            
            if num in hash_map:
                hash_map[num] += 1

            else:    
                hash_map[num] = 1 
        
        return hash_map.get(x,0)
```

*Generated on: 29/09/2026, 20:11:31*