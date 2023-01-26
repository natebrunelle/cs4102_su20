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

Due 11:59pm Thursday Feb 2. <span style="color: red;">My Gradescope autograder is broken, so submissions are not live right now. I'll update you when I've fixed it. Sorry!</span>

This assignment is intended to provide you experience in building/manipulating adjacency list representations of graphs, and to reinforce your understanding of BFS and DFS by adapting them to solve a novel problem. Here is a link to the [PA1 Task Description](/files/pa/pa1_writeup.pdf). Here is a [zip file](/files/pa/KidneyDonation.zip) with some starter code (in python and java both) and test cases. Modify the `DonorCycle.java` or `donor_cycle.py` file (you don't need to do both!) to solve the problem described in the writeup. To submit, re-zip the folder and upload to Gradescope.

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

