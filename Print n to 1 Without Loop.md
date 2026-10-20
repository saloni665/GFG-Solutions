## 01. Print n to 1 Without Loop

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-n-to-1-without-loop/1)

### Problem Description

**Task:** Given an integer n, print all numbers from n to 1 in decreasing order, separated by spaces, without using any loops.Examples :Input: n = 5

#### Examples

##### Example 1

- **Output:**
```text
3 2 1
```
- **Explanation:** The numbers from 3 to 1 are printed in decreasing order

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (2)

#### Solution 1 (Python)

- **Submitted:** 2026-10-20 22:53:03
- **Status:** Correct
- **Marks:** 0

```python
class Solution:
    def printNos(self, n: int) -> None:
        if n == 0:
            return
        
        print(n ,end = " ")
        self.printNos(n-1)
```

#### Solution 2 (Python)

- **Submitted:** 2026-09-24 17:59:51
- **Status:** Correct
- **Marks:** 1

```python
class Solution:
    def printNos(self, n):
        if n == 0:
            return

        print(n, end=" ")
        self.printNos(n - 1)
```

*Generated on: 20/10/2026, 22:53:36*