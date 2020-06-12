---
title: Exercise 3 Goldilocks and the 3 O's
...

# Introduction

The purpose of this assignment is to explore the EVAL function, counting functions, and asymptotic notation. 

The idea of EVAL is that we can have models of computing which are able to simulate instances of themselves. This idea is fundamental to the practice of computer science, as it enables us to have arbitrarily reprogrammable machines which run with fixed hardware.

Counting functions is important for evaluating the resources required for implementing functions, and helps us to study computing efficiency (i.e. complexity).

Asymptotic notation is used to study how algorithms and functions scale with 
arbitrarily large inputs, and is the basis for the study of complexity.


# Exercise 3-1: Programming Problems

The programming problems for this assignment will guide you through implementing the EVAL function discussed in class. Will will be building up the subroutines we will need. Use the psuedocode presented in class or in the textbook to guide you through it.


## Deliverable

Before you begin on this assignment, download either [eval.py](/files/exercises/exercise3_python/eval.py) or [eval.java](/files/exercises/exercise3_java/eval.java) depending on which programming language you prefer. Do ctrl+f and search for "TODO" to find all places where you must fill in code. Please do not change any code you’re not instructed to change. (**If you’re using java, do not add a package declaration to your program.**)

Follow the instructions in the program you downloaded (follow them line-by-line in python, follow the numbers in order in Java). Submit the completed straightline file. Your code will receive full credit provided you followed the instructions and, when run (with asserts enabled), the printed output has exclusively encouraging messages (and has no errors).

If you are stuck on one of the asserts, comment out that assert statement to skip it.


# Exercises 3-2 through 3-6: Written Problems

Answer each of the problems contained in [this pdf](/files/exercises/exercise3.pdf) with an accompanying proof.

To begin, download [exercise3.zip](/files/exercises/exercise3.zip) and upload as a new project in overleaf. Within that zip you will see 6 tex files. the `exercis3.tex` file contains the code which generates the pdf. You will provide your answers in the `exercise3-2.tex`, `exercise3-3.tex`, `exercise3-4.tex`, `exercise3-5.tex`, and `exercise3-6.tex` files. 

First, change `\submitter{TODO: your name}` in `exercise3.tex` to contain your name and UVA email id (e.g. `\submitter{Grace Hopper (gmh1a)}`)

Next, cite all your sources in `\collaborators{TODO: replace ...}` according to the [course policy](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/syllabus.html#no-plagiarism-nor-anything-like-it)

At this point, fill in all of your solutions in the proper tex file. When you rebuild the pdf, your solutions should appear as you write them.


## Deliverable

You will need to submit a separate pdf for each of the exercises 3-2, 3-3, 3-4, 3-5, and 3-6. We do this for a few reasons: we can release individual problems' grades as they're graded rather than waiting for the whole problem set to be graded, we can adjust deadlines for individual problems if necessary, if you need extra time on one problem then you can submit just that one late instead of receiving a late penalty on all problems, etc.  We have made it easy for you to get these separate pdfs, however.

At the very top of `exercise3.tex` there is a line which reads `\usepackage{uvatoc}`. That line tells LaTeX include everything in the pdf. To include only one problem, comment that line out and uncomment (one at a time) `\usepackage[response2]{uvatoc}`, `\usepackage[response3]{uvatoc}`, `\usepackage[response4]{uvatoc}`, `\usepackage[response5]{uvatoc}` and `\usepackage[response6]{uvatoc}` to build a pdf with only exercise 2-2, 2-3, 2-4, 2-5, and 2-6 respectively.

Rename the pdf files for the appropriate exercise, and submit to the [assignments page](https://kytos.cs.virginia.edu/cstheory).

*Edit Feb 13: The last couple of lectures took longer than I had anticipated. This is fine, but the result is that I didn't get to as much as I had expected for exercise 3-3, so I'm removing it from the problem set.*

