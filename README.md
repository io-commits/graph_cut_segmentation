# Graph Cuts Based Segmentation

This repository explores Graph-Based Semantic Segmentation methods, inspired by Jianbo Shi's work. 
It includes experiments with Normalized Cuts, focusing on graph structures to model spatial relationships for accurate image segmentation.

<img src="assets/original_image.png" height="400"> <img src="assets/segmented.png" height="400">

# Normalized Cuts Formula

The Normalized Cuts criterion is defined as:

$$Ncut(A, B) = \frac{\text{cut}(A, B)}{\text{assoc}(A, V)} + \frac{\text{cut}(A, B)}{\text{assoc}(B, V)}$$

Where:
- $\text{cut}(A, B) = \sum_{u \in A, v \in B} w(u, v)$
- $\text{assoc}(A, V) = \sum_{u \in A, t \in V} w(u, t)$

$w(u, v)$ represents the weight of the edge between nodes $u$ and $v$, $A$ and $B$ are two disjoint subsets of the graph, and $V$ is the set of all nodes.


