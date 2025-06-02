# Split Array - Largest Sum

a[] = {3,5,1}, k = 3
Result: 5



low = max(arr) (smallest possible max sum),

high = sum(arr) (largest possible max sum).

Loop while low <= high:

Compute mid = (low + high) // 2.

Use countPartitions(mid) to check how many subarrays we can form without exceeding mid as the max sum.

If partitions > k: too many splits → increase limit → low = mid + 1.

Else: valid or fewer splits → try smaller max → high = mid - 1.

Return low as the minimum possible max sum for k subarrays.
