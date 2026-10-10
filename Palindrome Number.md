## 01. Palindrome Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/palindrome0746/1)

### Problem Description

**Task:** You are given an integer n. Your task is to find if it is a palindrome. Examples:Input: n = 555

#### Examples

##### Example 1

- **Output:**
```text
trueExplanation: if number is palindrome, mainly ignore sign.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(d), d is number of digits in nAuxiliary Space: O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Python)

- **Submitted:** 2026-10-10 22:16:09
- **Status:** Correct
- **Marks:** 2

```python
class Solution:
    def isPalindrome(self, n):
        # code here
        n = abs (n)
        nums = n
        rev = 0 
        
        while nums > 0:
            digit = nums % 10 
            rev = rev * 10 + digit
            nums = nums // 10
            
        if rev == n:
            return True
        else :
            return False
```

*Generated on: 10/10/2026, 22:16:53*