# Algorithms-Design-Analysis

### Exp 1: Linear Search and Recursive Binary Search

**Linear Search** is a straightforward search algorithm that sequentially checks each element of a list until the desired element is found or the entire list is traversed. Its time complexity is O(n), where n is the number of elements in the list. Linear search is inefficient for large datasets as it does not leverage any information about the order of the elements.

**Recursive Binary Search** is a more efficient algorithm that works on sorted lists. It divides the list into halves, recursively searching the relevant half based on whether the target element is greater than or less than the midpoint. This reduces the search space by half with each step, resulting in a time complexity of O(log n). This makes binary search much faster than linear search for large datasets, but it requires the data to be sorted beforehand.

### Exp 2: Insertion, Bubble, and Selection Sort

**Insertion Sort** builds the sorted list one element at a time. It takes one element from the input and inserts it in the correct position within the already sorted section of the list. This algorithm is efficient for small datasets or nearly sorted data but has a time complexity of O(n²) in the worst case for larger unsorted data.

**Bubble Sort** repeatedly compares adjacent elements in the list and swaps them if they are in the wrong order. This process continues until no more swaps are needed, indicating that the list is sorted. Though simple, bubble sort has a time complexity of O(n²) and is inefficient for large datasets.

**Selection Sort** selects the smallest (or largest, depending on sorting order) element from the unsorted portion of the list and swaps it with the first element of the unsorted section. It then repeats this process for the remaining unsorted elements. Selection sort also has a time complexity of O(n²), and while it makes fewer swaps than bubble sort, it is still inefficient for large datasets.

### Exp 3: Merge Sort and Quick Sort

**Merge Sort** is a divide-and-conquer algorithm that splits the list into halves, recursively sorts each half, and then merges the sorted halves. It guarantees a time complexity of O(n log n), making it highly efficient for large datasets. However, it requires additional space for merging, leading to an O(n) space complexity.

**Quick Sort** is another divide-and-conquer algorithm. It selects a 'pivot' element and partitions the list such that all elements less than the pivot are to its left, and all elements greater are to its right. The process is then recursively applied to the sub-lists. Quick sort's average time complexity is O(n log n), but in the worst case (poor pivot selection), it can degrade to O(n²). It is efficient in practice and typically faster than merge sort.

### Exp 4: Strassen’s Algorithm

**Strassen’s Algorithm** is an optimized algorithm for matrix multiplication that reduces the time complexity compared to the traditional O(n³) method. Strassen's algorithm uses a divide-and-conquer approach, breaking matrices into submatrices and performing fewer multiplications. This results in a time complexity of approximately O(n^2.81), which is faster for large matrices. It is particularly useful for applications that involve large-scale matrix operations.

### Exp 5: Knapsack (Greedy)

The **Greedy Knapsack Problem** is an optimization problem where the goal is to maximize the value of items placed in a knapsack with a weight limit. In the **greedy approach**, items are selected based on a ratio of their value to weight (value/weight), choosing the most valuable items first until the capacity is reached. This approach works efficiently for the **fractional knapsack problem**, where items can be broken into smaller parts, with a time complexity of O(n log n). However, it does not always yield optimal solutions for the **0/1 knapsack problem**, where items cannot be divided.

### Exp 6: Prim’s Algorithm

**Prim’s Algorithm** is a greedy algorithm used to find the minimum spanning tree (MST) of a weighted, connected graph. It starts with a single node and expands the MST by adding the lowest-weight edge that connects a node in the tree to a node outside of it. This process continues until all nodes are included in the MST. Prim's algorithm has a time complexity of O(V²) with an adjacency matrix or O(E log V) with an adjacency list and a priority queue, where V is the number of vertices and E is the number of edges.

### Exp 7: Kruskal’s Algorithm

**Kruskal’s Algorithm** is another greedy algorithm used to find the minimum spanning tree of a graph. It works by sorting all edges in ascending order of weight and then adding edges to the MST, ensuring that no cycles are formed. The process continues until the MST includes all vertices. Kruskal’s algorithm typically has a time complexity of O(E log E), where E is the number of edges, making it efficient for sparse graphs.

### Exp 8: Dijkstra’s Algorithm

**Dijkstra’s Algorithm** is used to find the shortest path from a source node to all other nodes in a weighted graph. It works by iteratively selecting the node with the smallest known distance from the source and updating the distances to its neighboring nodes. This continues until the shortest path to every node is determined. Dijkstra's algorithm has a time complexity of O(V²) with an adjacency matrix or O(E log V) with a priority queue, making it efficient for graphs with non-negative weights.