---
title: Line Integrals
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---

In single variable calculus, we have definite integrals
$$\int_{x=a}^b f(x)dx$$

We integrate f(x) along a straight line

Note: If f(x) =1 

$$\int_a^bdx =x|^b_a = b-a \Rightarrow \text{length of line}$$

Now: Curve r(t) = (x(t), y(t), z(t))


$$\int_{t=a}^b ds =\text{arclength}$$

This is a special case of "*Line Integrals*"

In 3D:
$$\int_{t=a}^bf(x,y,z)ds$$ 
In 2D:

$$\int_{t=a}^bf(x,y)ds$$

If (x,y,z) = 1, we have an *arclength*


<u>How do we solve this?</u>

$$\int_c fds \space \text{integrating f over a curve c}$$

We need to transform this into a definite integral!

Step 1: Find a parametric description of c

$$\vec{r}(t) =x(t),y(t),z(t)$$

Step 2: Find f(x,y,z) on r(t)
		We plug in and get f(t)


Step 3: Find ds in terms of dt
	Recall that:
	$$ ds = ||\vec{v}||dt = ||\frac{d\vec{t}}{dt}|| dt$$
	$$\int^b_{t=a}f(t)||\frac{d\vec{t}}{dt}|| dt$$

Here's an abridged example, abbreviated as we did part of it yesterday. We plug in r(t).

![[PXL_20240605_143047855.jpg]]

$$\oint \Leftarrow\text{This means that the curve is closed! It is treated the same}$$
### Line Integrals and Vector Fields

##### Work

Work is a measure of F in the tangent direction!
$$\vec{F}\cdot \hat{T}$$

$$\text{Work} = \int_c\vec{f}\cdot\hat{T}ds$$

OR

$$\text{Work} = \int_c\vec{f}\cdot\frac{d\vec{r}}{dt}dt$$

##### Flux

Work is a measure of F in normal direction! Think of this as the flow across the curve. 
$$\vec{F}\cdot \hat{N}$$
Remember, now N = T x K

We'll also say for flux, f(t) = (P,Q) instead of X and Y
$$\text{Flux} = \int_c\vec{f}\cdot\hat{N}ds$$
OR

$$\text{Flux} = \int_c(P\frac{dy}{dt}-Q\frac{dx}{dt})dt$$

**Takeaways: Work = Tangential Direction, Flux = Normal Direction**

--- 

<u>Line Integrals and Special Fields</u>

If F is conservative,  ∇ x f =0

If F is incompressible,  ∇ ⋅ f =0 

