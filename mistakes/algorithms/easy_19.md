```python
def bonAppetit(bill, k, b):
    # Write your code here
    total = sum(bill)
    total_actual = sum(bill) - bill[k]
    anna_actual = total_actual//2
    if b - anna_actual != 0:
        print(b - anna_actual)
    else:
        print('Bon Appetit')
```

1. Compute the total cost of all dishes.
2. Subtract the price of the dish Alice did not eat to get the actual shared total.
3. Calculate how much Bob owes Alice; if the difference is zero, print “Bon Appetit.”

**time complexity** :O(n)
**space complexity** :O(1)