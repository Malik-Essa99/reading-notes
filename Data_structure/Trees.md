# Trees 
## Tree Traversal:

Tree traversal refers to the process of visiting and examining each node in a tree data structure. There are three commonly used methods for tree traversal: pre-order traversal, in-order traversal, and post-order traversal.

Example:

          A
         / \
        B   C
       / \   \
      D   E   F


+ Pre-order traversal: In pre-order traversal, we visit the root node first, then traverse the left subtree, and finally traverse the right subtree. The order of operations is root-left-right.


        Pre-order traversal: A - B - D - E - C - F



+ In-order traversal: In in-order traversal, we traverse the left subtree first, then visit the root node, and finally traverse the right subtree. The order of operations is left-root-right. In binary search trees, the in-order traversal visits the nodes in ascending order.

        In-order traversal: D - B - E - A - C - F


+ Post-order traversal: In post-order traversal, we traverse the left subtree first, then traverse the right subtree, and finally visit the root node. The order of operations is left-right-root. Post-order traversal is commonly used to delete nodes from a tree.


        Post-order traversal: D - E - B - F - C - A


Each traversal method has its own specific use case and can provide different perspectives on the tree structure. Traversals are often implemented recursively, where each recursive call handles a subtree, or iteratively using a stack or queue data structure to keep track of the nodes to be visited.

By applying these traversal methods, you can explore and process the nodes of a tree in different orders, depending on your specific needs and the problem you are trying to solve.