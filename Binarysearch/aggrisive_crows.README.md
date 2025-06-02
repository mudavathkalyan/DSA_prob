arr[] = {4,2,1,3,6},k = 2
return: 5


We are trying to maximize the minimum distance between cows placed in stalls. To do this, we use a binary search approach on possible distances.

We start by sorting the stalls, then search between the smallest possible distance (1) and the largest (stalls[n-1] - stalls[0]). At each step, we check if it's feasible to place all cows with at least the current distance using a helper function.

If placing is possible, we try larger distances to maximize it. If not, we try smaller distances. The process continues until we find the largest minimum distance that works.

