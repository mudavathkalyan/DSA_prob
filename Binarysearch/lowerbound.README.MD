# Implement Lower Bound
arr[] = {3,5,8,15,19}, x = 9
return: 3

Index 3 is the smallest index such that arr[3] >= x.

# Approach:binary search

Binary Search to Find the First Index ≥ x:

Set low to the first index and high to the last index.

While low <= high:

Compute mid = (low + high) // 2.

If arr[mid] >= x: store mid as a potential answer and search the left half.

If arr[mid] < x: search the right half.

Loop ends when low exceeds high.

