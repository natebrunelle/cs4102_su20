---
title: Exercise 4 Automata Tune
...


# Introduction

The purpose of this assignment is to finite state automata as a model of computing. To start with, you will be implementing several computations as Deterministic Finite State Automata (DFAs) and others as Non-Deterministic Finite State Automata (NFAs). You'll also be asked to prove some things about finite automata.

As an aside, these finite automata may seem to be the least "real" of the models of computing so far. However, as we will see, they're actually incredibly useful. Finite state automata are routinely used for a wide variety of applications:

- String matching (how similar are two strings?), including [Hamming distance](https://en.wikipedia.org/wiki/Hamming_distance) and [Edit distance](https://en.wikipedia.org/wiki/Edit_distance). These metrics are both used extensively for reconstructing genomes when doing genetic sequencing.
- Virus scanning, most notably [ClamAV](https://en.wikipedia.org/wiki/Clam_AntiVirus) and [Snort](https://en.wikipedia.org/wiki/Snort_(software)).
- [Decision-Tree models for Machine Learning](https://www.cs.virginia.edu/~tjt7a/docs/accelerating-random-forests.pdf)
- Formal software verification using [Linear Temporal Logic](https://www.cs.rice.edu/~vardi/papers/ijcai13.pdf) 
- Psuedo-random number generation [shameless plug](https://patents.google.com/patent/US9977652)

This assignment will also help you to get acquainted with closure and with regular expressions. As an aside, here is a regular-expressions-motivated reason that we prefer the way we represent natural numbers be onto: [Regexes for Roman Numberals](https://www.youtube.com/watch?v=M3x5Z3iIoSU&fbclid=IwAR0DZeaS_P5GyEBUkNUNJotDExLelFOBFCx5NQSS2nORjfnfng6_B-XwTo8).

# Exercise 4-1: DFA Programming Problems

The programming problems for this assignment will guide you through implementing the EVAL function discussed in class. Will will be building up the subroutines we will need. Use the psuedocode presented in class or in the textbook to guide you through it.


## Deliverable

Before you begin on this assignment, you will need to download two (or three) files, depending on your programming language of choice:

- Java: [DFA.java](/files/exercises/exercise4_java/DFA.java), [Tuple.java](/files/exercises/exercise4_java/Tuple.java) and [SeveralDFAs.java](/files/exercises/exercise4_java/SeveralDFAs.java).
- Python: [DFA.py](/files/exercises/exercise4_python/DFA.py), and [several_dfas.py](/files/exercises/exercise4_python/several_dfas.py)

(**If you’re using java, do not add a package declaration to your program.**)

The programming problems for this assignment work a little differently from what we've done in the previous assignments. For this one, there is not a guided exploration of the course materials with asserts and such. For this exercise you will be simply implementing three functions. The functions you are implementing are in the `several dfas` files, and only submit your `several dfas` file. You should not make any edits to the `DFA` file, and you will not submit it.

Inside `several dfas` there are 3 functions you must implement (each marked with TODO). These three functions don't do anything other than create and return a finite state automaton for a particular language. You'll see that in each I begin by providing you and example of how to implement an automaton by giving an implementation of infinte XOR and AND. In both the python and java code, to create a DFA you must define the 5 components we discussed in class:

- State set
- alphabet set
- starting state
- set of final states
- transition function

The state set is a set of strings, the alphabet is a set of characters, the starting state is a string (that should be in your state set as well), the set of final states is a set of string (and should be a subset of the state set), and the transition function is a map/dictionary (it maps state-character tuples to states). The java code has 3 files because it has an impelemention of tuples to encapsulate the state-character pairs.

After you create an automaton, you will need to test and debug it on your own. I have given you some pretty powerful tools to be able to do this. If you have a DFA in your program called `dfa`:

- You can convert an automaton to a string describing it using `dfa.toString()` in Java, or `str(dfa)` in python. This will display to you everything you might want to know about the automaton (currently active state, start state, transitions, final states, etc.)
- You can use `dfa.step(character)` to transition on a single character. Its return value is a boolean representing whether or not the new state is a final state. You can use `dfa.active` to get its current state.
- You can use `dfa.execute(string)` to run the machine on a given input string, its return value is a boolean representing whether or not the state that it ends in is a final state.
- You can visualize the automaton by invoking the `dfa.toDot()`. This method will print out a description of the automaton in the dot file format, which you can then convert into an image using an [online tool](https://dreampuf.github.io/GraphvizOnline/). To see your automaton, invoke `dfa.toDot()` and then copy-paste the printed text into that tool.


### Hamming Distance

I believe that the first two machines you're asked to implement are more self-explanatory, but the third (Hamming distance) is a bit trickier. 

First of all, the Hamming Distance between strings x and y is the minimum number of substitutions needed to convert the string x into the string y. For example, if x is the string "nate", then we would have the following Hamming Distance when comparing to different choices for y:

- y = "nate" has Hamming distance 0 (they're the same string, no subtitutions required)
- y = "hate" has Hamming distance 1 (substitute an "h" for an "n")
- y = "note" has Hamming distance 1 (substitute an "o" for an "a")
- y = "hath" has Hamming distance 2 (substitute an "h" for an "n" and an "h" for an "e")
- y = "moth" has Hamming distance 3 (substitution an "m" for an "n", an "o" for an "a", and an "h" for an "e")
- y = "rich" has Hamming distance 4 
- y = "naters" has Hamming distance infinity (we cannot convert "nate" to "naters" through subtitutions alone)

For this function, you'll need to create a different machine depending on the arguments given to that function. The arguments given are the string we're matching against, and the distance we would like to see. If we give the function the arguments "nate" and 2, then the automaton should return 1 for "nate", "hate", "note", "hath" (of those above), and return 0 for the rest. 

Essentially, the string and distance will be "hard-coded" into the automaton when you make it. The general idea for how this works is to have an automaton with states arranged in a grid. The column of a state represents how many characters of the string you've read so far, so the number of columns is equal to the length of the parameter string plus 1 (one column for each value 0-length). You advance one column every transition. The row of a state represents the total amount of distance "accumulated" thus far, so the number of rows is equal to the allowable distance plus a (one row for each value 0-distance). Every time the input string has a character which does not match that of the parameter string you move up one row. 

The image below shows an example of invoking the function with the string "aaaa" and the distance 2.

<img src=files/images/hamming.png height="500" >






# Exercises 4-2 through 4-5 Written problems.

Answer each of the problems contained in [this pdf](/files/exercises/exercise4.pdf) with an accompanying proof.

To begin, download [exercise4.zip](/files/exercises/exercise4.zip) and upload as a new project in overleaf. Within that zip you will see 6 tex files. the `exercise4.tex` file contains the code which generates the pdf. You will provide your answers in the `exercise4-2.tex`, `exercise4-3.tex`, `exercise4-4.tex`, and `exercise4-5.tex` files. 

First, change `\submitter{TODO: your name}` in `exercise4.tex` to contain your name and UVA email id (e.g. `\submitter{Grace Hopper (gmh1a)}`)

Next, cite all your sources in `\collaborators{TODO: replace ...}` according to the [course policy](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/syllabus.html#no-plagiarism-nor-anything-like-it)

At this point, fill in all of your solutions in the proper tex file. When you rebuild the pdf, your solutions should appear as you write them.


## Deliverable

You will need to submit a separate pdf for each of the exercises 4-2, 4-3, 4-4, and 4-5. We do this for a few reasons: we can release individual problems' grades as they're graded rather than waiting for the whole problem set to be graded, we can adjust deadlines for individual problems if necessary, if you need extra time on one problem then you can submit just that one late instead of receiving a late penalty on all problems, etc.  We have made it easy for you to get these separate pdfs, however.

At the very top of `exercise4.tex` there is a line which reads `\usepackage{uvatoc}`. That line tells LaTeX include everything in the pdf. To include only one problem, comment that line out and uncomment (one at a time) `\usepackage[response2]{uvatoc}`, `\usepackage[response3]{uvatoc}`, `\usepackage[response4]{uvatoc}`, `\usepackage[response5]{uvatoc}` and `\usepackage[response6]{uvatoc}` to build a pdf with only exercise 4-2, 4-3, 4-4, and 4-5 respectively.

Rename the pdf files for the appropriate exercise, and submit to the [assignments page](https://kytos.cs.virginia.edu/cstheory).

