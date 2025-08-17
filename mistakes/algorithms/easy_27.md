```python
def designerPdfViewer(h, word):
    # Write your code here
    max_h = 0              
    for ch in word:         
        idx = ord(ch) - ord('a')  
        max_h = max(max_h, h[idx]) 
    return max_h * len(word) 
```
1. h  is a 26-element list that gives the heights of the letters a–z in alphabetical order.
2. Iterate over each character  ch  in  word :
 •  ord(ch) - ord('a')  yields an index from 0 to 25;
 • track the maximum height encountered in  max_h .
3. The final area equals  max_h * len(word) , since each letter is treated as 1 mm wide.\\

**Time complexity**: O(|word|)
**Space complexity**: O(1)