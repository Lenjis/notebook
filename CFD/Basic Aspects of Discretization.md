# Basic Aspects of Discretization

> In essence, discretization is the process by which a closed-form mathematical expression, such as a function or a differential or integral equation involving functions.

## Introduction to finite defferences

![Taylor series about point(i,j)](image/BasicAspectsofDiscretization/1743155278026.png)

Solving

$$
\left( \frac{\partial u}{\partial x} \right) _{i,j} = \frac{u _{i + 1, j} - u _{i, j}}{\Delta x} - \left( \frac{\partial^2 u}{\partial x^2} \right) _{i,j} \frac{\Delta x}{2} - \left( \frac{\partial^3 u}{\partial x^3}\right) _{i,j} \frac{(\Delta x)^2}{6} + \dots
$$

for $(\frac{\partial u}{\partial x}) _{i,j}$

$$(\frac{\partial u}{\partial x}) _{i,j}=\frac{u _{i+1,j}-u _{i,j}}{\Delta x}+O(\Delta x)
$$

which is called *first-order-accurate.*

To construct a finite-difference quotient of *second-order* accuracy:

$$
u _{i+1,j} - u _{i-1,j} = 2\left(\frac{\partial u}{\partial x}\right) _{i,j} \Delta x + 2\left(\frac{\partial^3 u}{\partial x^3}\right) _{i,j} \frac{(\Delta x)^3}{6} + \dots
$$

$$
\left(\frac{\partial u}{\partial x}\right)
$$
