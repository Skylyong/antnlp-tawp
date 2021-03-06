# A Template for Academic Writing Projects

The repository contains a template for writing NLP/ML papers (using latex).
By no mean one could write great articles by filling a template,
but we hope this project could help less experienced researchers
to grasp key aspects of an academic paper.

In the template, we try to give a detailed todo list for each paper section 
(see texts in `docs/antnlp-tawp.pdf`),
a workflow for a new writing project,
and a flavor of using latex.

## As a Template Repository

We suggest using github repos to manage tex files. 
To start your own projects from this template, click `Use this template` (see [creating a repo from a template](https://help.github.com/en/articles/creating-a-repository-from-a-template)).


## Files and Directories

Suppose your project's name is "antnlp-tawp".
- `antnlp-tawp/docs`: latex source files for the main paper. We use `\input` commands in the main tex file `antnlp-tawp.tex` 
to facilitate collaborative writing.
- `antnlp-tawp/images`: images (prefer pdf format) used in the paper. You may have nested directories 
if some images are generated by other programs (e.g., source codes of matplotlib).
- `antnlp-tawp/supplementary`: latex source files for the supplementary.

Instead of "fig1.pdf, fig2.pdf, paper.tex, my-paper.tex",
please files with clear meaning (e.g., "pr-curve.pdf", "inorder-dep-parsing.tex").


## A Workflow

When you start a new paper, we suggest going with the following steps
1. list motivations (e.g., problem importance/challenges) in the _introduction_ section. 
It helps you to build a complete picture of the paper. 
1. list experiments.
1. draw the key figures of your model. It helps you to organize the _approach_ section.
1. the _approach_ section.
1. the _introduction_ section and the _abstract_.
1. the _experiments_ section.
1. the _related work_ section.
1. the _conclusion_.

The writing should start at least 1 month ahead of deadlines.

## Other Suggestions

- latex software: texlive. To be friendly to unicodes, we recommend compiling with xelatex. 
- latex source files
    - add a line break for each sentence (clauses, or long phrases). 
      Don't worry about the formatting, unless you adding an empty line, 
      latex automatically wraps them into one paragraph in the final pdf file. 
      Short sentences are prefered both for experssing ideas and reviewing.
- latex packages
    - equations: `IEEEeqnarray` package 
    - tables: avoid vertical lines. Usually, `\toprule`, `\midrule` and `\bottomrule` are  enough.
- figures
    - make sure to include vector graphics (pdf(recommended), eps, svg) in your final paper, rather than jpg, png, bmp.
    - to crop blank margin of a pdf, try `pdfcrop` in texlive.
    - figures with latex symbols and equations
        - Mac: keynote + LaTeXiT
        - Windows: ppt + kLatexFormula
        - Linux: wps+`images/latex2emf.py` (a linux version of  kLatexFormula is available.
          However, the current version of linux wps can not directly import emf file from clipboard.
          We still need to do the importing job manually.)
    - or you can try matplotlib (be sure that ticklabels, annotations, legend, etc 
     are in proper font size (the default setting is usually too small))
    - even tikz (use additional .tkz file to place your tikz figure source file, rather than in the main tex)

