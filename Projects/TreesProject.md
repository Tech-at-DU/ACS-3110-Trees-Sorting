# ACS 3310: Advanced Trees & Sorting Algorithms

## Trees Project Guidelines

## Project Summary

For this project, you will implement one of the tree structures below, write a basic unit test suite, find or create an appropriate dataset or application to use it with, and write a technical article to explain your project, how it works, and what you learned. On the final class (Dec 12th), you will give a brief (~5 min) presentation explaining the project based on your technical article. You can work individually or with a partner on this project. Groups of 3 or more students are not allowed.

## Project Options

**Select one of the following tree structures and an appropriate dataset it can be applied to**:

- An ideal project is to **integrate a tree we studied in class into an existing project** you've already built to add new functionality or improve performance of an existing feature
- Self-balancing binary search tree with rotations: AVL tree (or similar: splay tree)
- Self-balancing search tree with multiple keys: 2-3 tree (or stretch challenge: B-tree)
- Other k-ary (k-way) tree (not necessarily balanced, depending on application) such as a decision tree for classification or regression (Data Science concentration students only)
- Space-partitioning tree: 2D quadtree or 3D octree (or stretch challenge: k-d tree)
- Other tree structures and applications are welcome but **require prior instructor approval**

## Example Applications

- Implement an iterable ordered tree map (map ADT implemented with a search tree) that guarantees O(log n) running time for search, insertion, and deletion, and allows ordered traversal to retrieve all entries in order by key. An example application of a tree map is to store a very large phone book and traverse it to retrieve all names in alphabetical order.
- Implement an abstract syntax tree created by parsing a mathematical expression input by the user, construct the tree, evaluate and output the expression [Pinecone example]
- Implement a k-ary search tree to store a phylogenetic tree of a dataset of animal species that allows operations such as finding the closest common ancestor of two given species
- Implement a quadtree to represent a bitmap image with compression to reduce file size, or to reduce computational complexity of a grid-based game like Conway's Game of Life
- Implement a quadtree to recursively cluster 2D locations on a map (or use an octree to cluster 3D locations in a space) [example of quadtree used in an iOS library]

# Presentation & Article Guidelines

General article guidelines are similar to CS 1.3 Article Guidelines but somewhat more flexible due to the open-ended nature of independent projects like this. Beyond this, here are major points that I recommend you cover in your project presentation and article: Explain what problem you are solving and/or helpful background on the problem What type of tree you are using to solve this problem, what it does, and how it works Explain what exactly you built Show an example of it working. Conclude why this is better than a naive solution. Maybe: Talk about time and space complexity. No set length, but should cover what you worked on.

## Grading Guidelines

### Trees Project Code

**Earn points for items below satisfied in project and code.**<br>
_8 out of 12 points total is passing._

- 3 points for technical complexity undertaken (examples: 1 point for prefix tree; 2 points for AVL tree, 2-3 tree, game tree, or quadtree; 3 points for B-tree, octree, or k-d tree)
- 3 points for completion and correctness (i.e., does the project work as expected?)
- 1 point for high level of polish (i.e., is the finished project a high quality portfolio item?)
- 2 points for high code quality (use the [Code Review Rubric](https://docs.google.com/document/d/1zx0snt-A1OZakZSAemb6hjJSsQeyCQQJq68XiIyOcKM/edit) as a guideline)
- 3 points for commit history indicating consistent and well-paced project development over 2+ weeks (example: 0 points for most commits in the final few days of the course)

### Trees Project Article

**Earn points for items below included in article.**<br>
_8 out of 12 points total is considered passing._

- 3 points for describing in detail how the tree structure in your project works (concept)
- 2 points for describing how you implemented and used the tree structure (application)
- 2 points for article length (example: 1 point for 4+ minute read; 2 points for 6+ min read)
- 1 point for including algorithm analysis and how the tree structure improves scalability
- 1 point for including pseudocode or code snippets at relevant places in your article
- 1 point for including 3+ diagrams or images relevant to your article (memes don't count)
- 1 point for citing sources of all borrowed pseudocode, code, diagrams, and images
- 1 point for publishing article online, +1 bonus point for publishing in a Medium publication
- –12 points for plagiarising significant portions of article text, code, diagrams, or images. This will be dealt with according to Dominican University's academic honesty and integrity policy
