arr[] ={3, 4, 4, 7, 8, 10}, x= 5
Result: 4 7
The floor of 5 in the array is 4, and the ceiling of 5 in the array is 7.


# Ceil (smallest element ≥ x):

Initialize low = 0, high = n - 1, ans = -1.

While low <= high:

Compute mid = (low + high) // 2.

If arr[mid] ≥ x: store arr[mid] as potential answer, search left half.

Else: search right half.

Return ans.

# Floor (largest element ≤ x):

Initialize low = 0, high = n - 1, ans = -1.

While low <= high:

Compute mid = (low + high) // 2.

If arr[mid] ≤ x: store arr[mid] as potential answer, search right half.

Else: search left half.

Return ans.

