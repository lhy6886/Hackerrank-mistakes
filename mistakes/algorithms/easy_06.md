```python
def staircase(n):
    # Write your code here
    i = range(1, n+1)
    for stair in i:
        print(('#'*stair).rjust(n))
```
1. We need to print a staircase, just simply litera over i
2. i is the range about the number of stairs from the first step to the last step
and print #*stair means print stairs with #
3. .rjust right-justifies the string in a field of width  n , padding with spaces on the left so the whole string is aligned to the right.

**time complexity** :O(n)
**space complexity** : O(1)