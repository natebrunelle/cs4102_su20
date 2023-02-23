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
- Suppose we had a graph with $n$ nodes and $m$ strongly connected components. What is the maximum number of edges in this graph?
- In our implementation of Dijkstra's algorithm from class, inside the for loop that iterates over all of the neighbors of the current node, we have the conditional `if not done[neighbor]`. Suppose we removed that if statement so that the body of the loop occurred every time for every neighbor. Would the algorithm still be guaranteed to terminate, or could we have an infinite loop?

