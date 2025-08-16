```python
return candles.count(max(candles))
```

1. Return numbers of longest candles on the birthday cake
2. First we need to find out the longest candles by using max()
and then need to know the numbers, how many longest candles, using .count
3. You can also write as:

```python
a = max(candles)
b = candles.count(a)
return b
```

**time complexity** :O(k)k = len(candles)
**space complexity** :O(1)