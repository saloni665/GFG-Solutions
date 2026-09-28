## 01. For Pythonclass Solution: def countFactors (self, n): # code here num = n count = 0 for i in range(1, int(num**0.5)+1): if n%i==0: if i!=n//i: count +=2 else: count +=1 return count

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/number-of-factors1435/1)

### Problem Description

**Task:** Find the number of factors for a given integer n. Examples:

#### Examples

##### Example 1

- **Input:**
```text
n = 5
```
- **Output:**
```text
2
```
- **Explanation:** 5 has 2 factors 1 and 5

##### Example 2

- **Input:**
```text
n = 25
```
- **Output:**
```text
3
```
- **Explanation:** 25 has 3 factors 1, 5, 25

#### Constraints

- **1.** `1 ≤ n ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-21 23:15:49
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def countFactors (self, n):
        count = 0
        for i in range(1, n+1):
            if n % i == 0:
                count += 1
                
        return count
```

*Generated on: 28/09/2026, 21:59:31*