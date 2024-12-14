# **Doubling Dimension Analysis Using Cover Trees**

This repository implements two algorithms for computing the **doubling dimension** of graphs using **cover trees**, a hierarchical data structure. The doubling dimension is a measure of the intrinsic dimensionality of a graph and plays a critical role in analyzing graph embeddings, metric space clustering, and scalable algorithms.

- **Algorithm 1**: Adopts an exhaustive, greedy approach to evaluate all nodes for optimal accuracy in computing the doubling dimension. While this method provides precise results, it incurs higher computational overhead.
- **Algorithm 2**: Leverages clustering and targeted center selection to approximate the doubling dimension efficiently. This approach significantly reduces computational time while maintaining near-optimal accuracy.

The repository includes applications on real-world datasets, such as Twitter interaction networks and Facebook ego networks, demonstrating the trade-offs between accuracy and efficiency. It is particularly useful for graph analysis, metric space embedding, and scalable clustering tasks.

---

## **Files Included**

1. **`algorithm1.ipynb`**  
   Implements the exhaustive, greedy approach to compute the doubling dimension. This method systematically evaluates all possible nodes to identify the optimal doubling dimension with maximum accuracy.

2. **`algorithm2.ipynb`**  
   Implements the optimized clustering-based approach to compute the doubling dimension. This algorithm strategically selects one starting node and reduces computational complexity by approximating the doubling dimension.

3. **`congress_network_data.json`**  
   This dataset represents the Twitter interaction network for the **117th United States Congress**, encompassing both the House of Representatives and the Senate.  
   - **Source**: [SNAP: Stanford Large Network Dataset Collection](https://snap.stanford.edu/data/congress-twitter.html)  
   - **Description**: The dataset quantifies the transmission probabilities between members based on interactions like retweets, quote tweets, replies, and mentions. It was collected using Twitter’s API and provides a real-world graph for testing the algorithms. 

4. **`facebook.txt`**  
   This dataset consists of ego networks from Facebook, where nodes represent individuals and edges represent friendships.  
   - **Source**: [SNAP: Stanford Large Network Dataset Collection](https://snap.stanford.edu/data/ego-Facebook.html)  
   - **Description**: The dataset captures the structure of friend lists and circles, making it a useful test case for analyzing the geometric properties of social networks.

---


---

