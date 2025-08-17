```python
def utopianTree(n):
    # Write your code here
    height = 1
    for i in range(n):
        if i % 2 == 0:
            height *= 2
        else:
            height += 1
    return height
```

1. Set initial height is 1 and iterate over array,the tree has original height

**Time complexity**: O(n)
**Space complexity**: O(1)