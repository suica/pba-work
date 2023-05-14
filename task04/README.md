# Task04: Accelerated Nearest Search using Kd-Tree

![preview](preview.png)

**Deadline: March 18th (Thu) at 15:00pm**

----

## Before Doing Assignment

If you have not done the [task00](../task00), do it first to set up the C++ graphics development environment.

Follow [this document](../doc/submit.md) to submit the assignment, In a nutshell, before doing the assignment,

- install `eigen` library following  [this document](../doc/setup_eigen.md)
- make sure you synchronized the `main ` branch of your local repository  to that of remote repository.
- make sure you created branch `task03` from `main` branch.
- make sure you are currently in the `task03` branch (use `git branch -a` command).

Now you are ready to go!

---

## Problem 1

This program is computationally expensive. Build the program with ***Release*** mode to make the program run faster.  
Configure the project with 
```bash
cmake -DCMAKE_BUILD_TYPE=Release ..
```
instead of
```bash
cmake ..
```

Then, run the code. Take a screenshot image (it should look like image at the top) after 200 steps for the 20k particles.
Save the screenshot image overwriting `task03/problem1.png`

![problem1](problem1.png)


This program computes distance field from random particle.

Run the program with different numbers of the particles (5k, 10k, and 20k).
The number of the particle can be set at `line #189`  in [main.cpp](main.cpp).
Record the computation time by filling the table below.     

| #particle | time |
| --- | --- |
| 5000 | ? |
| 10000 | ? |
| 20000 | ? |


## Problem 2

The current code compute the distance in the brute-force way. 
If the is `N` number of points, the computational cost is `O(N)`.  
Let's accelerate the computation using the Kd-tree data structure.

Write a few lines of code around `line #115` to accelerate the search. 

Run the program with different numbers of the particles (5k, 10k, and 20k). 
Record the computation time by filling the table below.

| #particle | time |
| --- | --- |
| 5000 | ? |
| 10000 | ? |
| 20000 | ? |


## After Doing the Assignment

After modifying the code, push the code and submit a pull request.




## Notes

- Do not submit multiple pull requests. Only the first pull request is graded
- Do not close the pull request by yourself. The instructor will close the pull request
- If you mistakenly merge the pull request, it's OK, but be careful not to merge next time. 