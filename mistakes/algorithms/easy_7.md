```python
def miniMaxSum(arr):
    # Write your code here
    a = sorted(arr)
    sum1 = sum(a[0:4])
    sum2 = sum(a[1:5])
    print(sum1, sum2)
```
1. For this question, we need to find out minimum sum and maximum sum of array
2. So the solution is sort the array, and add first 4 numbers, this will be the minimum sum
and add last 4 numbers, this will be the maximum sum, and print them out

**time complexity** :O(n log n)
**space complexity** : O(n)