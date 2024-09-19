---
title: Summary of Line and Surface Integrals
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
#### Integration

- ##### Line Integrals
$$
\int_c(x,y,z)ds
$$

Where the curve C is parametrized as r(t)

and we solve this as..
$$
\int^b_a(F_{\text{oncurve}}||\frac{dr}{dt}||dt)
$$
---

- ##### 2D Surface Integrals

$$
\iint_s f(x,y,z)ds
$$

Where S could be
S = r(t,k)
or H (x,y,z) =0

What's important here, is that you get the normal, N (Usually the gradient)

and we solve this as...

$$
\int^b_a(F_{\text{onsurface}}||\vec{n}||dA)
$$
---

- ##### 3D Surface Integrals

$$
\iiint_{vol} f(x,y,z)ds
$$
We solve this one is a similar way! 

___
#### Theorems (Special cases that give alternative ways to calculate)

- ##### 1D

**FOTOC**
$$
\int_{x=a}^b (\frac{dg}{dx}) = g(b) - g(a)
$$
b) **Path Independent Special Case**

$$
\int_c \nabla g \cdot \hat{T}ds = g(b) - g(a)
$$

another form of that 
$$
\int_c (\nabla g \times\hat{k} ) \hat{N}ds = g(b) - g(a)
$$
- ##### 2D

**Green's Theorem**

Normal/Flux Form, also known as 2D Divergence Theorem. 
$$
\iint_R \nabla \cdot \vec{F}dA = \oint_c \vec{F} \cdot \hat{N}ds
$$

Tangential/ Circular form, also known as 2D Stokes theorem
$$
\iint_R (\nabla \times \vec{F}) \cdot \hat{k}dA = \oint_c \vec{F} \cdot \hat{T}ds
$$

- ##### 3D

**Stokes Theorem**

$$
\int_c (\nabla \times\vec{F} ) \hat{N}ds = \oint_c\vec{F}\cdot\hat{T}ds
$$

When Stokes is a flat region, S turns into R< and we just get Green's theorem again.

**Divergence Theorem**

$$
\iiint_{Vol}(\nabla\cdot F)dVol = \oint \oint_S \vec{F}\cdot \hat{N}ds
$$
