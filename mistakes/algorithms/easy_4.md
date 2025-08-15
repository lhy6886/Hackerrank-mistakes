def diagonalDifference(arr):
    # Write your code here
    n = len(arr)
    return abs(sum(arr[i][i] - arr[i][n-1-i] for i in range(n)))
    
    n = len(arr)
    for i in range(n):
        res = abs(sum(arr[i][i] - arr[i][n-1-i]))
    return res

both are good for this question, the second one is more clear for freshmen
We need to compute the absolute difference between the sums of the two diagonals of a square matrix of unknown size.
eg.we got a 3*3 square matrix, 
1 2 3
4 5 6
7 8 9
need to know the sum of 159 and 357,then we need to know the differences btw two sums
the location of these numbers are: 1[0,0], 2[0,1], 3[0,2], 4[1,0], 7[2,0]

and everything is clear, we got the sum firstly and we got absolute difference secondly

Time complexity: O(n)
Space complexity: O(1)