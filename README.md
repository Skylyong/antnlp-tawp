# A Template for Academic Writing Projects

The repository contains a template for writing NLP/ML papers (using latex).
By no mean one could write great articles by filling a template,
but we hope this project could help less experienced researchers
to grasp key aspects of an academic paper.

In the template, we try to give a detailed todo list for each paper section 
(see texts in `docs/antnlp-tawp.pdf`),
a workflow for a new writing project,
and a flavor of using latex.


## Files and Directories

Suppose your project's name is "antnlp-tawp".
- `antnlp-tawp/docs`: your latex source files. We use `\input` commands in the main tex file `antnlp-tawp.tex` 
to facilitate collaborative writing.
- `antnlp-tawp/images`: the images (prefer pdf format) used in your project. You may have nested directories 
if some images are generated by other programs (e.g., source codes of matplotlib).
- `antnlp-tawp/supplementary`: your latex source files for the supplementary.

Instead of "fig1.pdf, fig2.pdf, paper.tex, my-paper.tex",
we suggest naming files with clear meaning (e.g., "pr-curve.pdf", "inorder-dep-parsing.tex").


## A Workflow

When you start a new paper, we suggest going with the following steps
1. list the motivations (e.g., problem importance/challenges) in the _introduction_ section. 
It helps you to build a complete picture of your paper. 
1. list experiments.
1. draw the key figures of your model. It helps you to organize the _approach_ section.
1. the _approach_ section.
1. the _introduction_ section and the _abstract_.
1. the _experiments_ section.
1. the _related work_ section.
1. the _conclusion_.

The workflow should starts at least 1 month before your deadline.

## Other Suggestions

- latex software: texlive. To be friendly to unicodes, we recommend compiling with xelatex. 
- use git
- latex packages
    - .tex files: add a line break for each sentence (or clauses and long phrases).  Don't worry about the formatting, unless you adding an empty line, latex will automatically wrap them into one paragraph in the compiled pdf. Short sentences are prefered both for experssing your idea and review.
    - equations: `IEEEeqnarray` package 
    - tables: avoid vertical lines. Usually, `\toprule`, `\midrule` and `\bottomrule` are  enough.
- figures
    - Mac: keynote + LaTeXiT
    - Windows: ppt + kLatexFormula
    - Linux: wps+`images/latex2emf.py` (a linux version of  kLatexFormula is available.
      However, the current version of linux wps can not directly import emf file from clipboard.
      We still need to do the importing job manually.)

