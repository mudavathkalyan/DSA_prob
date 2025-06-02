arr = [4,5,6,7,0,1,2,3], k = 0
Result: 4
at 4th index k is present


Initialize: Set low = 0, high = n - 1.

Loop while low <= high:

Calculate mid = (low + high) // 2.

If arr[mid] == target: return mid.

Check which half is sorted:

If arr[low] <= arr[mid] (left half is sorted):

If arr[low] <= target <= arr[mid]: search left half (high = mid - 1).

Else: search right half (low = mid + 1).

Else (right half is sorted):

If arr[mid] <= target <= arr[high]: search right half (low = mid + 1).

Else: search left half (high = mid - 1).

If not found, return -1.