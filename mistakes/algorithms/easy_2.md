```python
def compareTriplets(a, b):
    # Write your code here
    alice = bob = 0
    for ai, bi in zip(a, b):
        if ai > bi:
            alice += 1
        elif ai < bi:
            bob += 1
    return [alice, bob]
```
To compare two people's grades stored in separate lists, we can use  zip() , which pairs the corresponding elements into tuples so we can compare them one by one.

**Time complexity**: O(n)
**Space complexity**: O(1)