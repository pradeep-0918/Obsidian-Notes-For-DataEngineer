---
title: DSA — Complete Problem Solving Syllabus & Pattern Roadmap
category: DSA
level: Beginner → Advanced → Competitive Programming
purpose: Placements + Product Companies + Competitive Programming
language: Java
status: Learning
tags:
  - dsa
  - algorithms
  - problem-solving
  - competitive-programming
  - placement-preparation
  - leetcode
  - coding-interviews
---
# 🚀 DSA — Complete Problem Solving Syllabus

> [!important]
> **Goal:** Do not memorize solutions.
>
> Train your brain to recognize:
>
> `Question → Constraints → Observation → Pattern → Template → Implementation → Optimization`
>
> The final objective is to look at a new problem and quickly identify which family of techniques can solve it.

---

# 0. 🧠 Problem-Solving Foundation

Before learning advanced DSA, master the following.

## 0.1 Complexity Analysis

* [[Big O Notation]]
* [[Big Omega]]
* [[Big Theta]]
* [[Time Complexity]]
* [[Space Complexity]]
* [[Amortized Analysis]]

### Complexity Classes

* [[O(1)]]
* [[O(log n)]]
* [[O(n)]]
* [[O(n log n)]]
* [[O(n²)]]
* [[O(n³)]]
* [[O(2^n)]]
* [[O(n!)]]

### Must Learn

* [[Complexity Comparison]]
* [[Worst Case Analysis]]
* [[Average Case Analysis]]
* [[Best Case Analysis]]
* [[Nested Loop Complexity]]
* [[Recursive Complexity]]
* [[Recurrence Relations]]
* [[Master Theorem]]
* [[Input Constraint Analysis]]

### Pattern

Whenever you see:

```text
n ≤ 20
→ exponential/backtracking/bitmask may work

n ≤ 100
→ O(n³) may work

n ≤ 1000
→ O(n²) may work

n ≤ 10⁵
→ O(n log n) / O(n)

n ≤ 10⁶
→ O(n) / optimized O(n log n)

n ≥ 10⁹
→ logarithmic / mathematical / binary search
```

---

# 1. 🧱 Programming Foundations

## 1.1 Arrays

* [[Array Basics]]
* [[Static Arrays]]
* [[Dynamic Arrays]]
* [[Array Traversal]]
* [[Insertion]]
* [[Deletion]]
* [[Rotation]]
* [[Reversal]]
* [[Frequency Counting]]
* [[In-place Modification]]

## 1.2 Strings

* [[String Basics]]
* [[Character Array]]
* [[StringBuilder]]
* [[String Manipulation]]
* [[Character Frequency]]
* [[Palindrome]]
* [[Anagram]]
* [[Substrings]]
* [[Subsequences]]

## 1.3 Hashing

* [[HashMap]]
* [[HashSet]]
* [[Frequency Map]]
* [[Counting]]
* [[Duplicate Detection]]
* [[Index Mapping]]
* [[Complement Lookup]]

## Core Patterns

* [[Frequency Pattern]]
* [[Lookup Pattern]]
* [[Counting Pattern]]
* [[Index Mapping Pattern]]
* [[Complement Pattern]]

---

# 2. 🔢 Mathematics for DSA

Mathematics is extremely important for advanced problem solving.

## 2.1 Number Theory

* [[Prime Numbers]]
* [[Prime Checking]]
* [[Sieve of Eratosthenes]]
* [[Prime Factorization]]
* [[Divisors]]
* [[GCD]]
* [[LCM]]
* [[Euclidean Algorithm]]
* [[Extended Euclidean Algorithm]]
* [[Modular Arithmetic]]
* [[Modular Inverse]]
* [[Fast Exponentiation]]
* [[Binary Exponentiation]]
* [[Euler Totient]]
* [[Chinese Remainder Theorem]]

## 2.2 Combinatorics

* [[Permutations]]
* [[Combinations]]
* [[Pascal Triangle]]
* [[nCr]]
* [[Catalan Numbers]]
* [[Inclusion Exclusion]]

## 2.3 Mathematical Patterns

* [[Parity]]
* [[Divisibility]]
* [[Modulo Pattern]]
* [[Digit Manipulation]]
* [[Bitwise Mathematics]]
* [[Invariants]]
* [[Mathematical Observation]]

---

# 3. 🔗 Linked Lists

## 3.1 Fundamentals

* [[Singly Linked List]]
* [[Doubly Linked List]]
* [[Circular Linked List]]
* [[Linked List Traversal]]
* [[Insertion]]
* [[Deletion]]
* [[Reverse Linked List]]

## 3.2 Important Problems

* [[Reverse Linked List]]
* [[Middle of Linked List]]
* [[Detect Cycle]]
* [[Find Cycle Start]]
* [[Remove Nth Node]]
* [[Merge Two Sorted Lists]]
* [[Intersection of Linked Lists]]
* [[Palindrome Linked List]]
* [[Reverse Nodes in K Group]]
* [[Rotate Linked List]]
* [[Copy List with Random Pointer]]

## Core Patterns

### Pattern 1 — Fast and Slow Pointer

Use when:

* middle element
* cycle detection
* cycle entry
* palindrome
* linked-list splitting

Template:

```java
ListNode slow = head;
ListNode fast = head;

while (fast != null && fast.next != null) {
    slow = slow.next;
    fast = fast.next.next;
}
```

### Pattern 2 — Dummy Node

Use for:

* insertion/deletion
* merging
* removing nodes
* manipulating head

```java
ListNode dummy = new ListNode(0);
dummy.next = head;
```

### Pattern 3 — Reversal

```java
ListNode prev = null;
ListNode curr = head;

while (curr != null) {
    ListNode next = curr.next;
    curr.next = prev;
    prev = curr;
    curr = next;
}

return prev;
```

---

# 4. 📚 Stack

## Topics

* [[Stack]]
* [[Monotonic Stack]]
* [[Min Stack]]
* [[Max Stack]]
* [[Expression Evaluation]]
* [[Parentheses]]
* [[Next Greater Element]]
* [[Next Smaller Element]]
* [[Previous Greater Element]]
* [[Previous Smaller Element]]

## Core Patterns

* [[Matching Pattern]]
* [[Monotonic Increasing Stack]]
* [[Monotonic Decreasing Stack]]
* [[Nearest Greater Pattern]]
* [[Nearest Smaller Pattern]]
* [[Contribution Pattern]]

## Must Solve

* [[Valid Parentheses]]
* [[Min Stack]]
* [[Daily Temperatures]]
* [[Next Greater Element]]
* [[Largest Rectangle in Histogram]]
* [[Trapping Rain Water]]

---

# 5. 🚶 Queue and Deque

* [[Queue]]
* [[Circular Queue]]
* [[Deque]]
* [[Priority Queue]]
* [[Monotonic Queue]]

## Patterns

* [[BFS Queue Pattern]]
* [[Sliding Window Maximum]]
* [[Monotonic Deque Pattern]]

---

# 6. 🔍 Searching

## 6.1 Linear Search

* [[Linear Search]]

## 6.2 Binary Search

* [[Binary Search]]
* [[Lower Bound]]
* [[Upper Bound]]
* [[First Occurrence]]
* [[Last Occurrence]]
* [[Search Insert Position]]
* [[Search in Rotated Array]]
* [[Peak Element]]
* [[Minimum in Rotated Array]]

## Most Important Pattern

### Binary Search on Answer

Recognize when:

> "Find minimum possible X"

or

> "Find maximum possible X"

and you can determine whether a candidate `X` is feasible.

Pattern:

```java
long low = ...;
long high = ...;

while (low <= high) {
    long mid = low + (high - low) / 2;

    if (check(mid)) {
        // move toward better answer
    } else {
        // move opposite
    }
}
```

## Binary Search Families

* [[Exact Search]]
* [[Boundary Search]]
* [[Rotated Array Search]]
* [[Peak Search]]
* [[Binary Search on Answer]]
* [[Minimum Feasible Value]]
* [[Maximum Feasible Value]]

---

# 7. ↔️ Two Pointers

## Topics

* [[Two Pointers]]
* [[Opposite Direction Pointers]]
* [[Same Direction Pointers]]
* [[Fast Slow Pointers]]
* [[Partition Pattern]]

## Recognition

Look for:

* sorted array
* pair/triplet
* target sum
* remove duplicates
* palindrome
* shrinking search space

## Templates

### Opposite Direction

```java
int left = 0;
int right = n - 1;

while (left < right) {

    if (condition) {
        left++;
    } else {
        right--;
    }
}
```

### Same Direction

```java
int left = 0;

for (int right = 0; right < n; right++) {

    while (!valid()) {
        left++;
    }

    // process window
}
```

---

# 8. 🪟 Sliding Window

One of the most important interview patterns.

## 8.1 Fixed Window

* [[Fixed Size Sliding Window]]
* [[Maximum Sum Subarray of Size K]]
* [[Average of Subarray]]

## 8.2 Variable Window

* [[Longest Substring]]
* [[Shortest Subarray]]
* [[Longest Subarray with Constraint]]
* [[At Most K]]
* [[Exactly K]]

## 8.3 Advanced

* [[Sliding Window Frequency Map]]
* [[Sliding Window with Set]]
* [[Sliding Window with Deque]]
* [[Minimum Window Substring]]

## Template

```java
int left = 0;

for (int right = 0; right < n; right++) {

    // add arr[right]

    while (!valid()) {
        // remove arr[left]
        left++;
    }

    // update answer
}
```

## Recognition Keywords

* longest
* shortest
* continuous
* contiguous
* substring
* subarray
* at most K
* at least K
* distinct elements

---

# 9. ➕ Prefix Sum

## Topics

* [[Prefix Sum]]
* [[Prefix XOR]]
* [[2D Prefix Sum]]
* [[Difference Array]]
* [[Range Sum]]
* [[Range Update]]

## Patterns

* [[Subarray Sum]]
* [[Subarray Sum Equals K]]
* [[Prefix Sum + HashMap]]
* [[Prefix XOR + HashMap]]
* [[Difference Array Pattern]]

## Template

```java
prefix[i + 1] = prefix[i] + arr[i];
```

For subarray:

```text
sum(l...r) = prefix[r + 1] - prefix[l]
```

---

# 10. 🧮 Sorting

## Basic

* [[Bubble Sort]]
* [[Selection Sort]]
* [[Insertion Sort]]

## Important

* [[Merge Sort]]
* [[Quick Sort]]
* [[Heap Sort]]
* [[Counting Sort]]
* [[Radix Sort]]
* [[Bucket Sort]]

## Patterns

* [[Sort and Scan]]
* [[Sort + Two Pointers]]
* [[Sort + Greedy]]
* [[Sort + Binary Search]]
* [[Custom Comparator]]

## Important Recognition

When a problem asks:

> "minimum operations"

> "maximum pairs"

> "closest values"

> "merge intervals"

First ask:

**Can sorting expose the structure?**

---

# 11. 📏 Intervals

## Topics

* [[Intervals]]
* [[Merge Intervals]]
* [[Insert Interval]]
* [[Interval Intersection]]
* [[Meeting Rooms]]
* [[Meeting Rooms II]]
* [[Activity Selection]]
* [[Calendar Scheduling]]

## Core Pattern

```text
Sort by start time.

If current.start <= previous.end:
    merge

else:
    create new interval
```

## Advanced

* [[Sweep Line]]
* [[Difference Array Intervals]]
* [[Event Sorting]]
* [[Coordinate Compression]]

---

# 12. 🧩 Recursion

## Fundamentals

* [[Recursion]]
* [[Base Case]]
* [[Recursive Case]]
* [[Call Stack]]
* [[Recursion Tree]]
* [[Backtracking]]
* [[Tail Recursion]]

## Must Master

For every recursive problem identify:

```text
1. State
2. Choice
3. Base Case
4. Transition
5. Return Value
```

---

# 13. 🔙 Backtracking

## Core Patterns

* [[Subsets]]
* [[Subsequences]]
* [[Permutations]]
* [[Combinations]]
* [[Combination Sum]]
* [[Palindrome Partitioning]]
* [[N Queens]]
* [[Sudoku]]
* [[Word Search]]
* [[Rat in a Maze]]

## Universal Template

```java
void backtrack(...) {

    if (baseCase) {
        answer.add(...);
        return;
    }

    for (choice : choices) {

        if (!valid(choice))
            continue;

        makeChoice(choice);

        backtrack(...);

        undoChoice(choice);
    }
}
```

## Recognition

Use backtracking when:

* generate all
* find all
* choose/not choose
* permutations
* combinations
* arrangements
* exhaustive search
* `n` is small

---

# 14. 🌳 Trees

One of the highest-priority DSA sections.

## 14.1 Binary Tree Fundamentals

* [[Binary Tree]]
* [[Tree Node]]
* [[Height]]
* [[Depth]]
* [[Level]]
* [[Leaf Node]]
* [[Subtree]]

## 14.2 Traversals

* [[Preorder]]
* [[Inorder]]
* [[Postorder]]
* [[Level Order]]
* [[Zigzag Traversal]]
* [[Boundary Traversal]]
* [[Vertical Traversal]]
* [[Diagonal Traversal]]
* [[Top View]]
* [[Bottom View]]
* [[Left View]]
* [[Right View]]

## 14.3 Tree Patterns

### Pattern 1 — DFS Return Information

Use when the answer depends on child subtrees.

```java
int dfs(Node root) {

    if (root == null)
        return 0;

    int left = dfs(root.left);
    int right = dfs(root.right);

    return ...;
}
```

Used for:

* [[Tree Height]]
* [[Balanced Binary Tree]]
* [[Diameter]]
* [[Maximum Path Sum]]
* [[Maximum Depth]]

### Pattern 2 — DFS Carry Information

```java
void dfs(Node node, int value) {
    ...
}
```

Used for:

* [[Root to Leaf Path]]
* [[Path Sum]]
* [[Binary Number from Root to Leaf]]
* [[Tree Path Problems]]

### Pattern 3 — Global Answer

```java
int ans = 0;

int dfs(Node root) {
    ...
    ans = Math.max(ans, value);
    return value;
}
```

Used for:

* [[Diameter of Binary Tree]]
* [[Maximum Path Sum]]
* [[Longest Path]]

### Pattern 4 — BFS

```java
Queue<Node> q = new LinkedList<>();
q.offer(root);

while (!q.isEmpty()) {

    int size = q.size();

    for (int i = 0; i < size; i++) {
        Node node = q.poll();
    }
}
```

Used for:

* [[Level Order]]
* [[Zigzag]]
* [[Right Side View]]
* [[Minimum Depth]]
* [[Level Based Problems]]

---

# 15. 🌲 Binary Search Tree

## Topics

* [[Binary Search Tree]]
* [[BST Search]]
* [[BST Insert]]
* [[BST Delete]]
* [[Validate BST]]
* [[Kth Smallest in BST]]
* [[Kth Largest in BST]]
* [[Lowest Common Ancestor in BST]]
* [[Predecessor]]
* [[Successor]]

## Key Insight

> **Inorder traversal of a BST produces sorted order.**

Therefore:

```text
BST + kth smallest
→ inorder

BST + range
→ exploit ordering

BST + ancestor
→ compare values
```

---

# 16. 🧠 Tree Advanced Patterns

* [[Lowest Common Ancestor]]
* [[Binary Lifting]]
* [[Tree Diameter]]
* [[Tree DP]]
* [[Rerooting DP]]
* [[Subtree Queries]]
* [[Euler Tour]]
* [[Tree Flattening]]
* [[Heavy Light Decomposition]]

## Must Master

* [[LCA Binary Tree]]
* [[LCA BST]]
* [[Distance Between Nodes]]
* [[Tree Diameter]]
* [[Maximum Path]]
* [[Subtree Sum]]
* [[Tree Queries]]

---

# 17. 🗺️ Graphs

Graphs are mandatory for high-level DSA.

## 17.1 Fundamentals

* [[Graph]]
* [[Vertex]]
* [[Edge]]
* [[Directed Graph]]
* [[Undirected Graph]]
* [[Weighted Graph]]
* [[Unweighted Graph]]
* [[Connected Graph]]
* [[Disconnected Graph]]
* [[Degree]]
* [[Indegree]]
* [[Outdegree]]

## Representation

* [[Adjacency Matrix]]
* [[Adjacency List]]
* [[Edge List]]

---

# 18. 🔎 Graph Traversal

## DFS

* [[Graph DFS]]
* [[Recursive DFS]]
* [[Iterative DFS]]

Template:

```java
void dfs(int node) {

    visited[node] = true;

    for (int next : graph[node]) {

        if (!visited[next]) {
            dfs(next);
        }
    }
}
```

## BFS

* [[Graph BFS]]
* [[Shortest Path Unweighted Graph]]
* [[Multi Source BFS]]

Template:

```java
Queue<Integer> q = new LinkedList<>();

q.offer(source);
visited[source] = true;

while (!q.isEmpty()) {

    int node = q.poll();

    for (int next : graph[node]) {

        if (!visited[next]) {
            visited[next] = true;
            q.offer(next);
        }
    }
}
```

---

# 19. 🔗 Graph Core Patterns

## Pattern 1 — Connected Components

* [[Number of Islands]]
* [[Connected Components]]
* [[Flood Fill]]
* [[Counting Components]]

Recognition:

> "How many groups?"

> "How many islands?"

> "How many disconnected regions?"

---

## Pattern 2 — Cycle Detection

### Undirected

* [[Cycle Detection Undirected Graph]]
* [[DFS Parent Method]]
* [[DSU Cycle Detection]]

### Directed

* [[Cycle Detection Directed Graph]]
* [[DFS Recursion Stack]]
* [[Kahn Algorithm]]

---

# 20. 🧭 Topological Sort

* [[Topological Sort]]
* [[Kahn Algorithm]]
* [[DFS Topological Sort]]
* [[Course Schedule]]
* [[Course Schedule II]]
* [[Dependency Graph]]

## Recognition

Whenever you see:

```text
prerequisite
dependency
before
after
ordering
task dependency
build order
course prerequisite
```

Think:

> **Directed Graph + Topological Sort**

---

# 21. 🛣️ Shortest Path

## Unweighted

* [[BFS Shortest Path]]

## Weighted

* [[Dijkstra]]
* [[Bellman Ford]]
* [[Floyd Warshall]]

## Special Cases

* [[0-1 BFS]]
* [[DAG Shortest Path]]
* [[Multi Source Shortest Path]]

## Recognition

```text
unweighted
→ BFS

positive weighted
→ Dijkstra

negative edges
→ Bellman Ford

all pairs
→ Floyd Warshall

weights only 0/1
→ 0-1 BFS
```

---

# 22. 🔗 Disjoint Set Union

* [[Disjoint Set Union]]
* [[Union Find]]
* [[Path Compression]]
* [[Union by Rank]]
* [[Union by Size]]

Template:

```java
int find(int x) {
    if (parent[x] == x)
        return x;

    return parent[x] = find(parent[x]);
}

void union(int a, int b) {

    a = find(a);
    b = find(b);

    if (a == b)
        return;

    if (size[a] < size[b]) {
        int temp = a;
        a = b;
        b = temp;
    }

    parent[b] = a;
    size[a] += size[b];
}
```

## Applications

* [[Connected Components]]
* [[Cycle Detection]]
* [[Kruskal]]
* [[Network Connectivity]]
* [[Dynamic Connectivity]]

---

# 23. 🌐 Minimum Spanning Tree

* [[Minimum Spanning Tree]]
* [[Kruskal Algorithm]]
* [[Prim Algorithm]]

## Recognition

Look for:

> Connect all nodes with minimum total cost.

---

# 24. 🏔️ Heap / Priority Queue

## Topics

* [[Heap]]
* [[Min Heap]]
* [[Max Heap]]
* [[Priority Queue]]
* [[Heapify]]
* [[Kth Largest]]
* [[Kth Smallest]]
* [[Top K Elements]]
* [[Median]]
* [[Merge K Sorted Lists]]

## Patterns

* [[Top K Pattern]]
* [[Two Heap Pattern]]
* [[Kth Element Pattern]]
* [[Priority Queue Greedy]]
* [[Heap + Graph]]

### Top K Template

```java
PriorityQueue<Integer> pq =
    new PriorityQueue<>();

for (int x : arr) {

    pq.offer(x);

    if (pq.size() > k)
        pq.poll();
}
```

---

# 25. 🔤 Trie

## Topics

* [[Trie]]
* [[Trie Insert]]
* [[Trie Search]]
* [[Trie Prefix Search]]
* [[Trie Delete]]
* [[Word Dictionary]]
* [[Word Search Trie]]

## Applications

* [[Prefix Matching]]
* [[Autocomplete]]
* [[Dictionary Search]]
* [[Word Search]]
* [[XOR Trie]]

---

# 26. 💰 Greedy Algorithms

Greedy is not simply "take the largest."

You must understand why a local decision produces a globally optimal result.

## Fundamentals

* [[Greedy Algorithm]]
* [[Greedy Choice]]
* [[Exchange Argument]]
* [[Optimal Substructure]]
* [[Proof of Greedy]]

## Patterns

* [[Activity Selection]]
* [[Interval Scheduling]]
* [[Fractional Knapsack]]
* [[Job Sequencing]]
* [[Minimum Platforms]]
* [[Jump Game]]
* [[Gas Station]]
* [[Huffman Coding]]
* [[Meeting Scheduling]]

## Recognition

Ask:

> Can I make the best local decision and prove it never hurts the future?

---

# 27. 🧮 Dynamic Programming

One of the most important sections.

## DP Fundamentals

* [[Dynamic Programming]]
* [[Overlapping Subproblems]]
* [[Optimal Substructure]]
* [[State]]
* [[Transition]]
* [[Base Case]]
* [[Memoization]]
* [[Tabulation]]
* [[Space Optimization]]

---

# 28. 1D DP

* [[Climbing Stairs]]
* [[House Robber]]
* [[Fibonacci DP]]
* [[Min Cost Climbing Stairs]]
* [[Decode Ways]]

Pattern:

```text
dp[i] = best answer considering first i elements
```

---

# 29. Linear DP

* [[Maximum Subarray DP]]
* [[Kadane Algorithm]]
* [[House Robber]]
* [[Stock DP]]
* [[Jump Game]]

---

# 30. Grid DP

* [[Grid DP]]
* [[Unique Paths]]
* [[Minimum Path Sum]]
* [[Maximum Path in Grid]]
* [[Obstacle Grid]]
* [[Cherry Pickup]]

Pattern:

```java
dp[i][j] =
    best(
        dp[i-1][j],
        dp[i][j-1]
    ) + value;
```

---

# 31. Knapsack DP

Extremely important.

## Patterns

* [[0/1 Knapsack]]
* [[Unbounded Knapsack]]
* [[Bounded Knapsack]]
* [[Subset Sum]]
* [[Partition Equal Subset Sum]]
* [[Target Sum]]
* [[Coin Change]]
* [[Coin Change II]]

## Recognition

Look for:

```text
choose / don't choose
weight
capacity
target
sum
items
maximum value
minimum coins
```

---

# 32. Subsequence DP

* [[Longest Increasing Subsequence]]
* [[Longest Common Subsequence]]
* [[Longest Palindromic Subsequence]]
* [[Edit Distance]]
* [[Distinct Subsequences]]
* [[Shortest Common Supersequence]]

## Pattern

Usually:

```text
dp[i][j]
```

represents the best answer using prefixes of two sequences.

---

# 33. Interval DP

* [[Matrix Chain Multiplication]]
* [[Burst Balloons]]
* [[Palindrome Partitioning]]
* [[Optimal BST]]
* [[Merge Stones]]

Pattern:

```text
dp[l][r]
```

means:

> answer for interval `[l,r]`.

---

# 34. Tree DP

* [[House Robber III]]
* [[Tree Diameter DP]]
* [[Maximum Independent Set Tree]]
* [[Subtree DP]]
* [[Rerooting DP]]

---

# 35. Bitmask DP

* [[Bitmask DP]]
* [[State Compression]]
* [[Traveling Salesman DP]]
* [[Subset DP]]
* [[Assignment DP]]

Use when:

```text
n is small
AND
state depends on selected/unselected elements
```

Typical:

```text
n ≤ 20
```

---

# 36. DP Recognition Framework

Whenever you see an optimization problem, ask:

```text
1. Can I divide the problem into states?

2. Does the same state appear repeatedly?

3. What information defines a state?

4. What choices can I make?

5. What is the transition?

6. What is the base case?

7. Can I memoize?

8. Can I convert to tabulation?

9. Can I optimize memory?
```

---

# 37. 🧠 Bit Manipulation

## Basics

* [[Binary Number System]]
* [[Bitwise AND]]
* [[Bitwise OR]]
* [[Bitwise XOR]]
* [[Bitwise NOT]]
* [[Left Shift]]
* [[Right Shift]]

## Important Tricks

* [[Check Odd Even]]
* [[Check Power of Two]]
* [[Set Bit]]
* [[Clear Bit]]
* [[Toggle Bit]]
* [[Count Set Bits]]
* [[Lowest Set Bit]]
* [[XOR Properties]]
* [[Swap Using XOR]]

## Advanced

* [[Bitmask]]
* [[Subsets Using Bitmask]]
* [[Bitmask DP]]
* [[XOR Trie]]
* [[XOR Basis]]

---

# 38. 📊 Advanced Array Patterns

## Difference Array

* [[Difference Array]]
* [[Range Increment]]
* [[Range Update]]

## Kadane

* [[Kadane Algorithm]]
* [[Maximum Subarray]]
* [[Circular Maximum Subarray]]

## Prefix + Hashing

* [[Subarray Sum K]]
* [[Longest Subarray Sum K]]
* [[Equal 0 and 1]]

## XOR

* [[Subarray XOR]]
* [[XOR Prefix]]
* [[Single Number]]
* [[Missing Number]]

---

# 39. 📦 Monotonic Structures

## Monotonic Stack

* [[Next Greater Element]]
* [[Previous Greater Element]]
* [[Next Smaller Element]]
* [[Largest Rectangle]]
* [[Stock Span]]
* [[Daily Temperatures]]

## Monotonic Queue

* [[Sliding Window Maximum]]
* [[Sliding Window Minimum]]

Recognition:

> Need the nearest greater/smaller element or maintain min/max over a moving range.

---

# 40. 🔢 Ordered Data Structures

* [[TreeSet]]
* [[TreeMap]]
* [[Ordered Set]]
* [[Ordered Map]]
* [[Ceiling]]
* [[Floor]]
* [[Lower Bound]]
* [[Upper Bound]]

Applications:

* [[Dynamic Ordering]]
* [[Range Queries]]
* [[Predecessor Successor]]
* [[Interval Queries]]

---

# 41. 🌳 Segment Tree

Very important for advanced competitive programming.

## Fundamentals

* [[Segment Tree]]
* [[Build Segment Tree]]
* [[Point Update]]
* [[Range Query]]
* [[Range Update]]

## Query Types

* [[Range Sum Query]]
* [[Range Minimum Query]]
* [[Range Maximum Query]]
* [[Range GCD Query]]
* [[Range XOR Query]]

## Advanced

* [[Lazy Propagation]]
* [[Lazy Segment Tree]]
* [[Segment Tree Beats]]

## Recognition

Look for:

```text
n ≥ 10^5

many queries

range query

updates between queries
```

Example:

```text
Update index i
Query [l,r]
Update index j
Query [x,y]
...
```

Think:

> **Segment Tree / Fenwick Tree**

---

# 42. 🌲 Fenwick Tree

Also called:

* [[Binary Indexed Tree]]
* [[Fenwick Tree]]

Topics:

* [[Point Update]]
* [[Prefix Sum Query]]
* [[Range Sum]]
* [[Coordinate Compression]]
* [[Inversion Count]]

Recognition:

> Dynamic prefix/range sums with updates.

---

# 43. 🧮 Sparse Table

* [[Sparse Table]]
* [[Range Minimum Query]]
* [[Idempotent Queries]]
* [[Binary Lifting Connection]]

Recognition:

> Many static range queries + no updates.

---

# 44. 🧭 Advanced Graph Algorithms

## Strongly Connected Components

* [[SCC]]
* [[Kosaraju Algorithm]]
* [[Tarjan Algorithm]]

## Bridges

* [[Bridge]]
* [[Tarjan Bridge Algorithm]]

## Articulation Points

* [[Articulation Point]]
* [[Cut Vertex]]

## Biconnected Components

* [[Biconnected Components]]

---

# 45. 🌊 Network Flow

Advanced competitive programming topic.

* [[Max Flow]]
* [[Min Cut]]
* [[Ford Fulkerson]]
* [[Edmonds Karp]]
* [[Dinic Algorithm]]
* [[Bipartite Matching]]
* [[Flow Network]]

---

# 46. 🔀 Bipartite Graph

* [[Bipartite Graph]]
* [[Bipartite BFS]]
* [[Bipartite DFS]]
* [[2 Coloring]]
* [[Bipartite Matching]]

Recognition:

> Divide nodes into two groups such that connected nodes belong to opposite groups.

---

# 47. 🎯 Advanced Searching

* [[Ternary Search]]
* [[Meet in the Middle]]
* [[Coordinate Compression]]
* [[Parallel Binary Search]]
* [[Parametric Search]]

---

# 48. 🧩 Meet in the Middle

Use when:

```text
n ≈ 40
```

and brute force:

```text
2^40
```

is too large.

Split:

```text
n/2 + n/2
```

Then solve each half.

Applications:

* [[Subset Sum Meet in Middle]]
* [[Closest Subset Sum]]
* [[Bitmask Optimization]]

---

# 49. 🧠 Divide and Conquer

* [[Divide and Conquer]]
* [[Merge Sort]]
* [[Quick Sort]]
* [[Binary Search]]
* [[Closest Pair]]
* [[Count Inversions]]
* [[Divide and Conquer DP]]

---

# 50. 🔢 String Algorithms

## Basic

* [[String Hashing]]
* [[Rolling Hash]]
* [[String Matching]]

## Advanced

* [[KMP]]
* [[Z Algorithm]]
* [[Rabin Karp]]
* [[Manacher Algorithm]]
* [[Suffix Array]]
* [[Suffix Automaton]]
* [[Aho Corasick]]

## Recognition

### KMP

Pattern matching with repeated prefixes.

### Rolling Hash

Fast substring comparison.

### Manacher

Longest palindromic substring.

### Aho-Corasick

Multiple pattern matching.

---

# 51. 🧬 Advanced DP

* [[Digit DP]]
* [[Probability DP]]
* [[Expected Value DP]]
* [[Game DP]]
* [[DP on DAG]]
* [[Profile DP]]
* [[Bitmask DP]]
* [[Tree DP]]
* [[Interval DP]]
* [[SOS DP]]
* [[Convex Hull Trick DP]]
* [[Divide and Conquer Optimization]]
* [[Knuth Optimization]]

---

# 52. 🎮 Game Theory

* [[Game Theory]]
* [[Winning State]]
* [[Losing State]]
* [[Nim Game]]
* [[Sprague Grundy]]
* [[Grundy Number]]
* [[Minimax]]
* [[Alpha Beta Pruning]]

---

# 53. 🧠 Computational Geometry

Advanced but useful for competitive programming.

* [[Point Geometry]]
* [[Distance Between Points]]
* [[Orientation]]
* [[Cross Product]]
* [[Line Intersection]]
* [[Segment Intersection]]
* [[Convex Hull]]
* [[Sweep Line]]
* [[Closest Pair of Points]]
* [[Polygon Area]]
* [[Point in Polygon]]

---

# 54. 🎯 Problem-Solving Patterns Master List

This is the most important section for your goal.

## Pattern 1 — Frequency Map

```text
Question:
How often does something occur?

Think:
HashMap / array frequency
```

---

## Pattern 2 — Hash Lookup

```text
Need fast existence/search?

Think:
HashSet / HashMap
```

---

## Pattern 3 — Two Sum / Complement

```text
Need x + y = target?

Store:
target - x
```

---

## Pattern 4 — Two Pointers

```text
Sorted array
Pair
Palindrome
Remove duplicates
Partition
```

---

## Pattern 5 — Sliding Window

```text
Continuous subarray/substring
Longest/shortest
At most K
Distinct count
```

---

## Pattern 6 — Prefix Sum

```text
Repeated range sum
Subarray sum
Range query
```

---

## Pattern 7 — Prefix Sum + HashMap

```text
Subarray sum = K
Longest subarray satisfying sum condition
```

---

## Pattern 8 — Binary Search

```text
Sorted
Monotonic
Minimum/maximum feasible answer
```

---

## Pattern 9 — Sort + Scan

```text
Intervals
Greedy
Duplicates
Closest values
Pairing
```

---

## Pattern 10 — Monotonic Stack

```text
Nearest greater/smaller
Histogram
Temperature
Stock span
```

---

## Pattern 11 — Heap

```text
Top K
Kth largest/smallest
Repeated minimum/maximum
Streaming median
```

---

## Pattern 12 — BFS

```text
Shortest path in unweighted graph
Level order
Minimum number of moves
Multi-source expansion
```

---

## Pattern 13 — DFS

```text
Explore
Components
Backtracking
Tree traversal
Graph traversal
```

---

## Pattern 14 — Multi-Source BFS

```text
Several starting points
Spread simultaneously
Minimum distance from nearest source
```

Examples:

* [[Rotting Oranges]]
* [[01 Matrix]]
* [[Walls and Gates]]

---

## Pattern 15 — Topological Sort

```text
Dependency
Prerequisite
Ordering
DAG
```

---

## Pattern 16 — Union Find

```text
Connectivity
Components
Dynamic connections
Cycle detection
```

---

## Pattern 17 — Greedy

```text
Local choice
Optimal global answer
Sort + choose
```

---

## Pattern 18 — Backtracking

```text
Generate all possibilities
n small
Choose → Explore → Undo
```

---

## Pattern 19 — Dynamic Programming

```text
Repeated states
Optimization
Count ways
Minimum/maximum
Choose/not choose
```

---

## Pattern 20 — Tree DFS

```text
Answer depends on subtrees
```

---

## Pattern 21 — Tree BFS

```text
Level
Distance
Minimum depth
View
```

---

## Pattern 22 — Binary Search on Answer

```text
Find minimum/maximum X
Check(X) is monotonic
```

---

## Pattern 23 — Difference Array

```text
Many range updates
Few final queries
```

---

## Pattern 24 — Coordinate Compression

```text
Huge values
Only relative ordering matters
```

---

## Pattern 25 — Segment Tree

```text
Many range queries
AND
Updates
```

---

## Pattern 26 — Fenwick Tree

```text
Dynamic prefix/range sums
```

---

## Pattern 27 — Trie

```text
Prefix
Dictionary
String search
Autocomplete
```

---

## Pattern 28 — Bitmask

```text
Small n
Subset selection
```

---

## Pattern 29 — Meet in the Middle

```text
n ≈ 40
2^n too large
```

---

## Pattern 30 — Sweep Line

```text
Intervals
Events
Geometric ranges
```

---

# 55. 🧠 The Ultimate Pattern Recognition Framework

For **every new problem**, force yourself to ask these questions.

```text
STEP 1
What is the input size?

STEP 2
What is the expected complexity?

STEP 3
Is the data sorted?

STEP 4
Is the problem asking about:
    - subarray?
    - substring?
    - subsequence?
    - subset?
    - pair?
    - interval?
    - path?
    - tree?
    - graph?

STEP 5
Is it asking:
    - minimum?
    - maximum?
    - count?
    - existence?
    - shortest?
    - longest?
    - all possibilities?

STEP 6
Can hashing solve it?

STEP 7
Can two pointers solve it?

STEP 8
Can sliding window solve it?

STEP 9
Can prefix sum solve it?

STEP 10
Can sorting simplify it?

STEP 11
Is there monotonicity?
    → Binary Search

STEP 12
Is there nearest greater/smaller?
    → Monotonic Stack

STEP 13
Is there top K?
    → Heap

STEP 14
Is there connectivity?
    → DFS/BFS/DSU

STEP 15
Is there dependency?
    → Topological Sort

STEP 16
Is there shortest path?
    → BFS/Dijkstra/etc.

STEP 17
Is there repeated state?
    → DP

STEP 18
Does the problem require all possibilities?
    → Backtracking

STEP 19
Are there range queries + updates?
    → Segment Tree/Fenwick

STEP 20
Is n small?
    → Bitmask / Backtracking / Exponential DP
```

---

# 56. ⚡ Pattern Recognition Cheat Sheet

| Problem Clue             | First Pattern to Think               |
| ------------------------ | ------------------------------------ |
| Pair sum                 | [[Two Pointers]] / [[HashMap]]       |
| Sorted array             | [[Binary Search]] / [[Two Pointers]] |
| Longest substring        | [[Sliding Window]]                   |
| Shortest substring       | [[Sliding Window]]                   |
| Subarray sum             | [[Prefix Sum]]                       |
| Subarray sum K           | [[Prefix Sum + HashMap]]             |
| Next greater             | [[Monotonic Stack]]                  |
| Top K                    | [[Heap]]                             |
| Kth largest              | [[Heap]] / [[Quickselect]]           |
| Minimum/maximum feasible | [[Binary Search on Answer]]          |
| Intervals                | [[Sort + Greedy]]                    |
| Dependencies             | [[Topological Sort]]                 |
| Shortest unweighted path | [[BFS]]                              |
| Shortest weighted path   | [[Dijkstra]]                         |
| Connectivity             | [[DFS/BFS/DSU]]                      |
| Number of islands        | [[DFS/BFS]]                          |
| Generate all             | [[Backtracking]]                     |
| Choose/not choose        | [[DP]] / [[Backtracking]]            |
| Repeated subproblems     | [[Dynamic Programming]]              |
| Prefix matching          | [[Trie]]                             |
| Range query + updates    | [[Segment Tree]]                     |
| Dynamic prefix sum       | [[Fenwick Tree]]                     |
| Static range minimum     | [[Sparse Table]]                     |
| Small n ≤ 20             | [[Bitmask]]                          |
| n ≈ 40                   | [[Meet in the Middle]]               |
| Tree path                | [[Tree DFS]]                         |
| Tree levels              | [[Tree BFS]]                         |
| BST kth smallest         | [[Inorder Traversal]]                |
| Cycle undirected         | [[DFS]] / [[DSU]]                    |
| Cycle directed           | [[Topological Sort]] / [[DFS]]       |
| 0/1 weights              | [[0-1 BFS]]                          |
| All pairs shortest path  | [[Floyd Warshall]]                   |
| Negative edges           | [[Bellman Ford]]                     |
| Minimum connection cost  | [[MST]]                              |
| Nearest greater/smaller  | [[Monotonic Stack]]                  |
| Range modifications      | [[Difference Array]]                 |

---

# 57. 🏗️ DSA Template Library

Create a separate Obsidian folder:

```text
DSA/
├── Templates/
├── Patterns/
├── Data Structures/
├── Algorithms/
├── Problems/
└── Revision/
```

Important templates:

* [[Java Fast Input Template]]
* [[Array Template]]
* [[HashMap Template]]
* [[Two Pointer Template]]
* [[Sliding Window Template]]
* [[Prefix Sum Template]]
* [[Binary Search Template]]
* [[Linked List Template]]
* [[Stack Template]]
* [[Monotonic Stack Template]]
* [[Heap Template]]
* [[Tree DFS Template]]
* [[Tree BFS Template]]
* [[Graph DFS Template]]
* [[Graph BFS Template]]
* [[Topological Sort Template]]
* [[Dijkstra Template]]
* [[DSU Template]]
* [[Backtracking Template]]
* [[1D DP Template]]
* [[2D DP Template]]
* [[Knapsack Template]]
* [[Trie Template]]
* [[Fenwick Tree Template]]
* [[Segment Tree Template]]
* [[Bitmask Template]]

---

# 58. 🧪 Problem Classification System

Every problem you solve should be classified.

Use:

```text
Problem
↓
Data Structure
↓
Pattern
↓
Technique
↓
Complexity
↓
Template
↓
Variation
```

Example:

```text
Longest Substring Without Repeating Characters

Data Structure:
HashSet

Pattern:
Sliding Window

Technique:
Two Pointers

Complexity:
O(n)

Template:
Variable Sliding Window
```

Another:

```text
Course Schedule

Data Structure:
Graph

Pattern:
Topological Sort

Technique:
Kahn Algorithm

Complexity:
O(V + E)
```

---

# 59. 📈 Difficulty Progression

## Level 0 — Fundamentals

* [[Arrays]]
* [[Strings]]
* [[Hashing]]
* [[Complexity]]

Target:

```text
50–100 problems
```

---

## Level 1 — Core Patterns

* [[Two Pointers]]
* [[Sliding Window]]
* [[Prefix Sum]]
* [[Binary Search]]
* [[Stack]]
* [[Queue]]

Target:

```text
100–150 problems
```

---

## Level 2 — Core Data Structures

* [[Linked List]]
* [[Trees]]
* [[BST]]
* [[Heap]]
* [[Trie]]
* [[Graphs]]

Target:

```text
150–200 problems
```

---

## Level 3 — Advanced Patterns

* [[Greedy]]
* [[Backtracking]]
* [[Dynamic Programming]]
* [[DSU]]
* [[Shortest Path]]
* [[Topological Sort]]

Target:

```text
150–200 problems
```

---

## Level 4 — Advanced Competitive Programming

* [[Segment Tree]]
* [[Fenwick Tree]]
* [[SCC]]
* [[Bridges]]
* [[Articulation Points]]
* [[Network Flow]]
* [[String Algorithms]]
* [[Bitmask DP]]
* [[Digit DP]]
* [[Game Theory]]
* [[Computational Geometry]]

Target:

```text
100+ problems
```

---

# 60. 🔥 Problem-Solving Training Method

Do NOT solve problems randomly.

For every pattern:

```text
1. Learn concept
2. Learn recognition clues
3. Learn template
4. Solve easy problem
5. Solve medium problem
6. Solve variation
7. Solve without template
8. Solve timed
9. Solve unseen problem
10. Explain solution
```

---

# 61. 🧠 The 5-Stage Mastery System

## Stage 1 — Understand

You can explain the algorithm.

## Stage 2 — Implement

You can code it without looking.

## Stage 3 — Recognize

You can identify the pattern from a new problem.

## Stage 4 — Adapt

You can modify the template for a variation.

## Stage 5 — Invent

You can combine multiple patterns.

Example:

```text
Sliding Window
+
HashMap
+
Prefix Sum
```

or:

```text
Binary Search
+
Greedy
```

or:

```text
DFS
+
Memoization
=
Tree/Graph DP
```

---

# 62. ⏱️ Timed Problem Training

Your ultimate goal should not literally be "solve every problem in a fraction of a second."

Instead train your **pattern recognition speed**.

### Target

```text
10 seconds
→ identify problem family

30 seconds
→ identify candidate pattern

1–2 minutes
→ derive approach

5–10 minutes
→ implement

5 minutes
→ test edge cases
```

Eventually:

```text
Question
↓
Pattern instantly recognized
↓
Known template
↓
Adapt
↓
Code
```

---

# 63. 🧠 Daily Pattern Training

For every study session:

### Round 1 — Recognition

Take 10 problems.

Do NOT solve them.

For each write only:

```text
Pattern:
Data Structure:
Expected Complexity:
```

Target:

```text
< 30 seconds/problem
```

---

### Round 2 — Implementation

Take 3 problems.

Solve from scratch.

---

### Round 3 — Variation

Take one known pattern and solve a different variation.

---

### Round 4 — Recall

Close all notes.

Write the template from memory.

---

### Round 5 — Explanation

Explain:

```text
Why this pattern?
Why not brute force?
Complexity?
Edge cases?
```

---

# 64. 🏆 Problem Count Target

A strong preparation should focus on **patterns rather than raw problem count**.

Suggested target:

```text
Easy:
150+

Medium:
300+

Hard:
100+

Total:
550+
```

But more important:

```text
100 patterns/variations mastered
>
1000 memorized solutions
```

---

# 65. 🎯 Placement Priority

If your immediate objective is placements, prioritize:

## Tier 1 — MUST MASTER

* [[Arrays]]
* [[Strings]]
* [[Hashing]]
* [[Two Pointers]]
* [[Sliding Window]]
* [[Prefix Sum]]
* [[Binary Search]]
* [[Stack]]
* [[Queue]]
* [[Linked List]]
* [[Trees]]
* [[BST]]
* [[Heap]]
* [[Graphs]]
* [[BFS]]
* [[DFS]]
* [[Topological Sort]]
* [[Greedy]]
* [[Backtracking]]
* [[Dynamic Programming]]

---

## Tier 2 — VERY IMPORTANT

* [[Trie]]
* [[DSU]]
* [[Dijkstra]]
* [[MST]]
* [[Monotonic Stack]]
* [[Fenwick Tree]]
* [[Segment Tree]]
* [[Bit Manipulation]]
* [[Intervals]]
* [[Matrix Problems]]

---

## Tier 3 — ADVANCED

* [[SCC]]
* [[Bridges]]
* [[Articulation Points]]
* [[Network Flow]]
* [[String Algorithms]]
* [[Digit DP]]
* [[Bitmask DP]]
* [[Game Theory]]
* [[Computational Geometry]]

---

# 66. 🧠 The Ultimate DSA Mental Model

When a problem arrives, don't immediately code.

Think:

```text
                    PROBLEM
                       │
                       ▼
                 CONSTRAINTS
                       │
                       ▼
                DATA STRUCTURE
                       │
                       ▼
                    PATTERN
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
       SEARCH        OPTIMIZE      COUNT
          │            │            │
          ▼            ▼            ▼
     Binary Search     DP         Hashing
     BFS/DFS            Greedy     Prefix
                       │
                       ▼
                    TEMPLATE
                       │
                       ▼
                   OPTIMIZE
                       │
                       ▼
                  EDGE CASES
                       │
                       ▼
                    SOLUTION
```

---

# 67. 🔥 The 20 Patterns You Must Know Cold

If you want product-company-level problem solving, these should become automatic:

1. [[Hashing]]
2. [[Two Pointers]]
3. [[Sliding Window]]
4. [[Prefix Sum]]
5. [[Binary Search]]
6. [[Sorting + Greedy]]
7. [[Intervals]]
8. [[Monotonic Stack]]
9. [[Heap / Top K]]
10. [[Linked List Fast Slow]]
11. [[Tree DFS]]
12. [[Tree BFS]]
13. [[Graph DFS/BFS]]
14. [[Topological Sort]]
15. [[Union Find]]
16. [[Backtracking]]
17. [[Dynamic Programming]]
18. [[Shortest Path]]
19. [[Bit Manipulation]]
20. [[Range Query Data Structures]]

---

# 68. 📝 Obsidian Problem Note Template

For every problem create:

````markdown
---
title:
platform:
difficulty:
pattern:
data_structure:
time_complexity:
space_complexity:
status:
---

# Problem

## Pattern

[[Pattern Name]]

## Why This Pattern?

-

## Brute Force

-

## Optimal Approach

-

## Key Observation

-

## Algorithm

1.
2.
3.
4.

## Template

```java

````

## Complexity

Time:
Space:

## Edge Cases

*

## Mistake I Made

*

## New Learning

*

## Similar Problems

* [[]]
* [[]]
* [[]]

## Pattern Variations

* [[]]
* [[]]

````

---

# 69. 🔁 Revision System

Use three revision categories.

## R1 — Forgot

You cannot solve without seeing the solution.

## R2 — Recognized but Slow

You know the pattern but implementation is slow.

## R3 — Mastered

You recognize and implement quickly.

Every problem should eventually move:

```text
R1 → R2 → R3
````

---

# 70. 🏁 Final Mastery Checklist

## Foundations

* [ ] [[Big O]]
* [ ] [[Arrays]]
* [ ] [[Strings]]
* [ ] [[Hashing]]
* [ ] [[Recursion]]

## Linear Structures

* [ ] [[Linked List]]
* [ ] [[Stack]]
* [ ] [[Queue]]
* [ ] [[Deque]]

## Searching / Sorting

* [ ] [[Binary Search]]
* [ ] [[Merge Sort]]
* [ ] [[Quick Sort]]
* [ ] [[Counting Sort]]

## Core Patterns

* [ ] [[Two Pointers]]
* [ ] [[Sliding Window]]
* [ ] [[Prefix Sum]]
* [ ] [[Difference Array]]
* [ ] [[Monotonic Stack]]
* [ ] [[Heap]]
* [ ] [[Intervals]]

## Trees

* [ ] [[Binary Tree]]
* [ ] [[Tree Traversal]]
* [ ] [[BST]]
* [ ] [[LCA]]
* [ ] [[Tree DP]]

## Graphs

* [ ] [[DFS]]
* [ ] [[BFS]]
* [ ] [[Connected Components]]
* [ ] [[Cycle Detection]]
* [ ] [[Topological Sort]]
* [ ] [[Shortest Path]]
* [ ] [[Dijkstra]]
* [ ] [[DSU]]
* [ ] [[MST]]
* [ ] [[SCC]]

## Advanced

* [ ] [[Trie]]
* [ ] [[Fenwick Tree]]
* [ ] [[Segment Tree]]
* [ ] [[Sparse Table]]
* [ ] [[Bitmask]]
* [ ] [[Bitmask DP]]
* [ ] [[Digit DP]]
* [ ] [[String Algorithms]]
* [ ] [[Network Flow]]

## DP

* [ ] [[1D DP]]
* [ ] [[Grid DP]]
* [ ] [[Knapsack DP]]
* [ ] [[Subsequence DP]]
* [ ] [[Interval DP]]
* [ ] [[Tree DP]]
* [ ] [[Bitmask DP]]

---

# 71. 🥇 Final Objective

The objective is NOT:

```text
"I solved 500 LeetCode problems."
```

The objective is:

```text
I see a new problem.

↓ 5–10 seconds

I identify the problem family.

↓ 20–30 seconds

I identify the pattern.

↓ 30–60 seconds

I derive the state/transition or algorithm.

↓ 1–2 minutes

I choose the correct template.

↓ 

I implement.

↓ 

I test edge cases.

↓ 

I optimize.
```

The final skill is:

> **Pattern Recognition + Algorithmic Thinking + Template Recall + Adaptation**

That is what turns DSA preparation into actual problem-solving ability.
