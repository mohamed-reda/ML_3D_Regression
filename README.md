# ML 3d Linear Regression example

## Overview

This project provides a minimal example of implementing simple linear regression using PyCharm Community Edition and
NumPy. The example demonstrates how to generate random input data, create targets with a predefined function, visualize
the training data, and train a linear regression model using gradient descent.

## Requirements

- PyCharm Community Edition (Read-only Jupyter notebook support)
- NumPy
- Matplotlib

## Getting Started

To experience the full support for local notebooks, it is recommended to use PyCharm Professional. Additionally,
JetBrains offers DataSpell as a dedicated IDE for data science with local and remote notebook support, and Datalore as
an online environment for Jupyter notebooks in the browser. More information about JetBrains Data Solutions can be found
on the [official website](https://www.jetbrains.com/datatools/).

## Usage

1. Import the relevant libraries by executing the provided code snippet.

2. Generate random input data to train on by following the code snippet that initializes and combines input variables (
   xs and zs).

3. Generate targets using a predefined function and add random noise to simulate real-world scenarios.

4. Plot the training data in 3D to visualize the trend that the model should learn.

5. Initialize weights and biases randomly within a specified range.

6. Set a learning rate to control the step size during gradient descent.

7. Train the model using gradient descent for a specified number of iterations.

8. Print the final weights and biases to evaluate convergence.

9. Plot the last outputs vs. targets to visualize the model accuracy.

## Modification

To experiment with the simple linear regression example, consider modifying the code snippet that changes the target
declaration. Observe the impact on the loss function, weights, and biases.

## Takeaways

- The algorithm's effectiveness is comparable to the lecture example but may require additional iterations.
- Higher target values result in higher loss values.
- The same algorithm and methodology can solve different problems, showcasing the versatility of machine learning.

Feel free to explore, modify, and learn from this simple linear regression example using PyCharm and NumPy.


---


to run jupyter:

jupyter notebook

(Use Control-C to stop this server)

----
pip install -r requirements.txt

python -m pip install jupyter

---
memory profile:

@memory_profiler.profile

python -m memory_profiler main.py

---

from line_profiler_pycharm import profile

@profile

python -m line_profiler main.py.lprof > results.txt
