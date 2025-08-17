```python
def countingValleys(steps, path):
    # Write your code here
    level = 0
    valleys = 0
    for i in path:
        pre_level = level
        if i == 'U':
            level += 1
        elif i == 'D':
            level -= 1
        if pre_level == -1 and level == 0:
            valleys += 1
    return valleys
```

1. A valley is only counted if the next step is up and the current level is –1 right before that step.
2. pre_level  records the level from the previous loop iteration.

**time complexity** :O(steps)
**space complexity** :O(1)