---
title: Programming Assignments
...

All programming assignments will be posted here as they are released.

# Instructions

Programming assignments are typically due on Thursdays (see the course schedule for exceptions). With the exception of ps0, all programming assignments may be completed in either Java or Python3 (your choice).

# Policies

You may collaborate with up to 2 other people (i.e. a group of up to 3 total) when completing programming assignments, but your collaboration must be [Whiteboard Only](/syllabus.html) You may additionally use external materials with following restrictions:

- You must understand everything you submit. Do not submit anything you could not explain to a member of the course staff.
- You **must** cite any and every source you consult beyond officially-provided materials (see list above). Included in your citation, you must identify which components of your submission came from each source (it will be understood that content with no citation is your own exclusive work). Your collaborators are considered to be sources, and so should be cited. An example citation might look like: "I collaborated with David Evans on the pdf style, I consulted \url{https://www.overleaf.com/learn/latex/Aligning\%20equations\%20with\%20amsmath} for help with the align environment, Robbie Hott helped me to debug the for loop on line 107 of my code."
- Do not seek "hints" or entire solutions to the problems. Limit your searching to background information only.

# Deliverables

Unless otherwise indicated, each program (either a .py file or a .java file) will be submitted in Gradescope. 

# Assignments

## PA0: Getting Started

Due 11:59pm Thursday Jan 26 (but will remain open for submission until Thursday Feb 2).

This assignment is intended to get you set up for future written and programming assignments. Here is a link to the [PA0 Task Description](https://www.cs.virginia.edu/~njb2b/cs3100/s2023/pa0.html).

Unlike with all future PAs, you may work and submit as a group of up to 5 on this assignment.

## PA1: Kidney Donation

Due 11:59pm Thursday Feb 9.

This assignment is intended to provide you experience in building/manipulating adjacency list representations of graphs, and to reinforce your understanding of BFS and DFS by adapting them to solve a novel problem. Here is a link to the [PA1 Task Description](/files/pa/pa1_writeup.pdf). Here is a [zip file](/files/pa/KidneyDonation.zip) with some starter code (in python and java both) and test cases. Modify the `DonorCycle.java` or `donor_cycle.py` file (you don't need to do both!) to solve the problem described in the writeup. To submit, simplyt upload your `DonorCycle.java` or `donorcycle.py` file to gradescope.

Here is a summary of the test cases provided:

- `example.txt` is the example file in the writeup. The answer should be **True**.
- `slides.txt` is the directed graph from the slides with the right-most node as the query. The answer should be **False**.
- `straightline.txt` is just a line of vertices. The answer should be **False**.
- `biggerloop.txt` is 10 vertices in a circle. The answer should be **True**.
- `almostcycle.txt` is 10 vertices in a cycle, but with one edge in the opposite direction from the rest. The answer should be **False**.
- `complete.txt` is 10 vertices that are each connected to all the other vertices. The answer should be **True**.
- `lollypop0.txt` is a graph with vertices in a "lollypop" shape, meaning there is a straight line of nodes connected to nodes in a loop. The query node is at the start of the "stick" of the lollypop, so the answer should be **False**.
- `lollypop5.txt` is the same lollypop graph as above, but now the query node is in the candy portion of the lollypop. The answer should be **True**.

To give input to your program, you should just run the program. At first nothing will appear to happen, but then if you copy-paste the contents of a file into the console (the place that things print to in your IDE) and hit "enter" the code should run. The starter code parses the input for you and invokes a function using those parameters. To provide output, simply print to the console. Make sure you do not have any print statements besides just your answer.

There will be additional tests run when you submit that you will not have direct access to, so make sure you do some debugging on your own, too!

## PA2: Amazon Subprime

Due 11:59pm Thursday Feb 16.

This assignment is intended to provide you experience in building/manipulating adjacency list representations of weighted graphs, and to reinforce your understanding of Dijkstra's algorithm by adapting it to solve a novel problem. Here is a link to the [PA2 Task Description](/files/pa/pa2_writeup.pdf). Here is a [zip file](/files/pa/AmazonSubprime.zip) with some starter code (in python and java both) and test cases. Modify the `Subprime.java` or `subprime.py` file (you don't need to do both!) to solve the problem described in the writeup. To submit, simplyt upload your `Subprime.java` or `subprime.py` file to gradescope. Sample implementations of Dijkstra's algorithm is also provided for both Java and Python. You're welcome to use that code however you wish, but your program will not have access to those files when being autograded, so any code you use should be copy-pasted into the program you submit.

There are two test cases provided:

- `test0.txt` is the test from the writeup. Its shortest path should be 0,2,3 and have cost 120
- `test1.txt` is a larger graph. Its shortest path should be 0,4,5,6,7,3 and have cost 70

To give input to your program, you should just run the program. At first nothing will appear to happen, but then if you copy-paste the contents of a file into the console (the place that things print to in your IDE) and hit "enter" the code should run. The starter code parses the input for you and invokes a function using those parameters. To provide output, simply print to the console. Make sure you do not have any print statements besides just your answer.

There will be additional tests run when you submit that you will not have direct access to (in fact the majority are hidden for this assignment), so make sure you do some debugging on your own, too!

## PA3: Depth Finder

Due 11:59pm Thursday Feb 23. 

This assignment is intended to provide you experience in designing and implementing divide and conquer algorithms. Here is a link to the [PA3 Task Description](/files/pa/pa3_writeup.pdf). Here is a [zip file](/files/pa/DepthFinder.zip) with some starter code (in python and java both). Modify  the `GamePlayer.java` or `gameplayer.py` file (you don't need to do both!) to solve the problem described in the writeup. To submit, simply upload your `GamePlayer.java` or `gameplayer.py` file to gradescope. Do not submit the other files (the autograder will be using a different version of each to ensure rules are followed).

There are no pre-defined tests for this assignment. Instead, tests are generated randomly each time. To run your code, run the `PlayGame.java` or `playgame.py` program, then give an integer greater than 4 in the console to identify the size of the test to run. Since the tests are random it would be wise to run your code several times for many different input sizes before concluding that it is correct.

To truly test your program, in addition to the random tests of various sizes, the autograder will run your program against a gameboard that "cheats". This adversarial gameboard will derives answers answers per-ping to guarantee that it will cause your algorithm to exceed the ping limit if any input can. The autograder tests marked "random" use the same implementation given to you in the starter code. The tests marked "adversary" use the cheating implementation.

## PA4: Median Finder

Due 11:59pm Thursday March 2. 

This assignment is intended to provide you experience in designing and implementing divide and conquer algorithms. Here is a link to the [PA4 Task Description](/files/pa/pa4_writeup.pdf). Here is a [zip file](/files/pa/pa4.zip) with some starter code (in python and java both). Modify  the `MedianFinder.java` or `medianfinder.py` file (you don't need to do both!) to solve the problem described in the writeup. To submit, simply upload your `MedianFinder.java` or `medianfinder.py` file to gradescope. Do not submit the other files (the autograder will be using a different version of each to ensure rules are followed).

## PA5: Greedy Choices


This assignment is intended to provide you experience in designing and implementing greedy choice functions. Here is a link to the [PA5 Task Description](/files/pa/pa5_writeup.pdf). Here is a [zip file](/files/pa/pa5.zip) with some starter code (in python and java both). You will be writings three different greedy choice functions (the choice functions only, I do the rest of the algorithm for you). One test case per greedy choice is provided just so you can see input format. You will need to build confidence for yourself on the correctness of your function, because no autograder feedback will be provided for you except to indicate whether or not there was an error when running your code.

## PA6: Clustering

This assignment is intended to provide you experience in implementing and applying Minimum Spanning Tree algorithms. Here is a link to the [PA6 Task Description](/files/pa/pa6_writeup.pdf). Here is a [zip file](/files/pa/pa6.zip) with some starter code (in python and java both). The test cases provided are simply random 2-d arrays of distances. No particular corner cases, edge cases, or misconceptions are intentionally tested for. You score should be visible immediately after the autograder checks your code.

## PA7: Birthday Prank

This assignment is intended to provide you experience in implementing Dynamic Programming algorithms. Here is a link to the [PA7 Task Description](/files/pa/pa7_writeup.pdf). Here is a [zip file](/files/pa/pa7.zip) with some starter code (in python and java both). Most test cases were designed to have cases were there are many options of boxes that nest but are not part of an optimal solution. There are also test cases where nearly every box should be included and one case where no two boxes fit teogher. You score should be visible immediately after the autograder checks your code, there are no hidden tests

## PA8: Drainage

This assignment is intended to provide you experience in implementing Dynamic Programming algorithms with backtracking. Here is a link to the [PA8 Task Description](/files/pa/pa8_writeup.pdf). Here is a [zip file](/files/pa/pa8.zip) with some starter code (in python and java both). Your score should be visible immediately after the autograder checks your code, there are no hidden tests

