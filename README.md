# Search Engine Performance Optimization Using Enhanced Page Ranking Algorithm

<div align = "justify">
    
# Overview

This project introduces an enhanced PageRank algorithm designed to optimize search engine performance in large-scale and dynamic web environments. Traditional algorithms like Google’s PageRank have been foundational, but they face limitations in handling the ever-growing complexities of modern web structures. By incorporating the Stother-William’s matrix multiplication technique, the proposed algorithm significantly reduces computational time while improving accuracy in identifying key influential pages.

# Problem Statement

With the continuous expansion of web content, the need for efficient and accurate page ranking algorithms has become critical for effective information retrieval. The challenge lies in developing a scalable algorithm that can handle large datasets while maintaining high accuracy and convergence speed. This project addresses these challenges by enhancing the traditional PageRank algorithm, making it suitable for large-scale applications like web indexing and social network analysis.

# Data Understanding

The dataset used in this project is the web-Google graph from the Stanford Network Analysis Project (SNAP), containing 260,815 nodes and 1,103,613 edges. This dataset represents the link structure of the web, where each node corresponds to a webpage and edges represent hyperlinks between pages.

The dataset’s size and structure make it ideal for testing the efficiency and scalability of the enhanced PageRank algorithm. It provides a real-world scenario for web graph analysis, where understanding node importance is critical for search engine optimization and ranking accuracy.

# Methodology

The proposed algorithm enhances the traditional PageRank by integrating Stother-William’s matrix multiplication, which reduces the computational complexity from O(n³) to approximately O(n^2.373). This optimization significantly improves the speed of iterative computations necessary for PageRank, allowing it to handle larger datasets more efficiently.

# Setup

Jupyter Notebook (for interactive development)

**Libraries:** pandas, matplotlib

# Workflow

<p align="center">
    <img src="https://github.com/user-attachments/assets/177a25af-74ec-4de7-8195-10446e2ac145" alt="Workflow"/>
</p>

# Implementation

1) **Input Adjacency Matrix:** Initialize the graph structure representing web pages and links.

2) **Transition Matrix Construction:** Normalize the adjacency matrix and handle dangling nodes.

3) **Initialization:** Set initial PageRank scores with equal values.

4) **Iterative Computation:** Update PageRank scores using the enhanced formula until convergence.

5) **Convergence Check:** Ensure the difference between iterations falls below a defined tolerance.

6) **Output Final Scores:** Once convergence is achieved, output the final PageRank scores.

The algorithm improves on traditional methods by converging faster and offering a more efficient computation process, making it particularly effective for large-scale networks.

# Results
Computation Time: The proposed algorithm significantly reduces computation time, showing a 41-45% improvement over Google’s traditional PageRank across various node counts.

<div align = "center">
  
| S.No. | Model      | Accuracy (in %) | F-1 score |
|-------|------------|-----------------|-----------|
| 1.    | Alexnet    | 94.1            | 0.94      |
| 2.    | Densenet   | 96.7            | 0.91      |
| 3.    | Googlenet  | 97.5            | 0.97      |
| 4.    | VGG        | 97.0            | 0.97      |
| 5.    | Resnet     | 97.5            | 0.97      |
| 6.    | RNN        | 87.8            | 0.70      |

</div>

Ranking Accuracy: The algorithm produces more accurate and stable PageRank scores after approximately 25 iterations.

## PageRank Score Comparison

<div align = "center">
  
| S. No | Node ID | Google PageRank | Proposed Algorithm PageRank |
|-------|---------|----------------|-----------------------------|
| 1     | 4985    | 0.00381        | 0.00684                     |
| 2     | 4897    | 0.00357        | 0.00639                     |
| 3     | 4996    | 0.00277        | 0.00502                     |
| 4     | 4998    | 0.00273        | 0.00497                     |
| 5     | 4982    | 0.00257        | 0.00493                     |

</div>

**Correlation Analysis:** A strong positive correlation between the proposed PageRank scores and in-degree centrality highlights the importance of incoming links in determining page relevance.

**GRAPHICAL ANALYSIS**

<table>
    <tr>
        <td>
            <img src="https://github.com/user-attachments/assets/3bac2d2a-28c1-4a3c-a1c2-1f372ddb71e3" alt="Convergence" width="300">
            <p align="center">Convergence</p>
        </td>
        <td>
            <img src="https://github.com/user-attachments/assets/232ff19c-b215-4701-b74c-8964565ce6b9" alt="Correlation Matrix" width="300">
            <p align="center">Correlation Matrix</p>
        </td>
        <td>
            <img src="https://github.com/user-attachments/assets/7f9cbc75-df71-4f6d-9372-2fae63a1e391" alt="Distribution" width="300">
            <p align="center">Distribution of PageRank Score</p>
        </td>
    </tr>
</table>

# Conclusion

This work underscores the importance of developing an efficient and accurate page ranking algorithm to meet the growing demands of information retrieval in dynamic and large-scale web environments. By integrating Stother-William’s matrix multiplication into the page ranking process, the proposed algorithm demonstrates a significant reduction in processing time ranging from 0.04 to 15.7 seconds thereby surpassing the computational efficiency of existing algorithms. The enhanced algorithm stabilizes PageRank scores after approximately 25 iterations highlighting its superior convergence capabilities.

</div>

# Credits

**1) Dataset link:** https://snap.stanford.edu/data/web-Google.html

**2) Contribution:** 

a) Dr. M Raja, Associate Professor, Vellore Institute of Technology, Chennai

b) Saket Verma, M.Tech CSE, Vellore Institute of Technology, Chennai
