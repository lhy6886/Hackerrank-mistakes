```python
def sockMerchant(n, ar):
    # Write your code here
    count = {}
    for color in ar:
        count[color] = count.get(color,0)+1
    pairs = 0
    for i in count.values():
        pairs += i //2
    return pairs
```

1. Create a dictionary to tally how many socks there are of each color.
2. Color is key and number of sock is value
2. Iterate over these tallies and add half of each count (using integer division) to the running total of pairs.

**time complexity** :O(n)
**space complexity** :O(n)