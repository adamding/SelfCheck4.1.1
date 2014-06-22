---
title       : Self-Check Questions (ungraded)
subtitle    : Random sampling from distributions
author      : Aidong Adam Ding
job         : Made using Slidify in R. (Click mouse then right arrow key for next slide.)
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : solarized_dark      # 
widgets     : [mathjax, quiz, bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- &submitcompare1
## Generate random samples from a distribution
Write the R command that sample 500 values randomly form the Chi-square distribution with 7 degrees of freedom, and store in variable y.

*** .hint
To generate data from the distribution, using the routines start with "r". 

*** .explanation
y \<- rchisq(500, df=7)

--- &submitcompare1
## Generate random samples from a distribution
Write the R command that sample 30 values randomly form the t-distribution with 1 degrees of freedom.

*** .hint
To generate data from the distribution, using the routines start with "r". 

*** .explanation
rt(30,df=1)

--- &submitcompare1
## Generate random samples from a distribution
Write a the R script that does the following three tasks:

(1) Randomly sample 60 values form the normal distribution with mean=1 and variance=5, and store to x.

(2) Draws the histogram of these 60 values.

(3) Add the normal density curve, of mean=1 and variance=5, to the histogram.

*** .hint
To generate data from the distribution, using the routines start with "r". 

*** .explanation
x<-rnorm(60, mean=1, sd=sqrt(5))

hist(x, freq=F)

curve(dnorm(x, mean=1, sd=sqrt(5)), add=T)





