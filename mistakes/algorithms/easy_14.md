```python
def breakingRecords(scores):
    # Write your code here
    maxs = scores[0]
    mins = scores[0]
    maxscore = 0 
    minscore = 0
    for num in scores[1:]:
        if num > maxs:
            maxscore += 1
            maxs = num
        if num < mins:
            minscore += 1
            mins = num
    return [maxscore,minscore]
```

1. Set first score in the array as max score and min score at the same time
2. Iterate from the second score, if a score is bigger than max score,then set that score as max score and maxscore + 1
3. The way to find min score is same as max score

**time complexity** :O(n)
**space complexity** :O(1)