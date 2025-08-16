```python
def countApplesAndOranges(s, t, a, b, apples, oranges):
    # Write your code here
    apple_cnt = 0
    orange_cnt = 0

    for d in apples:
        if s <= a + d <= t:
            apple_cnt += 1

    for d in oranges:
        if s <= b + d <= t:
            orange_cnt += 1

    print(apple_cnt)
    print(orange_cnt)
```

1. Initialize apple_count and orange_count to 0.
2. The house spans from position s to t (inclusive).
3. The apple tree is at position a; the orange tree is at b.
   Each apple falls distance d from a, and each orange falls distance d from b.
4. If s ≤ a + d ≤ t, increment apple_count by 1.
   If s ≤ b + d ≤ t, increment orange_count by 1.


**time complexity** :O(m + n),m = |apples|，n = |oranges|
**space complexity** :O(1)