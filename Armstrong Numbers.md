## 01. Armstrong Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/armstrong-numbers2727/1)

### Problem Description

**Task:** You are given a 3-digit number n, Find whether it is an Armstrong number or not.An Armstrong number of three digits is a number such that the sum of the cubes of its digits is equal to the number itself. 371 is an Armstrong number since 3³ + 7³ + 1³ = 371. Examples:Input: n = 153

#### Examples

##### Example 1

- **Output:**
```text
true
```
- **Explanation:** 153 is an Armstrong number since 1³ + 5³ + 3³ = 153.

##### Example 2

- **Input:**
```text
n = 372
```
- **Output:**
```text
false
```
- **Explanation:** 100 is not an Armstrong number since 1³ + 0³ + 0³ = 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-09-19 13:49:44
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def armstrongNumber(self, n):
        num = n
        total = 0
        nod = len(str(num))

        while num > 0:
            last_digit = num % 10
            total = total + (last_digit ** nod)
            num = num // 10

        return total == n
```

*Generated on: 06/10/2026, 20:17:57*