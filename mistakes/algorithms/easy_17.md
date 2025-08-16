```python
def migratoryBirds(arr):
    # Write your code here
    cnt = [0] * 6        
    for t in arr:
        cnt[t] += 1 
  
    max_cnt = max(cnt)
  
    for bird_id in range(1, 6):
        if cnt[bird_id] == max_cnt:
            return bird_id
```

1. Create a list  cnt  of length 6 to count occurrences of bird types 1–5.
2. Iterate over the array and increment the corresponding counter for each bird type.
3. Find the maximum count value.
4. Iterate bird IDs 1 to 5 in ascending order; if multiple IDs share the maximum count, return the smallest ID.

**time complexity** :O(n)
**space complexity** :O(1)