---
title: Exercise 2 Cirque du Ligne Droite
...

# Introduction

The purpose of this assignment is to develop your understanding of finite computation, focusing on the
material in Chapter 3 of the textbook and the AON/NAND computing models discussed therein as well as in class. 

These are models for finite computation because there is no way to provide dynamically-sized inputs within these models, instead each implementation can only accept inputs of a fixed length.

As we continue to study these models in class, we will explore the ways finite models are limitated, but also ways that they are valuable.

## Why the title is funny

In the humble opinion of Nate Brunelle, the title of this assignment is funny. The French "Cirque du Ligne Droite" translates to "Straight Line Circus". Nate thinks it's funny because it's kind of like "Cirque du Soleil". It's funnier because Circus sounds like circuit, and circuits and straightline programs are our models of computing so far (get it?). It's even FUNNIER because "circus" and "circuit" come from the same Latin root which means "circle", so it's an oxymoron to have a circular straightline. (Get it? Please say yes. Oh, gosh ... what have I done?!)

# Exercise 2-1: Programming Problems

The programming problems for this assignment are intended to get you acquainted with the AON-Straightline computing model. Most of what you'll be doing here is implementing a few functions in this model. I encourage you to additionally practice the AON-Circuit model by either implementing each function as a circuit and then converting to Straightline, or else converting your implemented straightline program to a circuit (in either case, you are only required to submit the straightline).

*Edit 2020-02-03: I neglected to remove the testing code from straightline.py, giving away the solution to the IMPL method. I encourage you to implement it on your own for the experience, but it will not be assessed as part of your grade.*

*Edit 2020-02-05: For COMPARE4, I originally required that you implement it in AON-Straightline (i.e. with ANDs, ORs, or NOTs only). I have decided to relax this requirement. I recommend implementing COMPARE4 by first implementing COMPARE3. To give you a hint on how this might work, if the most significant bit of two strings differ, then you can immediately tell which value is bigger. If the most significant bits match, then you are comparing two strings that are 1 bit shorter. If you impelement functions for COMPARE3, COMPARE2, COMPARE1, and IF, you may use those as subroutines for COMPARE4. If you did/do translate COMPARE4 to only AON, then that will be worth some extra credit.*

## Deliverable

Before you begin on this assignment, download either [straightline.py](/files/exercises/exercise2_python/straightline.py) or [straightline.java](/files/exercises/exercise2_java/straightline.java) depending on which programming language you prefer. Do ctrl+f and search for "TODO" to find all places where you must fill in code. Please do not change any code you’re not instructed to change. (**If you’re using java, do not add a package declaration to your program.**)

Follow the instructions in the program you downloaded (follow them line-by-line in python, follow the numbers in order in Java). Submit the completed straightline file. Your code will receive full credit provided you followed the instructions and, when run (with asserts enabled), the printed output has exclusively encouraging messages (and has no errors).

If you are stuck on one of the asserts, comment out that assert statement to skip it.


# Exercises 2-2 through 2-5: Written Problems

Answer each of the problems contained in [this pdf](/files/exercises/exercise2.pdf) with an accompanying proof.

To begin, download [exercise2.zip](/files/exercises/exercise2.zip) and upload as a new project in overleaf. Within that zip you will see 5 tex files. the `exercis21.tex` file contains the which generates the pdf. You will provide your answers in the `exercise2-2.tex`, `exercise2-3.tex`, `exercise2-4.tex`, and `exercise2-5.tex` files. 

First, change `\submitter{TODO: your name}` in `exercise2.tex` to contain your name and UVA email id (e.g. `\submitter{Grace Hopper (gmh1a)}`)

Next, cite all your sources in `\collaborators{TODO: replace ...}` according to the [course policy](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/syllabus.html#no-plagiarism-nor-anything-like-it)

At this point, fill in all of your solutions in the proper tex file. When you rebuild the pdf, your solutions should appear as you write them.


## Deliverable

You will need to submit a separate pdf for each of the exercises 2-2, 2-3, 2-4, and 2-5. We do this for a few reasons: we can release individual problems' grades as they're graded rather than waiting for the whole problem set to be graded, we can adjust deadlines for individual problems if necessary, if you need extra time on one problem then you can submit just that one late instead of receiving a late penalty on all problems, etc.  We have made it easy for you to get these separate pdfs, however.

At the very top of `exercise2.tex` there is a line which reads `\usepackage{uvatoc}`. That line tells LaTeX include everything in the pdf. To include only one problem, comment that line out and uncomment (one at a time) `\usepackage[response2]{uvatoc}`, `\usepackage[response3]{uvatoc}`, `\usepackage[response4]{uvatoc}`, and `\usepackage[response5]{uvatoc}` to build a pdf with only exercise 2-2, 2-3, 2-4, and 2-5 respectively.

Rename the pdf files for the appropriate exercise, and submit to the [assignments page](https://kytos.cs.virginia.edu/cstheory).

