# 5010671_SoumyajitBiswas
Cognizant Digital Nurture 3.0 (Deepskilling) Java FSE Assignments

**WEEK-1 (DSA)**

1) **Understanding the Problem**
Importance of Data Structures and Algorithms
Efficient data structures and algorithms are crucial for handling large inventories because:

Efficient Storage: Proper data structures help in storing data efficiently, reducing space complexity.
Fast Retrieval: Algorithms optimized for certain data structures ensure quick access and retrieval of data.
Scalability: As the inventory grows, the system must maintain performance. Efficient algorithms ensure scalability.
Data Integrity: Proper structures help in maintaining data consistency and integrity.
Suitable Data Structures
ArrayList: Provides dynamic arrays, allowing resizing as needed. Suitable for storing products when quick access by index is required.
HashMap: Allows storing key-value pairs, making it efficient for search, insert, and delete operations based on keys (e.g., product IDs).

**Analysis**
Time Complexity
Add Product: O(1) on average for HashMap.
Update Product: O(1) on average for HashMap.
Delete Product: O(1) on average for HashMap.
Optimization
Batch Operations: To handle large updates, consider batch operations to reduce overhead.
Concurrency Handling: Use concurrent data structures (e.g., ConcurrentHashMap) if multiple threads access the inventory.
