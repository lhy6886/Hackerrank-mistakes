```python
def timeConversion(s):
    # 07:05:45PM  ->  19:05:45
    t  = s[:-2]   
    ap = s[-2:]   

    h, m, sec = t.split(':')
    h = int(h)
    
    if ap == 'AM':
        if h == 12:
            h = 0
    else:               # PM
        if h != 12:
            h += 12
    
    return f'{h:02d}:{m}:{sec}'
```

1. We need to convert a time from 12-hour format (with AM/PM) into 24-hour format (without AM/PM).
2. First, split the string into two parts: the suffix (AM or PM) and the time portion.
3. Then split the time portion into three parts—hours, minutes, and seconds—because only the hours and the suffix determine the conversion.
4. Returning the new time string without the suffix is sufficient.

**time complexity** :O(1)
**space complexity** :O(1)