## Binary Trees, Binary Search Treess and K-ary Trees

Common Terms:
- node: contains own value and reference to other nodes
- root: node at the beginning of the tree
- k: a number that specifies number of childen any node may have in a k-ary tree. In a binary tree, k=2
- left: a reference to one child node, in a binary tree 
- right: a reference to the other child node in a binary tree
- edge: the edge in a tree is the link between a parent and child node
- leaf: a node that does not have any children
- height: the number of edges from the root to the furthest leaf

### Depth-First Traversal
- Prioritize going thru the height of the tree first (depth). You can do this multiple ways each of which change the order we search/print the root: 
  1. pre-order: root > left > right (top  to bottom)
      - using call stack via recursion
      - looks at root first
      - stores original root's left as root in order to add to call stack
      - continue until reach leaf node
  2. in-order: left > root > right (bottom to root, switch, bottom to root)
  3. post-order: left > right > root (bottom left, all items on that level, then up until right below root then move to right bottom move up and end on root)

### Breadth-First Traversal
- Uses a queue instead of call stack via recursion ^^
- Enqueing, and then dequeuing the root, gives us access to left and right children

### K-ary Trees
- if nodes are able to have more than 2 child nodes this is called a k-ary tree
- similar to breadth traversal in that use queue and dequeue but with k-ary we move down list of children of length k, rather than  checking for the presence of a left child. 

### Adding Nodes
- One strategy: fill all child spots from the top down from left to right
- To put in specific location you need to reference both the new node to create and the parent node which the child is attached to.

### Big O
- Time: For inserting & searching for specific node: O(n)
- Space:for breadth traversal O(w) where w is the largest width of the tree
- "Perfect" binary tree: 2^(h-1) where h=height of tree. Height can be calculated as log n where n is the number of nodes 

### Binary Search Tree
- Nodes are organized in a manner where all values that are smaller than the root are placed to the left and all values that are larger than the root are placed to the right
- To search: compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side if the value is larger you only traverse the right side.
- Best approach: while loop

### BST Big O
- Time: O(h) where h = height
- Space: O(1)



