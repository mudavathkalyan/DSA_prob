mat[]={
1 2 4
6 7 8 
9 10 34
} 

target = 78,
return: false


We treat the entire 2D matrix as a flattened 1D array and perform binary search over indices from 0 to (N×M) - 1.

At each step, we convert the current mid index back to 2D coordinates using:

row = mid // M

col = mid % M

We compare the matrix[row][col] with the target:

If equal → return true

If less → search right half

If greater → search left half

If the loop ends without finding the target, return false
