# Comparing the exponential distribution in R with the Central Limit Theorem
Alexander Pyle, <apyle@github.com>  
November 8, 2015  

 A sample set of headings that could be used to guide the creation of your report might be:

    Title (give an appropriate title) and Author Name
    Overview: In a few (2-3) sentences explain what is going to be reported on.
    Simulations: Include English explanations of the simulations you ran, with the accompanying R code. Your explanations should make clear what the R code accomplishes.
    Sample Mean versus Theoretical Mean: Include figures with titles. In the figures, highlight the means you are comparing. Include text that explains the figures and what is shown on them, and provides appropriate numbers.
    Sample Variance versus Theoretical Variance: Include figures (output from R) with titles. Highlight the variances you are comparing. Include text that explains your understanding of the differences of the variances.
    Distribution: Via figures and text, explain how one can tell the distribution is approximately normal. 
    


```r
# The following code might come in handy once I start actually working on the project ;-)

hist(runif(1000))
```

![](PA1_files/figure-html/unnamed-chunk-1-1.png) 

```r
mns = NULL
for (i in 1 : 1000) mns = c(mns, mean(runif(40)))
hist(mns)
```

![](PA1_files/figure-html/unnamed-chunk-1-2.png) 

```r
# nosim <- 1000
# cfunc <- function(x, n) sqrt(n) * (mean(x) - 0.9) / sqrt(.1 * .9)
# dat <- data.frame(
#         x = c(apply(matrix(sample(0:1, prob = c(.1,.9), nosim * 10, replace = TRUE), 
#                            nosim), 1, cfunc, 10),
#               apply(matrix(sample(0:1, prob = c(.1,.9), nosim * 30, replace = TRUE), 
#                            nosim), 1, cfunc, 30),
#               apply(matrix(sample(0:1, prob = c(.1,.9), nosim * 50, replace = TRUE), 
#                            nosim), 1, cfunc, 50)
#         ),
#         size = factor(rep(c(10, 30, 50), rep(nosim, 3))))
# g <- ggplot(dat, aes(x = x, fill = size)) + geom_histogram(binwidth=.3, colour = "black", aes(y = ..density..)) 
# g <- g + stat_function(fun = dnorm, size = 2)
# g + facet_grid(. ~ size)
```

