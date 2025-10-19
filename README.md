# Kd-Tree (2D Range Search & Nearest Neighbor)
A space-efficient implementation of a 2D tree data structure for geometric search operations on sets of points in a plane.

## Problem Statement

Given a set of points in a 2D plane, efficiently support:
- **Range search**: Find all points contained within a query rectangle
- **Nearest neighbor search**: Find the closest point to a query point

Brute force approaches require examining every point (O(n) per query). The kd-tree enables efficient pruning of the search space using geometric properties.

## Implementation

- **2D Binary Search Tree** with alternating split dimensions (vertical/horizontal)
- **Recursive range search** with rectangle intersection pruning
- **Optimized nearest neighbor** using distance-based subtree elimination
- **Custom Node structure** tracking partition boundaries for efficient pruning
- Handles duplicate point detection and null input validation

## Tech Stack

- Java 11
- Princeton algs4 library (Point2D, RectHV)
- Recursive tree traversal algorithms

## Key Concepts Demonstrated

- k-dimensional trees (k=2)
- Space partitioning data structures
- Geometric algorithms and computational geometry
- Pruning techniques for search optimization
- Recursive tree operations
- Balanced vs unbalanced tree performance trade-offs

## Performance

- **Insert**: O(log n) average case (balanced tree)
- **Range search**: O(R + log n) where R is number of points in range
- **Nearest neighbor**: O(log n) average case with effective pruning
- Space complexity: O(n)
- Significantly faster than brute force for large point sets

---

*Project from Princeton University Algorithms Part I course*  
*Instructor: Robert Sedgewick & Kevin Wayne*