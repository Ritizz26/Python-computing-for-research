# SciPy Basics
# Used for scientific and engineering calculations
# in the solar-cell modeling project.

import scipy

# Check the installed SciPy version
print(scipy.__version__)


# --------------------------------
# SciPy Optimize
# --------------------------------

# optimize contains tools for solving equations
# and finding optimal values.
from scipy import optimize


# --------------------------------
# Root Finding
# --------------------------------

# A root is a value where a function equals zero.
#
# Example:
# x^2 - 4 = 0
# The root in the interval 0 to 3 is x = 2.

def f(x):
    return x**2 - 4


# brentq() finds a root of a function
# within a specified interval.
root = optimize.brentq(f, 0, 3)

print("Root =", root)


# --------------------------------
# Passing Extra Arguments
# --------------------------------

# args=() passes additional values
# to the function being solved.

def solar_equation(I, V):
    return I - Iph + Io * (
        np.exp(q * (V + I * Rs) / (n * k * T)) - 1
    )


# Example:
# current = optimize.brentq(
#     solar_equation,
#     lower_limit,
#     upper_limit,
#     args=(V,)
# )


# --------------------------------
# Concepts Learned
# --------------------------------

# scipy                -> Scientific computing library
# scipy.optimize       -> Tools for solving and optimizing problems
# brentq()             -> Finds a root within an interval
# def function()       -> Defines a function for the solver
# args=()              -> Passes extra arguments to a function
# root                  -> Value where the function equals zero


# Applied to:
# - Numerical equation solving
# - Solar-cell modeling with series resistance