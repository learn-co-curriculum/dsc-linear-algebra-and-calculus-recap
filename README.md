# Linear Algebra and Calculus - Recap


## Introduction

Congratulations! You have learned the fundamentals of the math at the core of machine learning: linear algebra and calculus.


## Key Takeaways

### Linear Algebra

The goal of this part was to provide both a conceptual and computational introduction to linear algebra. Some of the key takeaways include: 

* Scalars, vectors, matrices, and tensors
  * A ***scalar*** is a single, real number
  * A ***vector*** is a one-dimensional array of numbers
  * A ***matrix*** is a 2-dimensional array of numbers
    * Two matrices can be added together if they have the same shape
    * Scalars can be added to matrices by adding the scalar (number) to each element
    * To calculate the dot product for matrix multiplication, the first matrix must have the same number of columns as the number of rows in the second matrix
  * A ***tensor*** is a generalized term for an n-dimensional rectangular grid of numbers. A vector is a one-dimensional (first-order tensor), a matrix is a two-dimensional (second-order tensor), etc.
  * One use case for vectors and matrices is for representing and solving systems of linear equations 
* Linear algebra in Python
  * Operating on ***NumPy*** data types is substantially more computationally efficient than performing the same operations on native Python data types
  * It is possible to use linear algebra in NumPy to solve for a linear regression using the ***OLS*** method
  * OLS is not computationally efficient, so in practice, we usually perform a gradient descent instead to solve a linear regression

### Calculus and Gradient Descent

The goal of this part was to learn some of the foundational calculus that underpins the gradient descent algorithm. Some of the key takeaways include:

* Calculus
  * A ***derivative*** is the "instantaneous rate of change" of a function - or it can be thought of as the "slope of the curve" at a point in time
    * A derivative can also be thought of as a special case of the rate of change over a period of time - as that period of time is zero. 
  * If you calculate the rate of change over a period of time and keep reducing the period of time, it usually tends to a limit - which is the value of that derivative
  * Rules can be used for finding derivatives
    * The ***power rule***, ***constant factor rule***, and ***addition rule*** are key tools for calculating derivatives for various kinds of functions
    * The ***chain rule*** can be a useful tool for calculating the derivate of composite functions
* Gradient descent
  * A derivative can be useful for identifying local ***maxima*** or ***minima*** as in both cases, the derivative tends to zero
  * A ***cost curve*** can be used to plot the values of a cost function (in the case of linear regression) for various values of offset and slope for the best fit line
  * ***Gradient descent*** can be used to move towards the local minimum on the cost curve and thus the ideal values for the y-intercept and slope to minimize the selected cost function when performing a linear regression
