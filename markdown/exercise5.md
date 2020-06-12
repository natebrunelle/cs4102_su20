---
title: Exercise 5 Non-determined to win
...


# Introduction

The purpose of this assignment is to use Non-determinstic finite state automata and regular expressions as models of computing. To start with, you will be implementing several computations as Non-Deterministic Finite State Automata (NFAs). Next you'll be implementing computations with regular expressions.

# Exercise 5-1: Programming Problems

You have been provided with python/java code to simulate non-determinsitic finite state automata, and to convert regular expressions into finite state automata.

I hope that you at least glance through the programs delivered to you. Every component of these programs (except one) has been discussed in class, and was implemented using the same approach discussed in class. The `NFA` program implements the definition of NFAs discussed in class. The constructions for union, concatenation, and kleene star match the constructions we discussed in class. The procedure for constructing a NFA that's equivalent to a regex matches that procedure we discussed in class. The only complex thing done in the programs for this assignment that was never discussed in class is a procedure for "parsing" a regular expression so that we know which operations act on which sub-expressions. You don't need to understand how that works, but it could be "fun" for you to try to figure out how to do that on your own.


## Deliverable

Before you begin on this assignment, you will need to download two (or three) files, depending on your programming language of choice:

- Java: [NFA.java](/files/exercises/exercise5_java/NFA.java), [Tuple.java](/files/exercises/exercise5_java/Tuple.java), [Regex.java](/files/exercises/exercise5_java/Regex.java), and [Exercise5.java](/files/exercises/exercise5_java/Exercise5.java).
- Python: [NFA.py](/files/exercises/exercise5_python/NFA.py), [regex.py](/files/exercises/exercise5_python/regex.py), and [exercise5.py](/files/exercises/exercise5_python/exercise5.py)

The `NFA` program defines an NFA class (similar to the DFA class you had for exercise 4.1). The `regex` program defines a class that reads regular expressions and converts them to NFAs. The `exercise5` program contains example uses of the `NFA` and `regex` functionality, and also contains stubs for the functions you must implement.

The `Tuple` program (java only) pairs together a state and a character (these paired are the input type for the transition function), and makes the syntax for implementing transitions a bit nicer.

(**If you’re using java, do not add a package declaration to your program.**)

For this exercise you will be implementing four functions. The functions you are implementing are in the `exercise5` (either .py or .java) files, and only submit your `exercise5` file. You should not need to make any edits to any other files, and you will not submit it.

 In both the python and java code, to create a NFA you must define the 5 components we discussed in class:

- State set 
- alphabet set 
- starting state 
- set of final states 
- transition function 

The state set is a set of strings, the alphabet is a set of characters, the starting state is a string (that should be in your state set as well), the set of final states is a set of string (and should be a subset of the state set), and the transition function is a map/dictionary (it maps state-character tuples to sets of states). The state-character pairs are encapsulated by the `Tuple` class in java.

After you create an automaton, you will need to test and debug it on your own. I have given you some pretty powerful tools to be able to do this. If you have a NFA in your program called `nfa`:

- You can convert an automaton to a string describing it using `nfa.toString()` in Java, or `str(nfa)` in python. This will display to you everything you might want to know about the automaton (currently active state, start state, transitions, final states, etc.)
- You can use `nfa.step(character)` to transition on a single character. Its return value is a boolean representing whether or not there is a final state among the now-active states. You can use `nfa.active` to get the set of its currently active states.
- You can use `nfa.execute(string)` to run the machine on a given input string, its return value is a boolean representing whether or not there is a final state among the states that are active at the end.
- You can visualize the automaton by invoking `nfa.toDot()`. This method will print out a description of the automaton in the dot file format, which you can then convert into an image using an [online tool](https://dreampuf.github.io/GraphvizOnline/). To see your automaton, invoke `nfa.toDot()` and then copy-paste the printed text into the web tool.




### Huntingtons Disease

For the `huntingtons` function you're asked to implement, the idea is for you to use regular expressions to diagnose whether a person has Huntington's disease by looking at their genome.

A dna sequence is a string of the characters a, t, g, c, representing the sequence of nucleotides that comprise an individual's dna molecules. Very often, the human genome has regions where the same nucleotide sequences repeat many times. Sometimes, certain numbers of these repeats will result in a genetic disorder.
        
Huntington's Disease is caused by having too many consecutive copies of the sequence "cag". By looking at a dna sequence, we can categorize how a person might be affected by Huntington's in the following way:
        
- An individual with less than 26 sequential repeats of "cag" in their genome is considered to be "normal".
- An individual with between 26 and 35 repeats of "cag" is considered to be a "carrier", and may give the disease to their children.
- An individual with between 36 and 39 repeats is said to be "at risk", and may or may not ever show symptoms.
- An individual with 40 or more repeats is said to be "affected", and will eventually show symptoms of the disease.

Your `huntingtons` function should take a dna sequence (a string from the alphabet a,g,t,c) and determine the classification for the individual (i.e. normal, carrier, at risk, or affected). To do this, define a regex for each category, convert each to a nfa, then check which category the given dna sequence falls into. Once you have determined the category, the function should return the appropriate string of: "normal", "carrier", "at risk", or "affected"
        
Note that the dna sequence may have characters before/after the "cag" repeats.
            
[Source describing Huntingtons](https://en.wikipedia.org/wiki/Huntington%27s_disease).



# Exercise 5-2 Written problem.

Answer the problem contained in [this pdf](/files/exercises/exercise5.pdf) with an accompanying proof.

To begin, download [exercise5.zip](/files/exercises/exercise5.zip) and upload as a new project in overleaf. Within that zip you will see 2 tex files. the `exercise5.tex` file contains the code which generates the pdf, and `exercise5_2.tex` is where you will provide your answer.

First, change `\submitter{TODO: your name}` in `exercise5.tex` to contain your name and UVA email id (e.g. `\submitter{Grace Hopper (gmh1a)}`)

Next, cite all your sources in `\collaborators{TODO: replace ...}` according to the [course policy](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/syllabus.html#no-plagiarism-nor-anything-like-it)

At this point, fill in your solution in the tex file. When you rebuild the pdf, your solutions should appear as you write them.


## Deliverable

At the very top of `exercise5.tex` there is a line which reads `\usepackage{uvatoc}`. That line tells LaTeX include everything in the pdf. To include only your solution, comment that line out and uncomment `\usepackage[response2]{uvatoc}` to build a pdf with only exercise 5-2.

Rename the pdf file and submit to the [assignments page](https://kytos.cs.virginia.edu/cstheory).

