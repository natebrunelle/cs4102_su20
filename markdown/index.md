---
title: cs4102
...


# Course Overview 

The goal of this course is to build a tool kit to better solve a variety of computational problems, and to evaluate the quality of such solutions. In particular, we will cover:

- Formal metrics for evaluating algorithm complexity (including the asymptotic classes big-oh, big-omega, big-theta, little-oh, and little-omega)
- Evaluating an algorithm's usage of resources (including time and space complexities) by a worst-case analysis, expected-case analysis, and amortized analysis
- Algorithm design strategies (including divide and conquer, dynamic programming, greedy, and reductions)
- The impact of data-structure choice on algorithm design
- Proving algorithm correctness
- Proving worst-case lower bounds on algorithm efficiency
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

1. You have credit for CS 2100, CS 2150, or an equivalent data structures course
1. You have credit for CS 2102, CS 2120, or an equivalent discrete math course


### Background

This course will assume knowledge of several topics from discrete math (CS2102 at UVA), two semesters of programming experience (through CS2110 at UVA), and data structures (CS2150 at UVA)

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
- Graphs ([CS2150](https://aaronbloomfield.github.io/pdr/slides/11-graphs.html#/cover))

For each of the Discrete Math topics, the [Fall 2019 lectures](http://www.cs.virginia.edu/luther/DMT1/F2019/schedule.html) are publicly available.




# What to expect

## In an algorithms course

In the opinion of this instructor, an algorithms course should serve to:

1. introduce students to particular noteworthy and/or widely-used algorithms, and
1. provide opportunity for students to hone their skill in developing correct and efficient algorithms.

Since developing a skill is a much more substantial undertaking than understanding prior work of others, the majority of your homework time will be spent on developing that skill. This will be at times uncomfortable, occasionally frustrating, but hopefully always fun and valuable in retrospect. I have a few guidelines/suggestions for how you can get the most out of this course:

1. Follow the instructions in the assignments. I've been a student before, and I understand the dizzying experience of learning something brand new. For this reason, I do not ask trick questions that are specifically intended to mislead you. 
1. Think carefully and precisely: While I will not purposefully mislead you, I may ask questions that are specifically designed to highlight and correct a misleading intuition or common misconception.
1. Don't expect homework to match lecture perfectly: Lecture is designed to introduce topics/concepts/strategies, and show how they operate. To maximize the future usefulness of this course, I selected ideas whose applications are broad. Almost always, I will tell you which ideas to employ. It will probably not be obvious how or why that idea is relevant, but I promise it is. The goal of the assignment is to broaden your understanding of the idea so that it will be more useful to you when you complete this class.


## In a summer course

A typical spring/fall semester at UVA is ~15 weeks long (including exams), whereas a summer course is 4 weeks long. This means that summer courses are accelerated roughly 4x compared to a course offered in the spring/fall. Considering that a full-time courseload at UVA is 12 credit hours, expect that a 3 credit-hour course offered during the summer (like this one) will require a full-time workload. Another way to think about it: the amount of time you spend per day on this one summer course should roughly match the aggregate amount of work you would spend per day on all your courses during a normal semester.

As a warning, with this 4x acceleration, it can be very difficult to catch up if you fall behind. Each lecture session this summer is 135 minutes. During a normal semester you have 150 minutes of instruction per week. This means that each summer lecture contains nearly a week's worth of content. Keep this in mind if you need to take a day off due to illness, etc.

Now that I've sufficiently warned you, please take comfort that I have done my best in trying to make this course workable with a summer schedule. The structures have been designed based on extensive student feedback. The most successful students tend to approach this course like a full-time job, establishing a regular work schedule of 8-9 hours of work per day (amortized).

# Can I take this course online?

Officially, no. Unless specifically designated as an online course, all UVA courses are in-person. That being said, I will do my best to produce and share recordings of the in-person lectures, and will never take attendance. Assignments will be posted, submitted, and graded online. We will not have any graded in-class activities (including exams). However, most (but not all) office hours in person. Additionally, most homework assignments are open for collaboration, which will be harder to do virtually. 

In summary, it's hypothetically possible to participate exclusively virtually and succeed in the course, but I'm assuming that all students can appear in-person, and so you'll have a better experience if you are physically present.


