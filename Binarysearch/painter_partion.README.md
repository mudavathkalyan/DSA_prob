boards[] = {10, 20, 30, 40}, k = 2
return: 60

You're not searching through the array, but through the range of possible answers—from the longest board (max) to the total length of all boards (sum).

The function countPainters(mid) checks how many painters are needed if each can paint at most mid time.

If you need more painters than allowed, mid is too low → search higher.

If it's within k, try to minimize further → search lower.

So, just like in subarray partition or cow placement problems, you:

Binary search over the answer space.

Use a feasibility function (countPainters, canWePlace, etc.) to guide the search.

Return the best feasible minimum or maximum based on the problem.