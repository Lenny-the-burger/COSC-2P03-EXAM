# Trees

-   Chapter 4 covers the topic of trees.
-   Understand the definitions and properties of different types of trees, including general trees, binary trees, and threaded trees.
-   Know how to represent, manipulate, and traverse trees, including recursive, iterative, and threaded traversals.
-   Be familiar with the concept of a binary search tree and know how to implement it.
-   Understand the concept of height-balanced trees, including AVL trees.
-   Know about B-trees, including setup and complexity considerations.
-   Be familiar with the concept of a heap and know how to represent it.

Trees are data structures that consist of nodes connected by edges. They have a hierarchical structure, with a root node at the top and child nodes below. Trees can be used to store and organize data in many different ways, such as storing the structure of a file system or simulating the behavior of a decision-making process.

```
    o
   / \
  o   o
 / \   \
o   o   o
```

## Definitions

There are several key terms that are used when discussing trees:

-   Node: a node is a point in the tree that stores a piece of data. A node may have zero or more child nodes, depending on the type of tree.
-   Edge: an edge is a connection between two nodes in the tree. In a tree, each node except the root has exactly one parent node, and each node except the leaves has one or more child nodes.
-   Root: the root is the topmost node in the tree. It has no parent node and is the ancestor of all other nodes in the tree.
-   Leaf: a leaf is a node that has no child nodes.
-   Subtree: a subtree is a portion of the tree that consists of a node and all of its descendants.
-   Ancestor: an ancestor of a node is any node on the path from the root to the node.
-   Descendant: a descendant of a node is any node that is a child, grandchild, great-grandchild, etc. of the node.

## Representation and manipulation of different types of trees

There are several different types of trees, each with its own characteristics and uses. Some common types of trees include:

-   General trees: a general tree is a tree in which each node can have any number of child nodes. This makes general trees the most flexible type of tree, but also the most difficult to work with because there is no standard way to represent or manipulate them.
-   Binary trees: a binary tree is a tree in which each node has at most two child nodes. This makes binary trees more structured and easier to work with than general trees, but also less flexible.
-   Binary search trees: a binary search tree is a binary tree in which the left child of a node is less than the parent node, and the right child is greater than the parent node. This property allows for fast insertion, deletion, and retrieval of items in the tree, making binary search trees a useful data structure for storing and organizing data that needs to be accessed quickly.

## Traversals

A traversal is the process of visiting all the nodes in a tree in a particular order. There are several different ways to traverse a tree, including:

-   Recursive traversal: a recursive traversal uses recursive function calls to visit each node in the tree. This approach is simple to implement but can be inefficient because it uses a lot of memory to store the function calls on the call stack.

-   Iterative traversal: an iterative traversal uses a loop to visit each node in the tree without the use of recursive function calls. This approach is more efficient than recursive traversal because it uses less memory, but it can be more difficult to implement.

-   Threaded traversal: a threaded traversal uses "threads" to link the nodes in the tree and allow for efficient traversal without the use of recursive function calls or explicit loops. This approach is the most efficient of the three because it uses the least amount of memory, but it requires the tree to be modified by adding the threads, which can be difficult to implement.

Tree traversal is the process of visiting (or "traversing") all the nodes in a tree data structure in a specific order. There are three main types of tree traversal:

-   Inorder traversal: in an inorder traversal, the nodes of the tree are visited in the order: left subtree, root, right subtree. This traversal visits the nodes of the tree in a sorted order, if the tree is a binary search tree (BST).
-   Preorder traversal: in a preorder traversal, the nodes of the tree are visited in the order: root, left subtree, right subtree. This traversal is often used to create a copy of the tree, or to get the postfix representation of an expression tree.
-   Postorder traversal: in a postorder traversal, the nodes of the tree are visited in the order: left subtree, right subtree, root. This traversal is often used to delete the nodes of a tree, or to evaluate an expression tree.

These traversal orders can be implemented using a recursive function or using an explicit stack to keep track of the nodes that have been visited. In addition, there are several other variations of tree traversal, such as level order traversal (which visits the nodes of the tree by level) and reverse order traversal (which visits the nodes in the opposite order as the standard traversal).

It's also possible to implement tree traversal using threads, which are auxiliary pointers that link a node to its inorder successor or predecessor. Inorder traversal using threads is often used to implement efficient iteration over the nodes of a tree.

## Binary search trees

A binary search tree (BST) is a binary tree that satisfies the following properties:

-   The left child of a node is less than the parent node.
-   The right child of a node is greater than the parent node.

These properties allow for fast insertion, deletion, and retrieval of items in the tree, making BSTs a useful data structure for storing and organizing data that needs to be accessed quickly.

### Bonus: BSP

Binary space partitioning (BSP) is a technique for recursively dividing a space into two convex subspaces by using a plane (or hyperplane) as a divider. This technique is commonly used in computer graphics to efficiently render and organize three-dimensional scenes.

Binary trees and quadtrees are two common data structures that use BSP for organizing and storing data.

A binary tree is a tree data structure in which each node has at most two children, called the left child and the right child. A binary tree can be used to represent a hierarchical structure, such as a file system, or to store data in a sorted order, such as in a binary search tree (BST). In a binary tree, BSP can be used to recursively divide the nodes of the tree into two convex regions, depending on the value of a specific attribute (such as the x-coordinate in a two-dimensional space).

A quadtree is a tree data structure in which each node has at most four children, called the north-west, north-east, south-west, and south-east children. A quadtree can be used to represent a two-dimensional space, such as an image or a map, by dividing the space into quadrants and storing the data in the appropriate quadrants. In a quadtree, BSP can be used to recursively divide the nodes of the tree into four convex regions, depending on the location of the data in the two-dimensional space.

In both binary trees and quadtrees, BSP can provide an efficient way to organize and store data, by dividing the space into smaller and smaller regions and storing the data in the appropriate regions. This can allow for faster search and retrieval of data, as well as more efficient rendering and visualization of the data.

## Threaded trees

A threaded tree is a tree in which each node has an additional "thread" pointer that links it to another node in the tree. These threads allow for efficient traversal of the tree without the use of recursive function calls or explicit loops. However, they require the tree to be modified by adding the threads, which can be difficult to implement.

## Height-balanced trees and AVL trees

A height-balanced tree is a tree in which the difference in height between the left and right subtrees of each node is at most one. This property allows for efficient insertion and deletion of items in the tree, as well as fast retrieval of items based on their position in the tree.

An AVL tree is a height-balanced binary search tree. It is named after its inventors, G.M. Adelson-Velsky and E.M. Landis, who described the tree in their 1962 paper. AVL trees are useful for storing and organizing data that needs to be accessed quickly and that may be subject to frequent insertions and deletions.

There are several methods for maintaining the balance of an AVL tree, including:

-   Rotations: an AVL tree can be balanced by performing rotations on the nodes of the tree. A rotation is a local operation that changes the structure of the tree by moving one or more nodes and their subtrees. There are four types of rotations: left rotation, right rotation, left-right rotation, and right-left rotation. Each type of rotation can be used to balance a different type of unbalanced tree, such as a tree with a left-heavy subtree or a tree with a right-left imbalance.
-   Double rotations: a double rotation is a combination of two rotations that can be used to balance a tree with a more complex imbalance, such as a tree with a right-right-left imbalance. A double rotation can be performed by first performing one type of rotation (such as a left rotation) on a subtree of the tree, and then performing another type of rotation (such as a right rotation) on the root of the tree.
-   Insertion and deletion: when a new node is inserted into an AVL tree, or an existing node is deleted from the tree, the balance of the tree may be affected. To maintain the balance of the tree, the tree must be re-balanced using one or more rotations after each insertion or deletion. This can be done by starting at the node where the insertion or deletion occurred and traversing up the tree to the root, checking the balance of each node and performing rotations as necessary.

These methods can be used to maintain the balance of an AVL tree, ensuring that the tree remains balanced and that the operations on the tree can be performed efficiently.

## B-trees

A B-tree is a tree data structure that allows for efficient insertion, deletion, and retrieval of items in a large, sorted dataset. B-trees are commonly used in file systems and databases because they allow for fast access to data while also minimizing the number of disk reads and writes required.

When working with B-trees, it's important to consider the following complexity considerations:

-   What to count: when calculating the time complexity of an operation on a B-tree, it's important to consider the number of items in the tree, as well as the size of the tree (i.e. the number of nodes and edges). This is because the time complexity of an operation on a B-tree is often a function of these factors.
-   How to count: when calculating the time complexity of an operation on a B-tree, it's important to consider the specific algorithm used to implement the operation. For example, an operation that uses a sequential search to find an item in the tree will have a different time complexity than an operation that uses a binary search to find the item.

## Heaps

A heap is a tree-based data structure that satisfies the following properties:

-   The tree is a complete binary tree (i.e. all levels are fully filled except the last level, which is filled from left to right).
-   The value of each node is greater than or equal to the value of its parent (for a max-heap) or less than or equal to the value of its parent (for a min-heap).

Heaps are useful for storing and organizing data in a way that allows for fast retrieval of the highest or lowest value item. They can be implemented using an array or a tree, and are commonly used in priority queue and sorting algorithms.

When working with heaps, it's important to consider the representation of the heap. For example, a heap implemented using an array will have a different time complexity for insertion and deletion operations than a heap implemented using a tree. It's also important to consider the type of heap (i.e. max-heap or min-heap) and the specific algorithm used to implement the operations on the heap.
