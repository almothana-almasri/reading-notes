[Back to Home](../README.md)

Trees are hierarchical structures composed of nodes connected by edges. They come in different types, such as Binary Trees, Binary Search Trees, and K-ary Trees.

Important tree terms include nodes (holding values and references), root (the starting node), edges (connections between nodes), leaves (nodes without children), and height (the length from the root to the furthest leaf).

Traversing a tree allows for searching and other operations. There are two main methods: depth-first and breadth-first. Depth-first explores the tree's depth first, while breadth-first goes through each level.

Depth-first traversals include pre-order (root, left, right), in-order (left, root, right), and post-order (left, right, root). Breadth-first goes level by level, using a queue.

Binary Trees have at most two children per node, while K-ary Trees have any number. Traversing a K-ary tree with breadth-first involves enqueueing and dequeuing nodes based on children.

Binary Search Trees (BST) organize values, with smaller ones to the left and larger ones to the right of each node. Searching in a BST follows a comparison and traversal process.

Time complexity depends on tree height: logarithmic (log(n)) for balanced trees and linear (n) for unbalanced ones. Space complexity is generally minimal.