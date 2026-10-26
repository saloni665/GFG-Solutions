## 01. Prime Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/prime-number2314/1)

### Problem Description

**Task:** Given a number n, determine whether it is a prime number or not.Note: A prime number is a number greater than 1 that has no positive divisors other than 1 and itself.Examples :Input: n = 7

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** 1 has only one divisor (1 itself), which is not sufficient for it to be considered prime.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-10 22:31:50
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def isPrime(self, n):
        # code here
        if n <= 1 :
            return False
        else :
           
            for i in range (2 ,n):
                if n % i == 0 :
                    return False
            
            return True
```

*Generated on: 26/10/2026, 21:50:01*