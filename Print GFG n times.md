## 01. Print GFG n times

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-gfg-n-times/1)

### Problem Description

**Task:** Given a positive number n, print the string "GFG" exactly n times separated by a single space.

#### Examples

##### Example 1

- **Input:**
```text
n = 5 GFG GFG GFG GFG GFG
```

##### Example 2

- **Input:**
```text
3 GFG GFG GFG
```

#### Constraints

- **1.** `1 ≤ n ≤ 10³`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-24 00:01:28
- **Status:** Correct
- **Marks:** 1

```python
n = int(input())
def printGfg(n):
    if n == 0:
        return

    print("GFG", end=" ")
    printGfg(n - 1)

printGfg(n)
```

*Generated on: 01/10/2026, 22:38:02*