```python
def catAndMouse(x, y, z):
    #
    # Write your code here.
    #
    if abs(x - z) < abs(y - z):
        return 'Cat A'
    elif abs(x - z) > abs(y - z):
        return 'Cat B'
    else :
        return 'Mouse C'
```

1. Simple calculate distance and compare

**time complexity** :O(1)
**space complexity** :O(1)