---
title: Distance and Arc Length Calculation
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
### Arclength Calculation

r(t) = Position at a time.

- To calculate distance, multiply **Speed** and **Time** 
- Speed is the magnitude of velocity
- Distance (S), also known as arclength is equal to the integral of the magnitude of V, times dt (a tiny chunk at that time) from time 1, to time 2.

$$
\int_t^{t+\Delta t} {||\vec{v}|| dt}
$$

### Frenet-Serret Frame (Moving Triad)

- This is a new coordinate system
- Made up of Unit Tangent (T), Unit Normal (N), and a perpendicular vector known as the Binormal (B) 
- The Binormal is found by taking the cross product of T and N 

$$
\vec{B} = \vec{T} \times \vec {N}
$$

- Right hand rule applies here! 
	- Fingers along T
	- Curl fingers towards N.
	- Thumb points in direction of B 
- Another nice trick, is that N always points to the center of curvature.
	- If T is going in a direction where the curve is increasing, N is facing up
	- If T is going in a direction where the curve is decreasing, N is going down

- Another unique thing about this coordinate system, is that T, N and B are all ***functions of time***
- T(t), N(t), B(t)
- This coordinate system can warp with time

![[Frenetframehelix.gif]] ![[Frenet-Serret-frame_along_Vivani-curve.gif|192]]

Black = B
Blue = T
Red = N

### Acceleration

What's cool about Acceleration along a curved path like such, is acceleration has two components

at = Transintestinal Acceleration
an = Normal Acceleration


Acceleration 
$$
\vec{a} = \vec{a_t} + \vec{a_n}
$$
at = Transintestinal Acceleration
$$
a_t=\vec{a} \cdot \hat{T}
$$
$$
a_t =\vec{a} \cdot \frac{\vec{v}}{||\vec{v}||}
$$
an = Normal Acceleration
$$
a_n=\vec{a} \cdot \hat{N}
$$

$$
a_n=\frac{||\vec{a} \times \vec{v}||}{||\vec{v}||}
$$

### Other helpful Frenet-Serret Stuff

$$
\vec{v} = ||\vec{v}||\hat{T}
$$

V = Magnitude of Velocity (Speed)
T = Direction of Unit Tangent (Direction)


$$
\hat{B} = \frac{\vec{v}\times\vec{a}}{||\vec{v}\times\vec{a}||}
$$
- This is **quite** a rigorous proof
- Note, in the bottom, he does switch `a X v` to `v X a`
	- Normally, this would switch the direction of the perpendicular product, but since we're taking the magnitude, *we do not care*.

$$
\hat{N} = \hat{B}\times\hat{T}
$$

- A re-arrangement of the previous formula
