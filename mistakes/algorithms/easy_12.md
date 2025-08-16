```python
def kangaroo(x1, v1, x2, v2):
    # Write your code here
    return 'YES' if v1 > v2 and (x2 - x1) % (v1 - v2) == 0 else 'NO'
```

1. A simple chase-and-catch problem, use mathmatical formula

**time complexity** :O(1)
**space complexity** :O(1)