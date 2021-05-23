---
title: cs4102
...

<div style="display:table; font-size:200%; margin: 1em auto; padding:1ex; box-shadow: 0 1px 10px rgba(0,0,0,.1); border: thin solid #eee; border-radius:1ex; background-image: linear-gradient(to bottom, #ffffff, #f2f2f2);">[Lecture Link in Collab (Weekdays at 10:30am)](collab.its.virginia.edu)</div>

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

1. You have credit for  CS 2150 (or an equivalent data structures course)
1. You have credit for CS 2102 (or an equivalent discrete math course)


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




# What to expect

## In this course

In the opinion of this instructor, an algorithms course should serve to:

1. introduce students to particular noteworthy and/or widely-used algorithms, and
1. provide opportunity for students to hone their skill in developing efficient algorithms.

Since developing a skill is a much more substantial undertaking than understanding prior work of others, the majority of your homework time will be spent on developing that skill. This will be at times uncomfortable, occasionally frustrating, but hopefully always fun and valuable in retrospect. I have a few guidelines/suggestions for how you can get the most out of this course:

1. Follow the instructions in the assignments. I've been a student before, and I understand the dizzying experience of learning something brand new. For this reason, I do not ask trick questions that are specifically intended to mislead you. 
1. Think carefully and precisely: While I will not purposefully mislead you, I may ask questions that are specifically designed to challenge an incorrect intuition or common misconception.
1. Don't expect homework to match lecture perfectly: Lecture is designed to introduce topics/concepts/strategies, and show how they operate. To maximize the future usefulness of this course, I selected ideas whose applications are broad. Almost always, I will tell you which ideas to employ. It will probably not be obvious how or why that idea is relevant, but I promise it is. The goal of the assignment is to broaden your understanding of the idea so that it will be more useful to you when you complete this class.


## In a summer course

A typical spring/fall semester at UVA is ~15 weeks long (including exams), whereas a summer course is 4 weeks long. This means that summer courses are accelerated roughly 4x compared to a course offered in the spring/fall. Considering that a full-time courseload at UVA is 12 credit hours, expect a 3 credit-hour course offered during the summer (like this one) to require a full-time workload. Another way to think about it: the amount of time you spend per day on this one summer course should roughly match the aggregate amount of work you would spend per day on all your courses during a normal semester.

As a warning, with this 4x acceleration, it can be very difficult to catch up if you fall behind. Each lecture session this summer is 135 minutes. During a normal semester you have 150 minutes of instruction per week. This means that each summer lecture contains nearly a week's worth of content. Keep this in mind if you need to take a day off due to illness, etc.

Now that I've sufficiently warned you, please take comfort that I have done my best in trying to make this course workable with a summer schedule. The structures have been designed based on extensive student feedback. The most successful students tend to approach this course like a full-time job, establishing a regular work schedule of 9ish hours of work per day (amortized).

## In an online course

As I'm sure you're aware, there are challenges presented by the online course format which can make learning more challenging. If there are things I can do to make the course work better for you with this online format, please let me know, and I'll do my best to work in those recommendations. To start with, here are the resources and suggestions that are provided by the course staff.

Course structures:

1. **Lecture**: will be hosted live online via zoom. Recordings will be posted after (sometimes it takes zoom a few hours to master the video). Due to instances of "zoom bombing", you will need a password to join (find it on piazza)
1. **Cohorts**: you are invited to participate in a cohort if you choose. These will be groups of approximately 6 students total who will work together on many of the tasks throughout the session (rules and restrictions on the collaboration depend on the type of task).
1. **Discord**: We will be using Discord for all course communication (announcements, office hours, memes, intra-cohort messaging, etc.). We highly encourage you to post questions or resources that you think could benefit your peers. This is also the best place to post questions outside of office hours.
1. **Office Hours**: There will be instructor and TA office hours on all class days (at least) hosted via Discord. These will be open chat rooms for you to discuss with course staff and classmates.
1. **Online submissions**: Problem set solutions must be submitted by pdf. Quizzes may be submitted as either a pdf or a txt file. We do not have a preference for how the pdfs are generated (LaTeX, Microsoft Word, pictures of handwriting are all acceptable) so long as what is submitted is legible, easy to follow, and you use the appropriate mathematical symbols when necessary (please use the equation editor if you're using Word). Please draft you submissions with readability in mind, submissions that appear as notes may not be accepted.


Some suggestions:

1. **Dedicate time and space** One of the most important things you can do to help yourself is to set aside time and space for your studies. Once you've selected that time and space, try to only do work at that time and in that location. As much as possible, don't use that time or place for anything else. Pick a chair in your bedroom, a spot on the floor, a chair at the kitchen table, or whatever you can do with the space you're in.
1. **Introduce yourself** If you opt in on the beginning of course questionnaire (little_1a), we will post a short bio about you on the course webpage. This could be helpful in you forming a study/work group for the class. It could also help you to make new friends!
1. **Attend live lecture** If you're able to, attending live lecture will help to establish your routine, put you in the learning mindset, and remind you that you're learning in a community.






