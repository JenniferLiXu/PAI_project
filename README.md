# PAItask

Projects for successful completion of the course Probabilistic Artifical Intelligence led by Prof. Andreas Krause at ETH Zurich, 2021. Partial code skeletons were provided and core logic and algorithms were implemented by the students. Evaluation was performed on black-box test data in a fixed environment, with a pass for successfully beating the performance baselines.


##Project0
Exact bayesian inference outputting posterior probabilities, given fixed prior probabilities for sampling from three known distributions :Normal, Laplace, student.

Baseline evaluation: Hellinger distance for posterior inference on 50 random datasets sampled from the DGP.

##Project1 GAUSSIAN PROCESS REGRESSION
Gaussian Process regression to model air pollution and predict fine particle concentration at new coordinate locations.
use: model selection, GP inference complexity O(n3) and asymmetric cost handling.

Method #1 (scikit-learn): GP regressor with optimal kernel selection via custom k-fold CV, K-means clustering to reduce sample size, custom prediction adjustment to adapt to asymmetric costs.
Method #2 (gpytorch): GP regressor with structured kernel interpolation, custom prediction adjustment to adapt to asymmetric costs.

##Project2 BAYESIAN NEURAL NETS 
Bayesian neural network implementation based on the ’Bayes by Backprop’ algorithm. for multi-class classification on the MNIST dataset. The test set contains added uncertainty via pixelation and random rotations. Additional calibration measurements of predictions

algorithm implementation, weight prior and variational posterior selection, calibration considerations.

##Project3 BAYESIAN OPTIMIZATION
Implementation of Bayesian optimization under constraints to the feasible domain (2D grid)
joint training of constraint and objective, acquisition function choice, constraint satisfaction.

##Project4 REINFORCEMENT LEARNING
Reinforcement learning task using Generalized Advantage Estimation (GAE)
It is a model-free policy gradient approach with two neural networks as actor and critic respectively. The control task is to learn a policy to smoothly descend a lunar lander to the ground in between two flags with minimal fuel use and without damaging it.
Challenges: dual neural network parametrizations, improving rewards structure, extending vanilla policy gradients with advantage estimation.



