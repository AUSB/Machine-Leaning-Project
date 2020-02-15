# Machine-leaning-project

A project using Python to implement linear least squares regression to compare Empirical risk minimization (ERM) and Regularized least squares regression (RLM)

Step 1 - load the data
The data is stored in two files, dataset1_inputs.txt and dataset1_outputs.txt
which contain the input values (i.e., values xi) and the target values (i.e., values ti)
respectively. These files are simple text files which can be loaded with the load function
in Matlab/Octave. Plot the outputs as a function of the inputs (ie plot the datapoints,
not a curve) and include this plot in your write-up.


Step 2 - ERM
For degrees W = 1, . . . 20, fit a polynomial of degree W to the data using (unregularized) least squares regression. For each learned function, compute the empirical square
loss on the data and plot it as a function of W. Include this plot in your report. Which
value of W do you think would be suitable?


Step 3 - RLM
Repeat the previous step using regularized least squares polynomial regression. Each
time train polynomial of degree 20 for regularization parameters λ so that ln(λ) =
−1, −2, · · · − 20. This time plot (and include) the empirical loss as a function of i.
Compare and discuss the two curves you get for ERM and RLM.


Step 4 - cross validation
Implement 10-fold cross validation for ERM. That is, randomly divide that data into
10 chunks of equal size. Then train a model on 9 chunks and test on the 10th that
was not used for training. For each model you train, average the 10 test scores you
got and plot these again as a function of W. Which value of W do you think would be suitable
