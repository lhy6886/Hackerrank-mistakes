```python
def angryProfessor(k, a):
    # Write your code here
    ontime = 0
    not_ontime = 0
    for i in a:
        if i <= 0:
            ontime += 1
        elif i > 0:
            not_ontime += 1
    if ontime >= k:
        return 'NO'
    else:
        return 'YES'
```

**Time complexity**: O(|a|)
**Space complexity**: O(1)