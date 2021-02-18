# Brief Summary :

## Task :

Plot 10 samples from the posterior distribution estimated in previous tutorial 

## How I implemented it in short :

1) Here , in pick_10_lines the passed values of m0,s0,Beta(mean and variance of prior grid, precision in noise added to true data) and calculated mn,sn(mean and variance of posterior distribution) and for next iteration I needed to make m0=mn and s0=sn (Because next time the posterior grid will become my prior)
2) In pick_10_lines after getting mn,sn (mean & covariance) of Posterior Gausian distribution , I have made use of library function to generate 10 (w0,w1) points

## Output :

[!plot1](https://github.com/Yashprime1/IIIT-Dharwad-ML-Tutorial---By-Dr.-Arun-Chauhan-/blob/main/Arun%20Sir/Tutorial-4/Bayesian_Regression.png?raw=true)
[!plot2](https://github.com/Yashprime1/IIIT-Dharwad-ML-Tutorial---By-Dr.-Arun-Chauhan-/blob/main/Arun%20Sir/Tutorial-4/10_points.png?raw=true)

