---
title: "The Data Science Toolbox - Course Reflections"
author: "Asad Ali Shah"
date: "4/1/2020"
output: html_document
---

## What is the question?

Any data science project must start with a question. Hilary Parker's blog entry on [Is Hilary the most poisened baby name in the history?](https://hilaryparker.com/2013/01/30/hilary-the-most-poisoned-baby-name-in-us-history/) a great example to start with a question. 

This is how she orients the readers by putting the question upfront in bold:

> Is Hilary/Hillary really the most rapidly poisoned name in recorded American history? An analysis.

## Main types of questions

Questions can be broadly categorizes into the following six types:

- Descriptive
- Exploratory
- Inferential
- Predictive
- Causal
- Mechanistic


## RStudio

RStudio has four quardants named from top-left anticlock-wise:

1. Source
2. Console
3. Files, plots, packages, help
4. and lastly Environment


## R Packages

In my view, R Packages are what make R useful while at the same time overwhelming to learn. How can you decide which of the 100 ways of doing a thing is the right or best way to? Or at least this is how I justify my lack of progress in R so far :)

Anyway, the course provided a good introduction and highlighted ways to look a gorups of packages starting with the grouping on CRAN, called [Task View](https://cran.r-project.org/web/views/). 

### Install packages
Use `install.packages("ggplot2")` and to install multiple packages use install.packages(c("ggplot2", "devtools", "dplyr").

### Load packages
Think of `install.packages` as installing a software. To use that software, you have to open it. `library(package)` is the software equivilant of opening for R packages. Note that in this case, no quotes are required.

### Update packages
Use `update.packages()` to update all the old packages. As a side note, to check what packages are installed, use `installed.packages()` or `library()`. 

### Remove packages
Use `remove.packages("name")`.

Some other useful functions include:
- `version` to check the version of R
- `sessionInfo()` a replacement of `version`
- `help()` for general help of `help("ggplot2")` for help of `ggplot2`
- `browseVignettes()` for all vignettes or `browseVignettes("ggplot2")` for `ggplot2` vignettes


## R Projects
R Projects are like Project folders within which you should have three more folders as follows:

1. Data
2. Scripts
3. Output

A repository in GitHub creates a project and a folder with the same name in the computer.


## GitHub, Git and RStudio

Create a GitHub account. 

To link it with the machine (and RStudio), install Git on your machine. Do not confuse Git with GitHub Desktop. 

Here is the sequence once Git is installed.

1. Add your email to Git using `git config` commands. Email has to be the same as the one used for GitHub account creation. User name can be different.
2. Find the path of `git.exe` and add it to RStudio: Tools > Global Options > Git/SVN
3. Take the SVN key and add it to your GitHub Account: Profile > Settings > SSH and GGP keys

Restart RStudio. Now RStudio should be linked with GitHub. Open a repository in GitHub. Copy URL. Add it to RStudio: File > New Project > ... Open a file in GitHub and you will immediately see in RStudio.