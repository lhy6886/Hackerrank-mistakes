```python
def divisibleSumPairs(n, k, ar):
    # Write your code here
    total = 0
    for i in range(n):
        for j in range(i+1,n):
            if (ar[i]+ar[j]) %k == 0:
                total += 1
    return total
```

1. Count how many pairs of elements have a sum divisible by k.
2. Iterate over the array once, and for each index i, check every index j > i

**time complexity** :O(n²)
**space complexity** :O(1)

OR we can use another code

```python
def divisibleSumPairs(n, k, ar):
    cnt = [0] * k
    total = 0
    for x in ar:
        r = x % k
        complement = (k - r) % k 
        total += cnt[complement]
        cnt[r] += 1
    return total
```

1. Create an array  cnt  of length  k , initialized with zeros;
  cnt[r]  will store how many numbers seen so far have remainder  r  when divided by  k .
2. Initialize  total  to 0; this will accumulate the count of valid pairs.
3. Traverse each element  x  in the array  ar :
4. Compute its remainder  r = x % k .
5. Compute the complementary remainder  complement = (k - r) % k ; this is the remainder that, when added to  r , yields a multiple of  k .
6. Add the number of elements previously seen with remainder  complement  to  total ,because each of those elements can pair with the current element to form a sum divisible by  k .
7. Increment  cnt[r]  by 1, recording the current remainder for future pairs.
8. After processing all elements, return  total , which now holds the number of unordered pairs whose sum is divisible by  k .

**time complexity** :O(n)
**space complexity** :O(k)