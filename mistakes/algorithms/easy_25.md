```python
def pickingNumbers(a):
    # Write your code here
    c = [0]*(max(a)+1)
    for i in a :
        c[i] += 1
    m = 0
    for i in range(len(c)-1):
        if c[i] + c[i+1] > m:
            m = c[i] + c[i+1]
    return m
```

1. Count occurrences of each number into an array c
2. Iteratee over c up to len(c)-1 to avoid out-of-range access
3. Summing each adjacent pair (i, i+1)

**time complexity** :O(n + m)
**space complexity** :O(m)