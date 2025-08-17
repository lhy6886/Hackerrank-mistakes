```python
def getMoneySpent(keyboards, drives, b):
    #
    # Write your code here.
    #
    max_cost = -1
    for k in keyboards:
        for d in drives:
            cost = k + d
            if cost <= b:
                max_cost = max(max_cost, cost)
    return max_cost
```

1. Set max_cost = -1 initially, in case it is not possible to buy both items.
2. Iterate over the prices of keyboards and drives; if the sum is within the budget, update max_cost to the maximum of cost and max_cost.

**time complexity** :O(|keyboards| × |drives|)
**space complexity** :O(1)