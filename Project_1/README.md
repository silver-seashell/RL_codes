
# Project 1: Solving the *n-Armed Bandit* Problem

## 1.
Using Python, write a program that generates a random vector with a Gaussian (normal) distribution with variance sigma^2 to represent the true action values q*(a).

---

## 2.
Assume **sigma^2 = 1**. For an n -armed bandit with **n = 10**, generate the average reward values q*(a) such that they are approximately equal to the values used in Figure (2-1) on page 28 of the textbook.

---

## 3.
Assume 1000 steps per run and 2000 independent runs.

For each of the following greedy-type action selection methods, compute and plot the average reward versus steps:

- greedy action selection
- ε-greedy with epsilon = 0.1 
- ε-greedy with epsilon = 0.01


---

## 4.
Using the softmax action selection method with T = 1, compute and plot the average reward versus steps and compare its results with those obtained in part 3.

---

## 5.
For the three action selection methods above, plot the percentage of optimal actions selected versus steps (i.e., percentage of times the action with maximum reward is chosen), and compare them with each other.

