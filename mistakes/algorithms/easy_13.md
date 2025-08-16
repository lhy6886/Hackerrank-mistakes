```python
def getTotalX(a, b):
    # Write your code here
    def _gcd(x, y):
        while y:
            x, y = y, x % y
        return x

    def _lcm(x, y):
        return (x * y) // _gcd(x, y)

    
    lcm_a = a[0] 
    for num in a[1:]:
        lcm_a = _lcm(lcm_a, num) 

   
    gcd_b = b[0]
    for num in b[1:]:
        gcd_b = _gcd(gcd_b, num)

    
    count = 0
    

    for x in range(lcm_a, gcd_b + 1, lcm_a):
        if gcd_b % x == 0:
            count += 1

    return count
```

1. Define two helper functions to compute gcd and lcm.
2. Initialize the running lcm with the first element of array a, then iterate from the second element to obtain the overall lcm of array a.
3. Similarly, initialize the running gcd with the first element of array b, then iterate to obtain the overall gcd of array b.
4. Count all integers x between the final lcm and the final gcd (inclusive) that are multiples of the lcm and divisors of the gcd, stepping by the lcm.

**time complexity** :O(1)
**space complexity** :O(1)