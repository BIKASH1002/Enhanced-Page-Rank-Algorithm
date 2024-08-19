# Overview

This project introduces an enhanced PageRank algorithm designed to optimize search engine performance in large-scale and dynamic web environments. Traditional algorithms like Google’s PageRank have been foundational, but they face limitations in handling the ever-growing complexities of modern web structures. By incorporating the Stother-William’s matrix multiplication technique, the proposed algorithm significantly reduces computational time while improving accuracy in identifying key influential pages.

# Problem Statement

With the continuous expansion of web content, the need for efficient and accurate page ranking algorithms has become critical for effective information retrieval. The challenge lies in developing a scalable algorithm that can handle large datasets while maintaining high accuracy and convergence speed. This project addresses these challenges by enhancing the traditional PageRank algorithm, making it suitable for large-scale applications like web indexing and social network analysis.

# Methodology

The proposed algorithm enhances the traditional PageRank by integrating Stother-William’s matrix multiplication, which reduces the computational complexity from O(n³) to approximately O(n².373). This optimization significantly improves the speed of iterative computations necessary for PageRank, allowing it to handle larger datasets more efficiently.

# Datasets

The dataset used is a WebGraph from the Stanford Network Analysis Project (SNAP) collection. It consists of:

**Nodes:** 260,815 (representing web pages)

**Edges:** 1,103,613 (representing hyperlinks)

The dataset is used to simulate the link structure of the web and test the efficiency and accuracy of the proposed algorithm.

# Proposed Algorithm Workflow

1) **Input Adjacency Matrix:** Initialize the graph structure representing web pages and links.

2) **Transition Matrix Construction:** Normalize the adjacency matrix and handle dangling nodes.

3) **Initialization:** Set initial PageRank scores with equal values.

4) **Iterative Computation:** Update PageRank scores using the enhanced formula until convergence.

5) **Convergence Check:** Ensure the difference between iterations falls below a defined tolerance.

6) **Output Final Scores:** Once convergence is achieved, output the final PageRank scores.

The algorithm improves on traditional methods by converging faster and offering a more efficient computation process, making it particularly effective for large-scale networks.

# Results
Computation Time: The proposed algorithm significantly reduces computation time, showing a 41-45% improvement over Google’s traditional PageRank across various node counts.

| S.No. | Model      | Accuracy (in %) | F-1 score |
|-------|------------|-----------------|-----------|
| 1.    | Alexnet    | 94.1            | 0.94      |
| 2.    | Densenet   | 96.7            | 0.91      |
| 3.    | Googlenet  | 97.5            | 0.97      |
| 4.    | VGG        | 97.0            | 0.97      |
| 5.    | Resnet     | 97.5            | 0.97      |
| 6.    | RNN        | 87.8            | 0.70      |

Ranking Accuracy: The algorithm produces more accurate and stable PageRank scores after approximately 25 iterations.

## PageRank Score Comparison

| S. No | Node ID | Google PageRank | Proposed Algorithm PageRank |
|-------|---------|----------------|-----------------------------|
| 1     | 4985    | 0.00381        | 0.00684                     |
| 2     | 4897    | 0.00357        | 0.00639                     |
| 3     | 4996    | 0.00277        | 0.00502                     |
| 4     | 4998    | 0.00273        | 0.00497                     |
| 5     | 4982    | 0.00257        | 0.00493                     |

Correlation Analysis: A strong positive correlation between the proposed PageRank scores and in-degree centrality highlights the importance of incoming links in determining page relevance.

# Future Work

Further improvements could involve extending the algorithm for real-time web crawling and integrating additional centrality measures to refine ranking accuracy.
