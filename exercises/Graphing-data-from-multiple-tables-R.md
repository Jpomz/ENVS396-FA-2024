---
layout: exercise
topic: Graphing
title: Graphing Data From Multiple Tables
language: R
---

An experiment in Kenya has been exploring the influence of large herbivores on plants.

Check to see if `ACACIA_DREPANOLOBIUM_SURVEY.txt` and `TREE_SURVEYS.txt` are in your `data` folder. 
If not, download [`ACACIA_DREPANOLOBIUM_SURVEY.txt`](https://esapubs.org/archive/ecol/E095/064/ACACIA_DREPANOLOBIUM_SURVEY.txt) and [`TREE_SURVEYS.txt`](https://ndownloader.figshare.com/files/5629536)
Use `read_tsv` to read in the data using the following commands:

```r
acacia <- read.csv("data/ACACIA_DREPANOLOBIUM_SURVEY.txt",
                    sep="\t",
                    na.strings = c("dead"))
trees <- read_tsv("data/TREE_SURVEYS.txt",
```

We want to compare the circumference to height relationship in acacia and to the same relationship for trees in the region. These data are stored in two different tables. Make a graph with the relationship between `CIRC` and `HEIGHT` for the trees as gray circles in the background and the same relationship for acacia as red circles plotted on top of the grah circles. Scale the both axes logarithmically. Inlude linear models for both sets of data. Provide clear labels for the axes.