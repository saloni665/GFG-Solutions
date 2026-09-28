## 01. 1 to n Without Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-1-to-n-without-using-loops3621/1)

### Problem Description

**Task:** Given an positive integer n, print numbers from 1 to n without using loops. Implement the function printTillN() to print the numbers from 1 to n as space-separated integers.Examples Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
1 2 3 4 5 6 7 8 9 10
```
- **Explanation:** We have to print numbers from 1 to 10.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-23 23:48:29
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def printTillN(self, n):
        def solve(i):
            if i > n:
                return

            print(i, end=" ")
            solve(i + 1)

        solve(1)
```

*Generated on: 28/09/2026, 22:04:07*