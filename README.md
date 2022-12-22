# Basic-AI-Graphing-Calculator
Here's a simple example of how you could write a Python program that works as a graphing calculator:

import matplotlib.pyplot as plt

def graph(formula, x_range):
    x = x_range
    y = [formula(i) for i in x]
    plt.plot(x, y)
    plt.show()

def f(x):
    return x**2

graph(f, range(-100, 101))


