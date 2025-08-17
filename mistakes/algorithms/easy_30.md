```python
def beautifulDays(i, j, k):
    # Write your code here
    total = 0
    for nums in range(i,j+1):
        reversed_num = int(str(nums)[::-1])
        if abs(nums - reversed_num) % k == 0:
            total += 1
    return total
```

1. Iterate over the range from i to j (inclusive).
2. Reverse each number after converting it to a string.
3. The slice [::-1] works only on strings or sequences, so the integer must first be cast to str.

**Time complexity**: O(|a|)
**Space complexity**: O(1)