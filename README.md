EMMLi: A Maximum Likelihood Approach To The Analysis Of Modularity
====================================================================

[![Build Status](https://travis-ci.org/timcdlucas/EMMLi.svg)](https://travis-ci.org/timcdlucas/EMMLi)
[![codecov.io](https://codecov.io/github/timcdlucas/EMMLi/coverage.svg?branch=master)](https://codecov.io/github/timcdlucas/EMMLi?branch=master)
[![cran version](http://www.r-pkg.org/badges/version/EMMLi)](https://cran.rstudio.com/web/packages/EMMLi) 

An R package for performing analyses of modularity on morphological landmark data.

The only function is `EMMLi` which takes a correlation matrix and a data frame that describes a number of modular models.

A. Goswami and J. Finarelli (2016) EMMLi: A maximum likelihood approach to the analysis of modularity.
Evolution [http://onlinelibrary.wiley.com/doi/10.1111/evo.12956/abstract](http://onlinelibrary.wiley.com/doi/10.1111/evo.12956/abstract)




Installation
--------------

To install the CRAN version

```r

install.packages('EMMLi')
```

or to install the development version from GitHub

```r
library(devtools)
install_github('timcdlucas/EMMLi')
```




Basic usage
------------

The package contains one function, `EMMLi`.
This function takes a correlation matrix, a data frame defining a set of models (which landmarks are part of which module) and the sample size (number of specimens).

```r
# An example correlation matrix
dim(macacaCorrel)

# An example data frame that defines the models
head(macacaModels)

# Run EMMLi
output <- EMMLi(macacaCorrel, 20, macacaModels)
```
