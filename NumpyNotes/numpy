"""
NumPy for Research Computing
============================

Purpose:
    Learn the NumPy features required for numerical research,
    especially mathematical modeling, parameter extraction,
    and data analysis.

NumPy will be used for:
    - Numerical arrays
    - Mathematical calculations
    - Vectorized operations
    - Experimental/simulation data
    - Residual and error calculations
    - Basic linear algebra
"""

import numpy as np


# ============================================================
# 1. NUMPY ARRAYS
# ============================================================

# A NumPy array stores numerical values.
# Arrays allow us to perform mathematical operations
# on many values at once.

voltage = np.array([0.0, 0.1, 0.2, 0.3, 0.4])

print(voltage)


# Example: experimental current data

current = np.array([0.0, 0.02, 0.15, 0.80, 2.10])

print(current)


# ============================================================
# 2. ARRAY INFORMATION
# ============================================================

print(voltage.shape)   # Shape/dimensions of the array
print(voltage.size)    # Number of elements
print(voltage.dtype)   # Type of data stored


# ============================================================
# 3. BASIC MATHEMATICAL OPERATIONS
# ============================================================

temperature_c = np.array([10, 20, 30, 40, 50])

temperature_k = temperature_c + 273.15

print(temperature_k)

# NumPy applies the operation to every element.
#
# [10, 20, 30] + 273.15
#
# becomes
#
# [283.15, 293.15, 303.15]


# Multiplication

voltage = np.array([1, 2, 3, 4, 5])

scaled_voltage = voltage * 2

print(scaled_voltage)


# Division

half_voltage = voltage / 2

print(half_voltage)


# Powers

squared_voltage = voltage ** 2

print(squared_voltage)


# ============================================================
# 4. MATHEMATICAL FUNCTIONS
# ============================================================

x = np.array([1, 4, 9, 16, 25])

print(np.sqrt(x))      # Square root
print(np.log(x))       # Natural logarithm
print(np.log10(x))     # Base-10 logarithm


# Exponential function

x = np.array([0, 1, 2, 3])

print(np.exp(x))

# np.exp(x) calculates e^x for every element.
#
# Exponential functions are especially important in
# semiconductor equations.


# ============================================================
# 5. CONSTANTS
# ============================================================

print(np.pi)

radius = 2

area = np.pi * radius ** 2

print(area)


# ============================================================
# 6. CREATING NUMERICAL RANGES
# ============================================================

# np.arange(start, stop, step)

x = np.arange(0, 10, 1)

print(x)

# The stop value is normally NOT included.


# np.linspace(start, stop, number_of_points)

x = np.linspace(0, 1, 11)

print(x)

# This creates 11 equally spaced values from 0 to 1.


# linspace is very useful when creating values for
# mathematical models and simulations.


# ============================================================
# 7. INDEXING
# ============================================================

voltage = np.array([0.0, 0.1, 0.2, 0.3, 0.4])

print(voltage[0])      # First element
print(voltage[2])      # Third element
print(voltage[-1])     # Last element


# Python uses zero-based indexing.
#
# voltage[0] -> first value
# voltage[1] -> second value
# voltage[2] -> third value


# ============================================================
# 8. SLICING
# ============================================================

print(voltage[1:4])

# This selects:
#
# index 1
# index 2
# index 3
#
# The ending index (4) is not included.


# ============================================================
# 9. BOOLEAN FILTERING
# ============================================================

voltage = np.array([0.1, 0.3, 0.5, 0.7, 0.9])

high_voltage = voltage[voltage > 0.5]

print(high_voltage)

# Boolean filtering allows us to select only the data
# satisfying a particular condition.
#
# This can be useful when analyzing only a certain
# region of experimental data.


# ============================================================
# 10. ELEMENT-WISE OPERATIONS
# ============================================================

voltage = np.array([1, 2, 3, 4])

current = np.array([2, 3, 4, 5])

power = voltage * current

print(power)

# Multiplication happens element by element:
#
# [1, 2, 3, 4] * [2, 3, 4, 5]
#
# gives
#
# [2, 6, 12, 20]


# ============================================================
# 11. BASIC STATISTICS
# ============================================================

current = np.array([0.10, 0.12, 0.11, 0.13, 0.09])

print(np.mean(current))   # Mean
print(np.max(current))    # Maximum
print(np.min(current))    # Minimum
print(np.std(current))    # Standard deviation


# These functions are useful when analyzing
# experimental measurements.


# ============================================================
# 12. WORKING WITH EXPERIMENTAL DATA
# ============================================================

voltage = np.array([0.0, 0.1, 0.2, 0.3, 0.4])

current = np.array([0.0, 0.03, 0.12, 0.75, 1.95])

print("Number of measurements:", len(voltage))

print("Average current:", np.mean(current))

print("Maximum current:", np.max(current))

print("Minimum current:", np.min(current))


# ============================================================
# 13. MATHEMATICAL MODEL USING NUMPY
# ============================================================

# One important use of NumPy in research is evaluating
# a mathematical equation for many values at once.

V = np.linspace(0, 0.7, 100)

I0 = 1e-12
Vt = 0.026

I = I0 * (np.exp(V / Vt) - 1)

print(I)

# Instead of calculating the equation separately for
# every voltage value, NumPy evaluates it for the
# entire array.


# ============================================================
# 14. RESIDUALS
# ============================================================

# A residual is the difference between a measured value
# and the corresponding model value.
#
# residual = measured - model

measured = np.array([1.0, 2.1, 2.9, 4.2])

model = np.array([1.1, 2.0, 3.0, 4.0])

residual = measured - model

print(residual)


# Residuals will become very important when we use
# optimization methods to fit a model to data.


# ============================================================
# 15. ERROR MEASURES
# ============================================================

absolute_error = np.abs(residual)

mean_absolute_error = np.mean(absolute_error)

mean_squared_error = np.mean(residual ** 2)

print("Mean Absolute Error:", mean_absolute_error)

print("Mean Squared Error:", mean_squared_error)


# These types of error measures can be used to compare
# how well different models or parameter sets fit data.


# ============================================================
# 16. BASIC MATRICES
# ============================================================

A = np.array([
    [1, 2],
    [3, 4]
])

print(A)

print(A.shape)

# A is a 2 x 2 matrix.


# ============================================================
# 17. MATRIX OPERATIONS
# ============================================================

B = np.array([
    [5, 6],
    [7, 8]
])


# Element-wise multiplication

print(A * B)


# Matrix multiplication

print(A @ B)

# The @ operator performs matrix multiplication.


# ============================================================
# 18. BASIC LINEAR ALGEBRA
# ============================================================

print(np.linalg.det(A))

print(np.linalg.inv(A))

# np.linalg contains linear algebra functions.
#
# det -> determinant
# inv -> inverse matrix
#
# More advanced linear algebra will only be learned
# if it becomes necessary for the research.


# ============================================================
# 19. RESEARCH-STYLE EXAMPLE
# ============================================================

# Suppose we have measured voltage and current
# from a device.

V_measured = np.array([
    0.10,
    0.20,
    0.30,
    0.40,
    0.50
])

I_measured = np.array([
    0.01,
    0.05,
    0.20,
    0.80,
    2.50
])


# Suppose we have a simple theoretical model.

I0 = 1e-4

Vt = 0.10

I_model = I0 * (np.exp(V_measured / Vt) - 1)


# Calculate the difference between measurement
# and theoretical model.

residual = I_measured - I_model


print("Measured current:")
print(I_measured)

print("Model current:")
print(I_model)

print("Residual:")
print(residual)


# ============================================================
# 20. KEY NUMPY CONCEPTS FOR THIS RESEARCH
# ============================================================

"""
The most important NumPy concepts to understand are:

1. np.array()
2. Array indexing and slicing
3. Vectorized mathematical operations
4. np.exp()
5. np.log()
6. np.linspace()
7. np.arange()
8. np.mean()
9. np.std()
10. Boolean filtering
11. Residual calculations
12. Basic matrix operations

These provide the numerical foundation for the research.

Next:
    SciPy will be used for optimization, curve fitting,
    numerical methods, and parameter extraction.
"""