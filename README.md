# StatInfer_PeerAssessment1
Coursera Statistical Inference Class, Peer Assessment Project #1

This exercise is asking you to use your knowledge of the theory given in class 
to relate two distributions.  

In this project you will investigate the exponential distribution in R and 
compare it with the Central Limit Theorem. The exponential distribution can be 
simulated in R with `rexp(n, lambda)` where lambda is the rate parameter. The 
mean of exponential distribution is 1/lambda and the standard deviation is also 
1/lambda. Set `lambda = 0.2` for all of the simulations. You will investigate 
the distribution of averages of 40 exponentials. Note that you will need to do 
a thousand simulations.

Illustrate via simulation and associated explanatory text the properties of the 
distribution of the mean of 40 exponentials.  You should

1. Show the sample mean and compare it to the theoretical mean of the distribution.
2. Show how variable the sample is (via variance) and compare it to the theoretical 
variance of the distribution.
3. Show that the distribution is approximately normal.

In point 3, focus on the difference between the distribution of a large collection 
of random exponentials and the distribution of a large collection of averages of 
40 exponentials. 

The report should be no more than 3 pages with 3 pages of supporting appendix 
material if needed (code, figures, etcetera). 
