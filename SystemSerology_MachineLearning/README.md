# Machine learning for systems serology data

Workshop session #1 of the ["Systems Biology of Infectious Diseases" workshop (Feb 24-26, 2020)](https://cvisb.org/2020-workshop/)

## Goal
We will introduce a general machine learning workflow to deal with system serology datasets.

## Getting started
Before the workshop, please install the required programs and packages so that we can directly get started. In particular:

1. Install [R](https://cran.r-project.org/mirrors.html) and [RStudio](https://rstudio.com/products/rstudio/download/). If you use Mac OS, please follow the instructions found [here](https://www.r-bloggers.com/installing-r-on-os-x/) to install also XQuartz and Xcode. 

2. Install the following packages:
* pheatmap
* ggplot2
* DMwR
* ggpubr
* ropls
* glmnet
* RColorBrewer
* tidyverse
* corrr
* igraph
* ggraph
* ggrepel

```
install.packages(c("pheatmap", "ggplot2", "DMwR", "ggpubr", "glmnet", "RColorBrewer", 
                   "tidyverse", "corrr", "igraph", "ggraph", "ggrepel"))
```

The package ropls needs to be installed from Bioconductor using:

```
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("ropls")
```

If you are not or only little experienced with R, consider looking at general R workshops before, for example the ones that can be found here: https://github.com/nuitrcs/rworkshops. However, the hands-on exercises are offered in different versions to have a version for every experience level.

## Dataset

The data for this session is taken from the following publication: 

[Lu al., IFN-γ-independent immune markers of Mycobacterium tuberculosis exposure, Nature Medicine (2019)](https://www.nature.com/articles/s41591-019-0441-3)

To import the data and get a overview of the data, run the [Notebook part 1.](systemsSerology_part1.Rmd) 

## Workflow

The basic workflow for machine learning systems serology data includes feature selection using LASSO (Least Absolute Shrinkage and Selection Operator), followed by PLS-DA (partial least square discriminant analysis). 

There will be different version of the exercises for different programming skills (coming soon!). 



