```python
def plusMinus(arr):
    # Write your code here
    pos = neg = zer = 0
    for i in arr:
        if i < 0:
            neg += 1
        elif i == 0:
            zer += 1
        else:
            pos += 1
    n = len(arr)
    print(f'{pos/n:.6f}\n{neg/n:.6f}\n{zer/n:.6f}')
```

first of all we need initialize 3 varaiables to 0, and then iterate over the array, if the number is bigger
than 0, pos+1, now we need to calculate the ratio, and round to 6 decimal places, this step can be done
in one sentence, and that's it.

**Time complexity**: O(n)
**Space complexity**: O(1)