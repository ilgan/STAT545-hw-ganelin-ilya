HW7
================
iganelin
2017-11-14

Homework 07: Data wrangling wrap up (Due date 10/11/17)
=======================================================

### Loading libraries

``` r
library(gapminder)
library(singer)
library(tidyverse)
library(knitr)
library(forcats)
library(magrittr)
library(dplyr)
library(meme)
library(readr)
library(tidyr)
library(stringr)
library(ggplot2)
library(downloader)
```

Firstly, we will download the picture to the main folder and create a meme

``` r
download.file(url = "http://www.happyfamilyneeds.com/wp-content/uploads/2017/08/angry8.jpg", destfile = "angry8.jpg", mode="wb")
u <- "angry8.jpg"
mmplot(u) + mm_caption("Homework 7", "Yes! Give me more!", color="purple")
```

![](HW7_files/figure-markdown_github-ascii_identifiers/unnamed-chunk-2-1.png)

Big picture
-----------

##### Write (or extract from a previous analysis) three or more R scripts to carry out a small data analysis.

##### The output of the first script must be the input of the second, and so on.

##### Something like this:

-   First script: download some data: [1\_download\_wind\_data.r](https://github.com/ilgan/STAT545-hw-ganelin-ilya/blob/master/HW7/1_download_wind_data.r)
-   Second script: read the data, perform some analysis and write numerical data to file in CSV or TSV forma: [2\_clean\_wind\_data.r](https://github.com/ilgan/STAT545-hw-ganelin-ilya/blob/master/HW7/2_clean_wind_data.r)
-   Third script: read the output of the second script, generate some figures and save them to files: [3\_plot\_wind\_data.rmd](https://github.com/ilgan/STAT545-hw-ganelin-ilya/blob/master/HW7/3_plot_wind_data.rmd)
-   Fourth script: an Rmd, actually, that presents original data, the statistical summaries, and/or the figures in a little report: [4\_wind\_data.rmd](https://github.com/ilgan/STAT545-hw-ganelin-ilya/blob/master/HW7/4_wind_data.rmd)
-   A fifth script to rule them all, i.e. to run the others in sequence: [Makefile](https://github.com/ilgan/STAT545-hw-ganelin-ilya/blob/master/HW7/Makefile)

#### Output Files from the pipeline

-   Media files are [here](https://github.com/ilgan/STAT545-hw-ganelin-ilya/tree/master/HW7/media)
