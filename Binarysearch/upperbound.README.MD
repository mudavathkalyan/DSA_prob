arr[] = {3,5,8,9,15,19}, x = 9
return: 4
Index 4 is the smallest index such that arr[4] > x.

Initialize: Set low = 0, high = n - 1.

Loop while low <= high:

Compute mid = (low + high) // 2.

If arr[mid] > x: store mid as a potential answer and search left half.

If arr[mid] <= x: search right half.

Loop ends when low > high.

This finds the smallest index with value > x.


