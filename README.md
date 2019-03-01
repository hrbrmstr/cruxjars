
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

## Installation

``` r
install.packages(c("cruxjars", "crux"), repos = "https://cinc.rud.is/")
```

## Usage

``` r
library(cruxjars)
library(crux)

# current version
packageVersion("crux")
## [1] '0.1.0'
```

``` r
str(
  summarise_url("http://time.com/5541738/joe-biden-backtracks-pence-praise-criticism/"), 1
)
## List of 14
##  $ url          : chr "http://time.com/5541738/joe-biden-backtracks-pence-praise-criticism/"
##  $ original_url : chr NA
##  $ title        : chr "Joe Biden Backtracks After Calling Pence 'a Decent Guy'"
##  $ description  : chr "The former Vice President took back his comment that Pence is \"a decent guy\" after fellow Democrats denounced his remarks"
##  $ site_name    : chr "Time"
##  $ theme_color  : chr NA
##  $ amp_url      : chr "http://amp.timeinc.net/time/5541738/joe-biden-backtracks-pence-praise-criticism"
##  $ canonical_url: chr "http://time.com/5541738/joe-biden-backtracks-pence-praise-criticism/"
##  $ image_url    : chr "http://timedotcom.files.wordpress.com/2019/03/ap19059832629402.jpg?quality=85&crop=0px%2C111px%2C6000px%2C3000p"| __truncated__
##  $ video_url    : chr NA
##  $ feed_url     : chr NA
##  $ favicon_url  : chr "http://time.com/img/favicons/favicon-192.png"
##  $ reading_time : int 2
##  $ text         : chr "(OMAHA, Neb.) — Former Vice President Joe Biden’s tendency to talk about his good relationships with Republican"| __truncated__
```

``` r
str(
  classify_url("https://www.washingtonpost.com/powerpost/house-democrats-explode-in-recriminations-as-liberals-lash-out-at-moderates/2019/02/28/c3d163fe-3b87-11e9-a06c-3ec8ed509d15_story.html")
)
## Classes 'tbl_df', 'tbl' and 'data.frame':    1 obs. of  10 variables:
##  $ url                 : chr "https://www.washingtonpost.com/powerpost/house-democrats-explode-in-recriminations-as-liberals-lash-out-at-mode"| __truncated__
##  $ is_ad_image         : logi FALSE
##  $ is_web_scheme       : logi TRUE
##  $ is_likely_article   : logi TRUE
##  $ is_likely_video     : logi FALSE
##  $ is_likely_audio     : logi FALSE
##  $ is_likely_binary_doc: logi FALSE
##  $ is_likely_archive   : logi FALSE
##  $ is_likely_executable: logi FALSE
##  $ is_likely_image     : logi FALSE
```

## crux Metrics

| Lang  | \# Files |  (%) | LoC |  (%) | Blank lines |  (%) | \# Lines |  (%) |
| :---- | -------: | ---: | --: | ---: | ----------: | ---: | -------: | ---: |
| HTML  |        1 | 0.08 | 691 | 0.87 |           8 | 0.18 |        0 | 0.00 |
| make  |        2 | 0.17 |  30 | 0.04 |          13 | 0.29 |        0 | 0.00 |
| Java  |        2 | 0.17 |  28 | 0.04 |           5 | 0.11 |       18 | 0.21 |
| Maven |        1 | 0.08 |  17 | 0.02 |           0 | 0.00 |        1 | 0.01 |
| R     |        5 | 0.42 |  15 | 0.02 |           2 | 0.04 |       32 | 0.38 |
| Rmd   |        1 | 0.08 |  13 | 0.02 |          17 | 0.38 |       33 | 0.39 |

## Code of Conduct

Please note that this project is released with a [Contributor Code of
Conduct](CONDUCT.md). By participating in this project you agree to
abide by its terms.
