---
title: Quizzes
...



# Goals

Quizzes are designed to assess your understanding of course concepts and your fluency with the vocabulary introduced. Ideally you will have learned all content necessary to successfully complete each quiz through a combination of lecture and your effort on related homeworks (programming and written).

# Collaboration

You must complete quizzes entirely on your own, do not discuss the contents of a quiz with anyone outside the course staff prior to its deadline. You may use only officially-provided or personally-created materials when completing at-home quizzes. This means you may only use:

- The course textbook
- Anything on the course webpage or directly linked to from the course webpage
- Your personal notes (or those of a note-taker if you receive them as accommodation)
- Your past assignment submissions
- Lecture recordings

You will be asked to pledge on each quiz that you've observed these directives.

# Deliverables

Quizzes will be delivered and submitted on Gradescope. You will have 60 minutes from the time that you first open the quiz to complete the quiz. This includes the time required to scan/photograph and upload any hand-written work, so familiarize yourself with the tool you will use to do this before beginning the quiz.

# Quiz Guides

## Quiz 1: Graphs and Asymptotics

This quiz will be based off of all content convered through our discussion of Dijkstra's Algorithm (which we concluded on Feb 6). This Quiz will be released during the evening of Thursday 2/23 and due at 11:59pm on Tuesday 2/28. The Quiz will consist of multiple choice questions and written questions. You should solve the written questions on your own paper, then scan/photograph and upload your solutions to gradescope. Your 60 minutes includes the time to do this, so please have a plan before you begin the quiz.

Here is what you'll be expected to do on the quiz:

- Intuitively understand the definitions of $O$, $\Omega$, $\Theta$, $o$, $\omega$ and how they relate to evaluating the running time of algorithms
- Be able to demonstrate asymptotic bounds of functions
- Understand the definition of a graph and definitions of various properties of graphs including:
    - Directed Graph
    - Undirected Graph
    - Weighted Graph
    - Node degree (including in-degree and out-degree)
    - Path
    - Cycle
    - Simple Path
    - Connected Graph
    - Cyclic Graph
    - Topological sort
    - Strongly Connected Component
    - Bipartite
- Be able to reason about the tradeoffs between using an adjacency list representation of a graph vs. an adjacency matrix representation
- Understand the following algorithms/traversals to the extent that you could step through them manually and reason about hypothetical changes to them:
  - Breadth-First Search (BFS)
  - Depth-First Search (DFS)
  - Dijkstra's Algorithm

Here are some vague hypothetical questions that could be asked and additionally some actual questions that I discarded from the quiz to keep it of appropriate length:

- Show that $f(n)\in O(g(n))$
- If $f(n)$ and $g(n)$ represent the worst case running time of two different algorithms, what does $f(n)\in \Omega(g(n))$ tell us about how many operations they'll do for large inputs?
- Suppose we did a DFS on the given graph starting from node $0$, what type of edge is $(3,4)$? Is it a tree edge, back edge, forward edge, or cross edge?
- Is it possible to run DFS on an acyclic graph and find cross edges? If so, then give and example graph and start node. If not, argue why.
- Suppose we did a BFS on the given graph starting from node $5$, which node would be the last one removed from the queue?
- Suppose we had a graph were all edge weights were positive and unique. Could our implementation of Dijkstra's algorithm from class ever add the same node to the priority queue twice?
- Suppose we had a graph with $n$ nodes and $2$ strongly connected components. What is the maximum number of edges in this graph?
- In our implementation of Dijkstra's algorithm from class, inside the for loop that iterates over all of the neighbors of the current node, we have the conditional `if not done[neighbor]`. Suppose we removed that if statement so that the body of the loop occurred every time for every neighbor. Would the algorithm still be guaranteed to terminate, or could we have an infinite loop?

## Quiz 2: Divide and Conquer

This quiz will be based off of all content convered relating the Divide and Conquer algorithms (which we concluded on Feb 23). The Quiz will consist of multiple choice questions and written questions. You should solve the written questions on your own paper, then scan/photograph and upload your solutions to gradescope. Your 60 minutes includes the time to do this, so please have a plan before you begin the quiz.

Here is what you'll be expected to do on the quiz:

- Reason about the divide and conquer algorithms discussed in class
    - Mergesort
    - Karatsuba
    - Closest Pair of Points
    - Strassen's
- Provide a recurrence relation to express the running time of a divide and conquer algorithm
- Solve recurrence relations using the Master Theorem and the Tree method
- Evaluate the running time of a divide and conquer algorithm running in parallel

## Quiz 3: Greedy

This quiz will be based off of all content convered relating the Divide and Conquer algorithms (which we concluded on March 16). The Quiz will consist of multiple choice questions and written questions. You should solve the written questions on your own paper, then scan/photograph and upload your solutions to gradescope. Your 60 minutes includes the time to do this, so please have a plan before you begin the quiz.

Here is what you may be expected to do on the quiz:

- Know and reason about the definitions and importance of Optimal Substructure and Greedy Choice Functions
- Prove a problem has optimal substructure
- Be able to find counterexamples for potential Greedy Choice Functions
- Know the definition of a Minimum Spanning Tree
- Know the Cut Property of Minimum Spanning Trees
- Know Prim's and Kruskal's algorithms to the extent that you could do them by hand and know the differences between them
- Understand the knapsack problem and why the fractional version allows for a greedy solution whereas the 0/1 version does not

## Quiz 4: Dynamic Programming

This quiz will be based off of all content convered relating to Dynamic Programming algorithms (which we concluded on March 30). The Quiz will consist of multiple choice questions and written questions. You should solve the written questions on your own paper, then scan/photograph and upload your solutions to gradescope. Your 60 minutes includes the time to do this, so please have a plan before you begin the quiz.

Here is what you may be expected to do on the quiz:

- Know and reason about the definitions and importance of Optimal Substructure, memoization, and overlapping subproblems as they relate to dynamic programming
- Explain the differences and similarities between a top-down and bottom-up dynamic programming algorithm
- Use a description of a problems optimal substructure to:
    - Write a dynamic programming algorithm (either top-down or bottom-up)
    - Identify the base case of a dynamic programming algorithm
    - Identify the base case of a dynamic programming algorithm
    - Evaluate the running time of the dynamic programming algorithm
    - Reason about the size/shape of the memory used to store subproblems' solutions
    - Finish filling in an incomplete memory
- Understand the dynamic programming algorithms discussed in class to be able to:
    - Execute them by hand for a small number of steps
    - Fill in cells in the memory
    - Identify what problems might depend on other problems
    - Use a completed memory to do backtracking

## Quiz 5: Reductions

This quiz will be based off of all content convered relating to Max Flow and Reductions (which we concluded on April 13). The Quiz will consist of multiple choice questions and written questions. You should solve the written questions on your own paper, then scan/photograph and upload your solutions to gradescope. Your 60 minutes includes the time to do this, so please have a plan before you begin the quiz.

Here is what you may be expected to do on the quiz:

- Understand the definition of a flow network and the max flow problem
- Be able to convert between a flow network and a residual graph
- Know the definition of and be able to find an augmenting path
- How to evaluate the running time of the Edmonds-Karp Algorithm
- Understand the Ford-Fulkerson algorithm to a sufficient degree to be able to run it by hand.
- Understand the relationship between Max Flow and Min Cut
- Understand and recall details about the reductions presented in class including:
    - Maximum Bipartite Matching to Max Flow
    - Vertex Disjoint Paths to Edge Disjoint Paths
    - Edge Disjoint Paths to Max Flow
    - Closest Pair of Points to Element Uniqueness
- Understand how to use reductions to apply a worst-case-lower-bound from one problem to another
- Understand why reductions demonstrate worst-case-lower-bounds
- Draw and/or reason about decision trees.


# Final Quizzes

During the final exam period there is only one required quiz due (Quiz 5). You may additionally attempt new quizzes to replace the original quizzes from any unit. That is, during the final exam period you may optionally take replacement Quizzes 1-5. For all but one quiz, your grade on a replacement quiz will replace your grade on the original, whether it is better or worse. For up to one replacement quiz we will drop the replacement grade if it is worse than the original.

If you would like feedback on quizzes to decide whether you'd like to do a replacement quiz we will provide your opportunity to do so. The course staff will hold 2 intermediate grading sessions during the final exam period. During each of these sessions we will clear out all quizzes submitted prior to the start of the session. Sessions will be held on May 5 at 4pm and May 7 at 4pm.

As with all other quizzes, the quizzes will be delivered remotely on gradescope. They will be released throughout the day on May 3 and due at 11:59pm on May 9. You may start them at any time in this window, but you have a 60 minute time window to complete each quiz. In case you wanted to view a quiz before deciding to submit it, we will only consider a quiz "taken" if you upload an image for your written problems. 

The difficulty level and content coverage of each replacement quiz will match that of the original quizzes as closely as possible. Please keep in mind, though, that it is not possible to do this perfectly, and opinions will vary, so you may find some quizzes to be somewhat easier or harder than the original.




