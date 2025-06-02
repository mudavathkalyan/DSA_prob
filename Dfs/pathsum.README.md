Tree:
      5
     / \
    4   8
   /   / \
  11  13  4
 /  \
7    2

target = 22  

Output: true

Explanation:
We use DFS to explore each path from root to leaf, keeping a running sum.
Path 5 → 4 → 11 → 2 has sum 22, so we return true.

Traversing every root-to-leaf path, accumulating the sum along the way. If we reach a leaf and the accumulated sum equals the target, we return true.
