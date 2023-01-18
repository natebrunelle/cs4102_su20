---
title: cs3100
...


# Course Overview 

The goal of this course is to build a tool kit to better solve a variety of computational problems, and to evaluate the quality of such solutions. In particular, we will cover:

- Formal metrics for evaluating algorithm complexity (including the asymptotic classes big-oh, big-omega, big-theta, little-oh, and little-omega)
- Evaluating an algorithm's usage of resources (including time and space complexities) by a worst-case analysis, expected-case analysis, and amortized analysis
- Algorithm design strategies (including divide and conquer, dynamic programming, greedy, and reductions)
- The impact of data-structure choice on algorithm design
- Proving algorithm correctness
- Proving worst-case lower bounds on algorithm efficiency using reductions
- Algorithms on graphs

## Learning Outcomes

At the conclusion of this course, a successful student will be able to:

- Analyze a pre-written algorithm to determine its resource complexity
- Employ the strategies of divide and conquer, greedy, and dynamic programming (perhaps in concert) to develop novel algorithms
- Prove the correctness of algorithms built using these strategies
- Identify trade-offs in algorithm design (such as time vs. space, average-case vs. worst case, dynamic vs. static)
- Prove lower bounds on algorithm complexity



## Eligibility

You should take this course if and only if

1. You have credit for CS 2100, CS 2150, or an equivalent data structures course
1. You have credit for CS 2120, CS 2102, or an equivalent discrete math course


### Background

This course will assume knowledge of several topics from discrete math (CS2120 at UVA), two semesters of programming experience (through CS2100 at UVA), and data structures (also CS2100 at UVA)

In particular, we assume knowledge of (with recommended resources for review):

- Logarithms and identities ([Log rules](https://en.wikipedia.org/wiki/List_of_logarithmic_identities))
- Sets ([CS2102 Sets Primer](https://www.cs.virginia.edu/~njb2b/cs2120/f2021/sets.html))
- Functions ([Section 4.3 of this text](http://www.cs.virginia.edu/~njb2b/cs2120/f2021/files/mcs.pdf))
- Proof Techniques ([CS2102 Proof Techniques](http://www.cs.virginia.edu/~njb2b/cs2120/f2021/techniques-q8.html))
- Proof Styles, we'll mostly be using "prose proofs" ([CS2102 Proof style guide](http://www.cs.virginia.edu/~njb2b/cs2120/f2021/proofs.html))
- Logic and Notation ([CS2102 Glossary of logical terms](http://www.cs.virginia.edu/~njb2b/cs2120/f2021/glossary.html))
- Recursion ([CS2100](https://markfloryan.github.io/dsa1/slides/04-trees.html#/3/1), [CS2110 part 1](https://deternitydx.github.io/uvacs4102/pdfs/31-recursion.pdf), [CS2110 part 2](https://deternitydx.github.io/uvacs4102/pdfs/32-recursion.pdf))
- Trees ([CS2100](https://markfloryan.github.io/dsa1/slides/04-trees.html#/), [CS2150](https://aaronbloomfield.github.io/pdr/slides/05-trees.html#/))
- Lists ([CS2100](https://markfloryan.github.io/dsa1/slides/02-lists.html#/), [CS2150]())
- Queues ([CS2100](https://markfloryan.github.io/dsa1/slides/02-lists.html#/queues), [CS2150](https://aaronbloomfield.github.io/pdr/slides/02-lists.html#/queues))
- Stacks ([CS2100](https://markfloryan.github.io/dsa1/slides/02-lists.html#/stacks), [CS2150](https://aaronbloomfield.github.io/pdr/slides/02-lists.html#/stacks))
- Priority Queues ([CS2100](https://markfloryan.github.io/dsa1/slides/07-priorityqueues.html#/), [CS2150](https://aaronbloomfield.github.io/pdr/slides/10-heaps-huffman.html#/cover))
- Hash Tables ([CS2100](https://markfloryan.github.io/dsa1/slides/06-hashing.html#/), [CS2150](https://aaronbloomfield.github.io/pdr/slides/06-hashes.html#/cover))

For each of the Discrete Math topics, the [Fall 2019 lectures](http://www.cs.virginia.edu/luther/DMT1/F2019/schedule.html) are publicly available.

# Platforms

Platform                    Purpose
-------------------------   ----------------------------------------------
This Website                Central repository of course information and content including: syllabus, schedule, file hosting, readings, assignment writeups, etc.
Collab                      Linking to all of the other tools, lecture recordings
Piazza                      Course content and policy questions
Discord                     Online office hours, informal interactions, homework collaboration
Gradescope                  Homework submission and grading


# What to expect in an algorithms course

In the opinion of this instructor, an algorithms course should serve to:

1. introduce students to particular noteworthy and/or widely-used algorithms, and
1. provide opportunity for students to hone their skill in developing and justifying correct and efficient algorithms.

Since developing a skill is a much more substantial undertaking than understanding prior work of others, the majority of your homework time will be spent on developing that skill. This will be at times uncomfortable, occasionally frustrating, but hopefully always fun and valuable in retrospect. I have a few guidelines/suggestions for how you can get the most out of this course:

1. Follow the instructions in the assignments. I've been a student before, and I understand the dizzying experience of learning something brand new. For this reason, I do not ask trick questions that are specifically intended to mislead you. If a question seems misleading, then most likely either there's something about the instructions or the content that you're missing, or else I made an error in drafting the assignment. In either case, the best thing to do is ask!
1. Think carefully and precisely: While I will not purposefully mislead you, I may ask questions that are specifically designed to expose and correct a misleading intuition or common misconception.
1. Don't expect homework to match lecture perfectly: Lecture is designed to introduce topics/concepts/strategies, and show how they operate. To maximize the future usefulness of this course's content, I selected topics whose applications are broad, and try to demonstrate that breadth thorugh a combination of lecture and homework. Almost always, I will tell you which topics to employ. It may not be obvious how or why that concept is relevant, but I promise it is. The goal of the assignment is to broaden your understanding of the concept so that it will be more useful to you when you complete this class.



# What to expect in office hours

Instructor and TA office hours will be available to assist you in understanding course concepts and applying those concepts to your assignments. Office hours should never be used as a substitute for your own learning or for your own earnest effort. As such, the amount of assistance the course staff will provide should correlate with the amount of effort you've made and understanding you possess. In short, the more effort and understanding you have demonstrated before arriving to office hours, the more precise the help we will provide. If you're just beginning to solve the problem or are missing some concept then the help given will be more conceptual in nature.

The CS department allocation to a non-lab course (like this one) is 20 minutes of TA time per week per student. This accounts for all time the TA spends on any course activity (office hours, grading, staff meetings, personal prep, etc.), so TAs have less that 20 minutes per student to spend in office hours. Because this resource can be scarce, here are some expectations and tips for managing office hours:

-  When there is a queue in office hours, we will limit each student-TA interaction to addressing just a single question. To ask multiple questions you will need to re-enter the queue. The reason for this policy is to help as many students as quickly as possible, since after a first round of assistance you will have an opportunity to make more progress on your own before your turn comes up again. I recommend arriving prepared with the question that is your biggest "blocker" to progress.
- When asking for help with debugging a programming assignment it will be best if you come prepared with test cases where your code gives the correct answer, and test cases where it gives the incorrect answer. This demonstrates substantial understanding of what your code is supposed to do and what your code is currently doing, and also gives the TA a lot of information to go off of, so you're more likely to receive more specific help.
- Work-in-progress code is often difficult for a third-party to read. Be prepared to help the course staff member to understand your approach.
- For quick clarification questions, consider using Piazza first. Your question may already be answered there, and even if not then you may get an answer faster compared to going to office hours.


