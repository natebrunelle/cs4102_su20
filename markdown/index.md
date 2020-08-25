---
title: cs4102
...

<div style="display:table; font-size:200%; margin: 1em auto; padding:1ex; box-shadow: 0 1px 10px rgba(0,0,0,.1); border: thin solid #eee; border-radius:1ex; background-image: linear-gradient(to bottom, #ffffff, #f2f2f2);">[Join Lecture (links to piazza for security)](https://piazza.com/class/ke4kba81aay39?cid=6)</div>

# Course Overview 

The goal of this course is to build a tool kit to better solve a variety of computational problems, and to evaluate the quality of such solutions. In particular, we will cover:

- Formal metrics for evaluating algorithm complexity (including the asymptotic classes big-oh, big-omega, big-theta, little-oh, and little-omega)
- Evaluating an algorithm's usage of resources (including time and space complexities) by a worst-case analysis, expected-case analysis, and amortized analysis
- Algorithm design strategies (including divide and conquer, dynamic programming, greedy, and reductions)
- The impact of data-structure choice on algorithm design
- Proving algorithm correctness
- Proving worst-case lower bounds on algorithm efficiency
- Discussion of randomized algorithms and expected efficiency
- Algorithms on graphs
- NP-Completeness

## Learning Outcomes

At the conclusion of this course, a successful student will be able to:

- Analyze a pre-written algorithm to determine its resource complexity
- Employ the strategies of divide and conquer, greedy, and dynamic programming (perhaps in concert) to develop novel algorithms
- Prove the correctness of algorithms built using these strategies
- Identify trade-offs in algorithm design (such as time vs. space, average-case vs. worst case, dynamic vs. static)
- Prove lower bounds on algorithm complexity



## Eligibility

You should take this course if and only if

1. You earned at least a C- in CS 2150 (or an equivalent data structures course)
1. You earned at least a C- in CS 2102 (or an equivalent discrete math course)


### Background

This course will assume knowledge of several topics from discrete math (CS2102 at UVA), two semesters of programming experience (through CS2110 at UVA), and data structures (CS2150 at UVA)

In particular, we assume knowledge of (with recommended resources for review):

- Logarithms and identities ([Log rules](https://en.wikipedia.org/wiki/List_of_logarithmic_identities))
- Sets ([CS2102 Sets Primer](http://www.cs.virginia.edu/luther/DMT1/S2020/sets.html))
- Functions ([Section 4.3 of this text](http://www.cs.virginia.edu/luther/DMT1/S2020/files/mcs.pdf))
- Proof Techniques ([CS2102 Proof Techniques](http://www.cs.virginia.edu/luther/DMT1/S2020/techniques-q8.html))
- Proof Styles, we'll mostly be using "prose proofs" ([CS2102 Proof style guide](http://www.cs.virginia.edu/luther/DMT1/S2020/proofs.html))
- Logic and Notation ([CS2102 Glossary of logical terms](http://www.cs.virginia.edu/luther/DMT1/S2020/glossary.html))
- Recursion ([CS2110 part 1](https://deternitydx.github.io/uvacs4102/pdfs/31-recursion.pdf), [CS2110 part 2](https://deternitydx.github.io/uvacs4102/pdfs/32-recursion.pdf))
- Trees ([CS2150 trees](https://aaronbloomfield.github.io/pdr/slides/05-trees.html#/))
- Queues ([CS2150 lists](https://aaronbloomfield.github.io/pdr/slides/02-lists.html#/))
- Stacks ([CS2150 lists](https://aaronbloomfield.github.io/pdr/slides/02-lists.html#/))
- Priority Queues ([CS2150 Heaps](https://aaronbloomfield.github.io/pdr/slides/10-heaps-huffman.html#/cover))
- Hash Tables ([CS2150 Hashing](https://aaronbloomfield.github.io/pdr/slides/06-hashes.html#/cover))
- Graphs ([CS2150 Graphs](https://aaronbloomfield.github.io/pdr/slides/11-graphs.html#/cover))

For each of the CS2102 topics, you can view last [semester's lectures](http://www.cs.virginia.edu/luther/DMT1/S2020/schedule.html) for more information

## Course Structure

You will see the following components in this course this semester. Look in the syllabus for the details on each:

- **Lectures**: Introduces new concepts, we expect all students to participate/view lectures
- **Workshops**: Gives additional examples and deeper discussions of topics discussed in lecture, this is optional for all students, but you may find it helpful
- **Exercises**: Collaborative work to develop your skills with course concepts
- **Quizzes**: Individual work to evaluate your fluency with course concepts
- **Office Hours**: Opportunity for individualized assistance with course concepts
- **Piazza**: A forum to ask questions that you think might be valuable for other students to see answered, that could be answered by other students, or that you prefer to ask outside of an office-hours/lecture environment.



# What to expect

## In this course

In the opinion of the course staff, an algorithms course should serve to:

1. introduce students to particular noteworthy and/or widely-used algorithms, and
1. provide opportunity for students to hone their skill in developing efficient algorithms.

Since developing a skill is a much more substantial undertaking than understanding prior work of others, the majority of your homework time will be spent on developing that skill. This will be at times uncomfortable, occasionally frustrating, but hopefully always fun and valuable (at least in retrospect). We have a few guidelines/suggestions for how you can get the most out of this course:

1. Follow the instructions in the assignments. The instructors have been students before, and understand the dizzying experience of learning something brand new. For this reason, we do not ask trick questions that are specifically intended to mislead you. 
1. Think carefully and precisely: While we will not purposefully mislead you, we may ask questions that are specifically designed to challenge an incorrect intuition or common misconception.
1. Don't expect homework to match lecture perfectly: Lecture is designed to introduce topics/concepts/strategies, and show how they operate. To maximize the future usefulness of this course, the course covers ideas whose applications are broad. Almost always, the homework directions will tell you which ideas to employ. It will probably not be obvious how or why that idea is relevant, but we promise it is. The goal of the assignment is to broaden your understanding of the idea so that it will be more useful to you when you complete this class.




## In an online course

As you're likely aware, there are challenges presented by the online course format which can make learning more challenging. If there are things we can do to make the course work better for you with this online format, please let us know, and we'll do our best to work in those recommendations. 

We have also provided some suggestions for how you can best set yourself up for learning in this course as well as others:

1. **Dedicate time and space** One of the most important things you can do to help yourself is to set aside time and space for your studies. Once you've selected that time and space, try to only do work at that time and in that location. As much as possible, don't use that time or place for anything else. Pick a chair in your bedroom, a spot on the floor, a chair at the kitchen table, or whatever you can do with the space you're in.
1. **Introduce yourself** Come to office hours, turn on your video, and introduce yourself to your classmates. This could be helpful in you forming a study/work group for the class. It could also help you to make new friends!
1. **Attend live meetings** If you're able to, attending live lectures and problem-solving-sessions will help to establish your routine, put you in the learning mindset, and remind you that you're learning in a community. If you're not able to attend live lecture, then try to view the lecture at the same time every day, and please ask questions about lecture on piazza to (at least somewhat) mimic the interactions present in a live setting.
1. **Be active** You likely moved around outside a lot when you were transitioning among your classrooms, dorms, libraries, and dining areas. Try your best to mimic that frequent activity, as it helps you to kind of "refresh" for the next task. Take several short walks a day (don't forget your mask), do yoga, hop on a stationary bike, do whatever activity most appeals to you.






