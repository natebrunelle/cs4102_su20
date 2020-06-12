---
title: Exercise 1 Enchantress of Numbers
...

# Introduction

From the notes of Ada Lovelace[^future]:

>*\[The Analytical Engine\] might act upon other things besides number, were objects found whose mutual fundamental relations could be expressed by those of the abstract science of operations, and which should be also susceptible of adaptations to the action of the operating notation and mechanism of the engine...Supposing, for instance, that the fundamental relations of pitched sounds in the science of harmony and of musical composition were susceptible of such expression and adaptations, the engine might compose elaborate and scientific pieces of music of any degree of complexity or extent.*

Throughout the semester, our models of computing will almost exclusively use binary strings as their input/output type. In this assignment you will explore the representation of several objects in binary, illustrating that binary strings are sufficient for an incredible variety of applications. This assignment will give you experience in comparing sizes of set, toward determining how many bits a representation might require, or if a binary representation is even possible. You will be asked to write a few proofs relating to these concepts, and also implement binary representations of two new types.

[^future]: Ada Lovelace was dubbed the "Enchantress of Numbers" by Charles Babbage.

# Exercises 1-1 through 1-4: Written Problems

Answer each of the problems contained in [this pdf](/files/exercises/exercise1.pdf) with an accompanying proof.

To begin, download [exercise1.zip](/files/exercises/exercise1.zip) and upload as a new project in overleaf. Within that zip you will see 5 tex files. the `exercise1.tex` file contains the which generates the pdf. You will provide your answers in the `exercise1-1.tex`, `exercise1-2.tex`, `exercise1-3.tex`, and `exercise1-4.tex` files. 

First, change `\submitter{TODO: your name}` in `exercise1.tex` to contain your name and UVA email id (e.g. `\submitter{Grace Hopper (gmh1a)}`)

Next, cite all your sources in `\collaborators{TODO: replace ...}` according to the [course policy](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/syllabus.html#no-plagiarism-nor-anything-like-it)

At this point, fill in all of your solutions in the proper tex file. When you rebuild the pdf, your solutions should appear as you write them.


## Deliverable

You will need to submit a separate pdf for each of the exercises 1-1, 1-2, 1-3, and 1-4. We do this for a few reasons: we can release individual problems' grades as they're graded rather than waiting for the whole problem set to be graded, we can adjust deadlines for individual problems if necessary, if you need extra time on one problem then you can submit just that one late instead of receiving a late penalty on all problems, etc.  We have made it easy for you to get these separate pdfs, however.

At the very top of `exercise1.tex` there is a line which reads `\usepackage{uvatoc}`. That line tells LaTeX include everything in the pdf. To include only one problem, comment that line out and uncomment (one at a time) `\usepackage[response1]{uvatoc}`, `\usepackage[response2]{uvatoc}`, `\usepackage[response3]{uvatoc}`, and `\usepackage[response4]{uvatoc}` to build a pdf with only exercise 1-1, 1-2, 1-3, and 1-4 respectively.

Rename the pdf files for the appropriate exercise, and submit to the [assignments page](https://kytos.cs.virginia.edu/cstheory)


# Exercise 1-5: Programming Problems

For these problems, you will be implementing binary representations of two different types: integers and integer Cartesian coordinates (i.e. ordered pairs of integers). We have additionally provided an implementation of a binary representation of natural numbers, which you are welcome to use as subroutines in your implementations.


Integers and Cartesian coordinates were chosen to illustrate a counter-intuitive points regarding infinite sets. In class, we demonstrated that the cardinality of the natural numbers matches that of the set of all binary strings. 

In this assignment, by implementing a binary representation of integers, you're demonstrating that the cardinality of the integers is equal to that of the natural numbers. This is despite the fact that there are, intuitively, two integers for each natural number: a positive and a negative.

Additionally, by implementing a binary representation of integer Cartesian Coordinates, you're demonstrating that the cardinality of the pairs of integers is equal to that of the natural numbers (and therefore the integers as well). This is despite the fact that there are, intuitively, and infinite number of ordered pairs for each natural number: (0,0), (0,1), (0,2), (0,3), ...

Hopefully, this helps you to appreciate that even though binary strings are countable (the smallest infinity) and therefore we can't represent some sets we care about (e.g. the real numbers), there is still **a lot** that we *can* represent with binary strings.


## Deliverable

Before you begin on this assignment, download either [binary_strings.py](/files/exercises/exercise1_python/binary_strings.py) or [binary_strings.java](/files/exercises/exercise1_java/binary_strings.java) depending on which programming language you prefer. Do ctrl+f and search for "TODO" to find all places where you must fill in code. Please do not change any code you’re not instructed to change. (If you’re using java, do not add a package to your program.)

Follow the instructions in the program you downloaded (follow them line-by-line in python, follow the numbers in order in Java). Submit the completed binary_strings file. Your code will receive full credit provided you followed the instructions and, when run (with asserts enabled), the printed output has exclusively encouraging messages (and has no errors).

If you are stuck on one of the asserts, comment out that assert statement to skip it.


