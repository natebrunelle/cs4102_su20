---
title: PA0 Getting Started
...

This "programming assignment" is intended to help you to get set up with the tools you'll need for the coming semester, namely: Java, Python, and LaTeX (Overleaf). Unlike with all future programming assignments, you will not actually be asked to submit a program. Instead, you will be asked to submit a pdf generated with LaTeX.

# Setting up your programming Environment

To set up your Java or Python3 programming environments, follow [this guide](https://www.cs.virginia.edu/~njb2b/cs3100/s2023/installing.html).

# Getting Started with LaTeX
LaTeX is essentially a programming language for documents. It’s the most powerful and widely-used tool for producing highly-readable documents with combinations of code, pseudo-code, mathematics, figures, etc. We will be using it for all written assignments this semester.

## Register for Overleaf
While you’re welcome to use any LaTeX tool that you’d like, we highly recommend using Overleaf. To use this tool, first visit https://www.overleaf.com and register an account (if you don’t already have one). UVA has a site license, so if you register with your @virginia.edu email address you will have full access to all the Overleaf features for free.

## Set Up Your Project
You will have a separate Overleaf project for each exercise. The easiest way to set up the repository is to upload the zip file posted with each exercise. To do this:

1. Download the ps0.zip file 
2. In Overleaf, click on Create First Project or New Project and select Upload Project from the menu.
3. Select the exercise0.zip file you downloaded in step 1.

## Editing The LaTeX Template
1. Look for the line, submitter{TODO: your name} and replace the TODO: your name with your name and UVA id: submitter{Nathan Brunelle (njb2b)}
1. List your collaborators and resources, replacing the TODO in collaborators{TODO: replace …} with your collaborators and resources. (Remember to update this before submitting if you work with more people.)
1. Replace the line, usepackage{algo} (the second line in the file) with usepackage[response]{algo}. You can do this by using the LaTeX comment token, %. The rest of the line after a % is treated as a comment.
1. Then, try rebuilding the PDF by clicking Recompile. You should see a file that includes your name and collaborators, but with all the directions removed (we don’t want to see these in your submission).

## Deliverable
- Modify the ps0.tex file to complete each problem. To see an example of what your submission might look like, see this pdf. You should reproduce the proof seen there for problem 2.
- Learn how to include drawings in your documents with the includegraphics{file} command by including a caricature of Nathan Brunelle (or some other image) in the same pdf. Make sure the entire image fits on a single page. You may need to resize the image.
- Submit the generated **pdf** (NOT a .tex or .zip file) to Gradescipe.
