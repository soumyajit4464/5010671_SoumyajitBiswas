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



2) **Understanding Asymptotic Notation**
Big O Notation
Big O notation is a mathematical notation used to describe the upper bound of an algorithm's running time. It provides an estimate of the worst-case scenario in terms of input size, helping in understanding the efficiency and scalability of an algorithm.

Scenarios for Search Operations
Best Case: The minimum time an algorithm takes to complete, often when the element is found in the first iteration.
Average Case: The expected time an algorithm takes to complete, averaging over all possible inputs.
Worst Case: The maximum time an algorithm takes to complete, often when the element is not found, requiring the algorithm to go through all elements.

**Analysis**
Time Complexity
Linear Search: O(n) in the worst case, where n is the number of products. It scans each element until it finds the target or reaches the end.
Binary Search: O(log n) in the worst case, assuming the array is sorted. It repeatedly divides the search interval in half.
Suitability
Binary Search: More suitable for the platform due to its significantly lower time complexity (O(log n)) compared to linear search (O(n)). However, it requires the array to be sorted, which might add overhead if the array is frequently updated.



3) **Understanding Sorting Algorithms**
Bubble Sort
Bubble Sort is a simple comparison-based sorting algorithm. It repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. This process is repeated until the list is sorted.

Time Complexity: O(n^2) in the worst and average cases, O(n) in the best case (already sorted array).
Insertion Sort
Insertion Sort builds the sorted array one element at a time, by repeatedly picking the next element and inserting it into the correct position.

Time Complexity: O(n^2) in the worst and average cases, O(n) in the best case (already sorted array).
Quick Sort
Quick Sort is a divide-and-conquer algorithm. It selects a pivot element, partitions the array around the pivot, and then recursively sorts the sub-arrays.

Time Complexity: O(n log n) on average, O(n^2) in the worst case, but with good pivot selection, the worst case is rare.
Merge Sort
Merge Sort is a stable, divide-and-conquer sorting algorithm. It divides the array into halves, recursively sorts each half, and then merges the sorted halves.

Time Complexity: O(n log n) in all cases (best, average, and worst).

**Analysis**
Time Complexity
Bubble Sort: O(n^2) in the worst and average cases, making it inefficient for large datasets.
Quick Sort: O(n log n) on average, making it significantly faster for large datasets. In the worst case (rare with good pivot selection), it can degrade to O(n^2).
Preference for Quick Sort
Quick Sort is generally preferred over Bubble Sort because:

Efficiency: Quick Sort has an average time complexity of O(n log n), making it suitable for large datasets.
Practical Performance: Despite its worst-case complexity of O(n^2), Quick Sort's average-case performance is much better than Bubble Sort.
In-place Sorting: Quick Sort is an in-place sorting algorithm, requiring less additional memory compared to Merge Sort.


4) **Understanding Array Representation**
Array Representation in Memory
Arrays are a collection of elements stored in contiguous memory locations. The key characteristics of arrays are:

Fixed Size: The size of an array is defined at the time of creation and cannot be changed.
Index-Based Access: Elements can be accessed directly using their index, making access time O(1).
Contiguous Memory Allocation: Elements are stored in contiguous memory locations, ensuring efficient memory usage.
Advantages of Arrays
Fast Access: O(1) time complexity for accessing elements.
Memory Efficiency: Contiguous allocation reduces memory overhead.
Cache Friendliness: Contiguous memory locations improve cache performance.

**Analysis**
Time Complexity
Add Employee: O(1) on average, but O(n) when resizing the array is necessary.
Search Employee: O(n) in the worst case since it involves linear search.
Traverse Employees: O(n) as it needs to iterate through all employees.
Delete Employee: O(n) in the worst case due to the need to find and shift elements.
Limitations of Arrays
Fixed Size: Initial capacity must be defined, and resizing arrays can be costly.
Inefficient Deletions: Deleting elements requires shifting, leading to O(n) complexity.
Not Dynamic: Arrays are not dynamic in size, requiring manual resizing.



5) **Understanding Linked Lists**
Types of Linked Lists
Singly Linked List: Each node contains data and a reference to the next node. Operations like insertion and deletion are efficient but traversal is only possible in one direction.
Doubly Linked List: Each node contains data, a reference to the next node, and a reference to the previous node. This allows traversal in both directions but requires extra memory for storing two references.

**Analysis**
Time Complexity
Add Task: O(n) in the worst case as it may require traversing to the end of the list.
Search Task: O(n) since it involves linear search through the list.
Traverse Tasks: O(n) as it needs to iterate through all nodes.
Delete Task: O(n) because it may require traversing to find the node to delete.
Advantages of Linked Lists over Arrays for Dynamic Data
Dynamic Size: Linked lists can grow and shrink dynamically without needing to resize or reallocate memory.
Efficient Insertions/Deletions: Insertion and deletion of elements are more efficient than arrays, especially when the size of the dataset is unpredictable.
Memory Utilization: Linked lists do not require a contiguous block of memory, making them more memory efficient when the size of the dataset changes frequently.



6) **Understanding Search Algorithms**
Linear Search
Description: A straightforward algorithm that checks each element in the list sequentially until the target element is found or the list ends.
Time Complexity: O(n) in the worst case, where n is the number of elements in the list.
Binary Search
Description: A more efficient algorithm that works on sorted lists. It repeatedly divides the search interval in half, reducing the search space significantly.
Time Complexity: O(log n) in the worst case, where n is the number of elements in the list.

**Analysis**
Time Complexity
Linear Search: O(n) in the worst case, as it involves checking each element sequentially.
Binary Search: O(log n) in the worst case, as it reduces the search space by half with each step.
When to Use Each Algorithm
Linear Search: Suitable for small or unsorted datasets. It is simple to implement and doesn't require the data to be sorted.
Binary Search: Preferred for large, sorted datasets. It is more efficient due to its logarithmic time complexity.



7) **Understanding Recursive Algorithms**
Concept of Recursion
Recursion is a technique where a function calls itself to solve smaller instances of the same problem until a base condition is met. This approach can simplify problems that have a repetitive or nested structure, such as tree traversals, combinatorial problems, and divide-and-conquer algorithms.

Example: Financial Forecasting
In financial forecasting, recursion can be used to predict future values based on past data and growth rates. For instance, predicting future value based on a constant growth rate can be naturally expressed using a recursive formula.

**Analysis**
Time Complexity
The time complexity of the recursive algorithm is O(n), where n is the number of years. This is because each recursive call reduces the problem size by one year until the base case is reached.
Optimizing the Recursive Solution
Memoization: To avoid redundant calculations and excessive computation, we can store the results of subproblems (e.g., the predicted value for each year) and reuse them when needed. This technique is called memoization.
Iterative Approach: Alternatively, we can use an iterative approach to compute the future value, which can be more efficient and easier to understand.
