---
title: Exercise 0 Getting Started
...



# Exercise 0-1: Onboarding

## Course Pledge

Read the [course pledge](pledge.html). If there are any items therein that you would like to discuss, do not hesitate to meet with Nathan Brunelle.

## Course Registration Survey

Read Jeremy Kun's ["Habits of Highly Mathematical People"](https://medium.com/@jeremyjkun/habits-of-highly-mathematical-people-b719df12d15e) and complete [this survey](https://docs.google.com/forms/d/e/1FAIpQLSeachrnhASxThVUp-A3LQPPYGsE8Zfo8e-FyRFnjFAUt9YK-Q/viewform?usp=sf_link)

## Deliverable

Your only deliverable for Exercise 0-1 is to complete the survey.

# Exercise 0-2: Getting Started with LaTeX

For the assignments in this class, you will be required to submit your responses as PDF files typeset with LaTeX[^future], a professional formatting system that is used in most serious mathematical typesetting, which is a set of libraries built on the TeX typesetting language developed by Donald Knuth.
If you haven’t used LaTeX before, there is a bit of a learning curve to using it, but you will find the ability it gives you to efficiently produce beautiful and complex documents to be a valuable life-long skill. We recommend using Overleaf, an in-browser collaborative editor for LaTeX.

[^future]:To Quote Leslie Lamport (the creator LaTeX) "One of the hardest things about LaTeX is deciding how to pronounce it. This is also one of the few things I'm not going to tell you about LaTeX, since pronunciation is best determined by usage, not fiat. TeX is usually pronounced teck, making lah-teck, and lay-teck the logical choices; but language is not always logical, so lay-tecks is also possible."

## Register for Overleaf

Visit [https://www.overleaf.com](https://www.overleaf.com) and register for an Overleaf account (if you don’t already have one). UVA has a site license to Overleaf, so if you register with your @virginia.edu email address you will have full access to all the Overleaf features for free.

## Set Up Your Repository

Create your own copy of the Exercise 0-2 repository by following these steps:

1. Download the *Exercise 0-2* template from: [https://www.cs.virginia.edu/~njb2b/cstheory/s2020/exercises/exercise0_2.zip](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/files/exercises/exercise0_2.zip)
1. In Overleaf, click on *Create First Project* or *New Project in Overleaf* and select *Upload Project* from the menu.
1. Click *Select a .zip file* then select *exercise0_2.zip* you downloaded in step 1

## Editing exercise0_2.tex

1. Look for the line, *submitter{TODO: your name}* and replace the TODO: your name with your name and UVA id: *submitter{Nathan Brunelle (njb2b)}*
1. List your collaborators and resources, replacing the TODO in *collaborators{TODO: replace ...}* with your collaborators and resources. (Remember to update this before submitting if you work with more people.)
1. Replace the line, *usepackage{uvatoc}* (the second line in the file) with *usepackage[response]{uvatoc}*. You can do this by using the LaTeX comment token, %. The rest of the line after a % is treated as a comment.
1. Then, try rebuilding the PDF by clicking *Recompile*. You should see a file that includes your name and collaborators, but with all the directions removed (we don’t want to see these again in your submission).

## Deliverable

- Modify the [exercise0_2.tex](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/files/exercises/exercise0_2.zip) file to reproduce the proof seen in [this pdf](https://www.cs.virginia.edu/~njb2b/cstheory/s2020/files/exercises/exercise0_2_target.pdf). 
- Learn how to include drawings in your documents with the *includegraphics{file}* command by including a caricature of Nathan Brunelle in the same pdf.
- Submit the generated pdf on [the kytos submission system](https://kytos.cs.virginia.edu/cstheory/task.php?task=exercise0_2). Name it *exercise0_2.pdf*.


# Exercise 0-3: Programming

This semester you will be able to use either Java or Python (your choice) for the programming exercises. This exercise is for you to get your programming environment set up and to complete a couple of (hopefully) easy programming tasks.

You're only required to install one of Java or Python (you do not need to install both).

## Java

If you already/still have a Java JDK installed on your machine from CS2110, you're likely good to go! If not, follow the procedure below according to the OS you're using.

### Windows

To install on windows, I recommend [this super helpful video](https://www.youtube.com/watch?v=RFk653ilyhA) made by our very own Professor Will McBurney of CS2110 fame.

### Mac

To install Java JDK on a Mac, follow this procedure:

1. Go to http://jdk.java.net in a web browser

1. Click on jdk13

1. Select the correct download for your operating system

1. Once that file is downloaded, extract the zip or tar.gz file into /Library/Java/JavaVirtualMachines/

5) Remember where you extract the folder, as you will need it soon.

### Eclipse

If you would like to use Eclipse as your IDE (any IDE suffices):

1. Go to http://eclipse.org

1. Click on download in the top right.

1. Download Eclipse IDE 2019-12

1. When finished download, attempt to run the file. It will ask for a Java VM. The window should say something like: “The required 64-bit Java 1.8.0 virtual machine could not be found. Do you want to browse your system for it?”

1. Click “Yes” on that window.

1. Navigate to where you stored the openjdk-13.0.2_windows-x64-bin folder from the installing OpenJDK step. Go into that folder, then into the folder “bin”, and select javaw.exe

---On Mac, the you will want to link to jdk-13.0.2.jdk/Contents/Home/bin

------Also, check your Library folder -> /Library/Java/JavaVirtualMachines/jdkX.Y.Z.jdk/ (where X Y and Z are version numbers) for a Contents/Home/bin if the above address doesn't work

1. At this point, Eclipse will install. Accept all license agreements.

## Python 3

If you already have python 3 installed on your machine (perhaps from CS1110), then you're likely good to go. If not, I recommend following the procedure available on the [cs1110 webpage](https://cs1110.cs.virginia.edu/lab01-installing.html). You can skip any steps involving PyGame or sdl.

## Deliverable

Before completing this portion of the assignment, download either [mset.java](/files/exercises/exercise0_3_java/mset.java) or [mset.py](/files/exercises/exercise0_3_python/mset.py) depending on which programming language you prefer to use. Do ctrl+f and search for "TODO" to find all places where you must fill in code. Please do not change any code you're not instructed to change. (If you're using java, do not add a package to your program.)

Python and Java already provide built-in set datatypes, which is what you should use if you want to use sets in a real problem. But, for understanding purposes, we are going to define our own set datatype which we will call mset to avoid confusion with built-in sets. Our goal is to match as closely as possible the definition of a mathematical set, as given in the textbook. 

Follow the instructions in the program you downloaded (follow them line-by-line in python, follow the numbers in order in Java). Submit the completed mset file. Your code will receive full credit provided you followed the instructions and, when run, the printed output has exclusively encouraging messages (and has no errors).





