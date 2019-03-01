
[![Travis-CI Build
Status](https://travis-ci.org/hrbrmstr/cruxjars.svg?branch=master)](https://travis-ci.org/hrbrmstr/cruxjars)
[![Coverage
Status](https://codecov.io/gh/hrbrmstr/cruxjars/branch/master/graph/badge.svg)](https://codecov.io/gh/hrbrmstr/cruxjars)
[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/cruxjars)](https://cran.r-project.org/package=cruxjars)

# cruxjars

Java Archive Wrapper Supporting the ‘crux’ Package

## Description

Contents of the ‘crux’ & supporting Java archives
<https://github.com/chimbori/crux>.Version number reflects the version
number of the included ‘JAR’ file.

## What’s Inside The Tin

The following functions are implemented:

## Installation

``` r
devtools::install_git("https://sr.ht.com/~hrbrmstr/cruxjars.git")
# or
devtools::install_git("https://gitlab.com/hrbrmstr/cruxjars.git")
# or (if you must)
devtools::install_github("hrbrmstr/cruxjars")
```

## Usage

``` r
library(cruxjars)

# current version
packageVersion("cruxjars")
## [1] '2.0.2'
```

## cruxjars Metrics

| Lang  | \# Files | (%) | LoC |  (%) | Blank lines |  (%) | \# Lines |  (%) |
| :---- | -------: | --: | --: | ---: | ----------: | ---: | -------: | ---: |
| Java  |        2 | 0.2 |  28 | 0.36 |           5 | 0.18 |       18 | 0.21 |
| Maven |        1 | 0.1 |  17 | 0.22 |           0 | 0.00 |        1 | 0.01 |
| R     |        5 | 0.5 |  15 | 0.19 |           2 | 0.07 |       32 | 0.38 |
| make  |        1 | 0.1 |  10 | 0.13 |           4 | 0.14 |        0 | 0.00 |
| Rmd   |        1 | 0.1 |   8 | 0.10 |          17 | 0.61 |       33 | 0.39 |

## Code of Conduct

Please note that this project is released with a [Contributor Code of
Conduct](CONDUCT.md). By participating in this project you agree to
abide by its terms.
