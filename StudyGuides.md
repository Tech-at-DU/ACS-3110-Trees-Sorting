# Quiz Study Guides

## General Information

- **Grading**: Quizzes will be graded with an answer key by the course instructor (Dani). Some questions may have multiple correct answers. Partial credit given as applicable.
- **Accommodations**: If you have a disability that requires accommodations for quizzes, you must follow the DU Accommodations Policy, then clarify with the course instructor exactly what accommodations will be made at least 24 hours before the quiz.

## Tips to Prepare

- Review resources and starter code found in the course repo.
- Complete the homework assigned after the relevant lessons. Work with other students, discuss your design and code, ask for feedback from others, and improve your code.
- If you were absent for any class sessions, it's essential to catch up on what you missed. Review the lesson topics and resources, watch videos of class activities when available, do the activities on your own, and discuss with classmates who attended and took notes.
- Use the course Slack channel (`#acs-3110`) to coordinate study sessions with classmates, ask questions when you're stuck, and share relevant resources you find.

## Quiz 1 Study Guide

### Iterative Sorting Algorithms (Bubble Sort, Selection Sort, Insertion Sort)

- Describe the major steps of each iterative sorting algorithm (bubble sort, selection sort, and insertion sort) in pseudocode or plain English.
- Write code snippets to complete partial implementations of these 3 algorithms.
- Describe what progress towards sorting is made after each iteration of the outer loop of these 3 algorithms. That is, describe what changes have been made that show the algorithm is modifying the input list so that it's closer to sorted order.
- Analyze the best case and worst case time complexity of these 3 algorithms and how the triangular series is related to their complexity.
- Recommended: Play with VisuAlgo's interactive sorting visualizations, pause the animation part-way through and test if you can describe the algorithm's progress.

### Divide-and-Conquer Recursion

- Describe the steps of divide-and-conquer algorithms (divide, conquer, combine), including binary search, merge sort, and quick sort.

### Recursive Sorting Algorithms (Merge Sort, Quick Sort)

- Describe how the merge algorithm combines two sorted lists into one sorted list.
- Write code snippets to complete a partial implementation of the merge algorithm.
- Analyze the time complexity of recursive merge sort and its merge algorithm.
- Describe how the partition algorithm chooses a pivot and swaps values in-place.
- Draw the execution tree diagram of quick sort given an input and choice of pivot.
- Analyze the actual time complexity of quick sort on a specific input and choice of pivot, then compare your result to its best case and worst case time complexity.
- Highly recommended: Review the video of the quick sort review activity from class. If you were absent on that class day, it's especially helpful to do the activity described in the video (drawing several quick sort execution trees) on your own, then compare and discuss your results with classmates who attended that day.

## Quiz 2 Study Guide

### K-ary Search Trees (Prefix Trees, aka Tries)

- Draw a diagram of how a prefix tree (trie) data structure is organized in memory.
- Describe the steps required to insert a new string into a trie, determine whether a complete string is in a trie, or find all strings in a trie that complete a given prefix.
- Analyze the worst case time complexity of trie insert and search operations and what features of the trie structure or strings it holds affect the complexity analysis.
- Recommended: Play with USF's interactive trie visualization and insert several strings with similar prefixes. Use the trie diagram to check your understanding of how to find strings in the trie and some not in the trie, then test if your process is the same as the animation played when you enter test strings into the "Find" box.

### Rotating Binary Search Trees (AVL Trees)

- Draw a diagram of how an AVL tree data structure is organized in memory.
- Define balance factor for AVL trees, show how it is calculated, and which values are considered balanced and which are unbalanced.
- Describe and perform the steps to search/find whether a value is in an AVL tree.
- Describe and perform the steps to insert a new value into an AVL tree.
- Describe rotations for AVL trees: single (left, right) and double (left-right, right-left) and how they change a subtree's structure and balance factor.
- Analyze the time complexity of AVL tree insert and search operations and what features of the tree structure and how it's balanced affect the complexity analysis.
- Recommended: Play with VisuAlgo's interactive AVL tree visualization and insert new values that would make the tree less balanced. Pause the animation to step through it slowly and test if you can predict which rotations will occur and where.

## Quiz 3 Study Guide

### Multiple Key Search Trees (2-3 Trees, B-Trees)

- Draw a diagram of how a 2-3 tree data structure is organized in memory.
- Describe the difference between 2-way nodes and 3-way nodes, how many keys each has, and how keys partition all keys in their left, middle, and right subtrees.
- Describe and perform the steps to search/find whether a value is in a 2-3 tree.
- Describe and perform the steps to insert a new value into a 2-3 tree, including any split and promote operations if/when they are triggered.
- Explain which level leaf nodes are on and why this is always true.
- Analyze the time complexity of 2-3 tree insert and search operations and what features of the tree structure and how it's balanced affect the complexity analysis.
- Recommended: Play with USF's interactive B-tree visualization with max degree = 3 for 2-3 trees and insert several values to see the split and promote operations that change the tree's structure. Use the diagram to check your understanding of how to find values that are in the tree and test if your process is the same as the animation played when you enter test values into the "Find" box.
- Recommended: Video 10.B.1: 2-3 Trees & B-Trees Lesson
- Not covered on Quiz 3: Delete operation or general B-trees with max degree > 3.

### Priority Queues & Heaps (Binary Heaps, Heapsort)

- Draw a diagram of how a binary heap data structure is organized in memory (using an array) and how it is conceptually organized as a complete binary tree.
- Describe the steps required to insert a new value into a binary heap or delete the root (min or max value) in a min or max binary heap, including the bubble down or bubble up helper methods.
- Write code snippets to complete a partial implementation of the above methods.
- Analyze the worst case time complexity of binary heap insert and delete methods and the bubble down or bubble up helper methods these operations trigger. Hint: time complexity is based on the shape of the (conceptual) complete binary tree.
- Write pseudocode or Python code to implement heap sort using a binary heap.
- Highly recommended: Review the binary heap worksheet or digital practice questions completed in class and compare your answers with classmates.
- Recommended: Video 11.B.2: Binary Heaps & Heap Sort Lesson
