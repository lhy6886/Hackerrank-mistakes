```python
def hurdleRace(k, height):
    # Write your code here
    magic = 0
    if k < max(height):
        magic += max(height) - k
    return magic
```

1. K is the initial jump height; magic is the number of magic potions needed.
2. If the initial jump height is less than the maximum hurdle height, the character must take (maximum height − initial height) potions.

**time complexity** :O(n)
**space complexity** :O(1)