# Brief Summary :

## Task :

Plot Figure 3.7 from PRML using your preferable language. Use line of intercept = -0.3 and slope =0.5 with gaussian noise (mean =0; var = 0.04) to generate 10 sample points (x_i, y_i) between -1 and +1 on x axis. For more details refer respective video lecture and PRML.
Hint: You can define 2 dimensional grid uniformly between -1 and +1 on x-aix and y-axis respectively. Then calculate the probability of Gaussian for given mean and variance using library functions. Calculate the un-normalized posterior by multiplying (one-to-one) prior and likelihood grids; hence results in the same dimensional grid with posterior probability. Use heat map to plot the figure. Prior is gaussian distribution with mean = 0 and var = 0.5.

## How I implemented it in short :

1) First made a line with 10 points with Gausian noise and without gausian noise(true function)
2) Then made 3 functions for likelihood grid , prior grid , posterior grid calculation. 
3) Later a driver code which will plot the curves
4) In driver code , I made a loop for 10 data points generated in step 1 and calculated likelihood grid for each new point added and then multiplied it with prior grid to generate posterior grid and then changed my new posterior grid to prior to act as a prior for next point.
5) Now to plot the 3rd Column in the given 3.7 figure , I needed to pick (w0,w1) points from posterior distribution randomly so I calculated the mean and variance of that seperately in a function called pick_10_lines.


## Output :

[!plot](https://github.com/Yashprime1/ML-Tutorial---By-Dr.-Arun-Chauhan-/blob/main/Arun%20Sir/Tutorial-2/tutorial-2.png?raw=true)
