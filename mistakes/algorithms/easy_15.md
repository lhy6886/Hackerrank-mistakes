```python
def birthday(s, d, m):
    # Write your code here
    total = 0
    for i in range(n-m+1):
        part = sum(s[i:i+m])
        if part == d:
            total += 1
    return total
```

1. The problem asks for the number of contiguous sub-arrays of length m whose sum equals d.
2. Initialize  total = 0 .
3. Loop over every valid starting index  i  from  0  to  n - m  inclusive.
4. For each  i , compute the sum of the slice  s[i : i + m]  (i.e., elements at indices  i … i + m - 1 ).
5. If the sum equals  d , increment  total .

**time complexity** :O(n)
**space complexity** :O(1)