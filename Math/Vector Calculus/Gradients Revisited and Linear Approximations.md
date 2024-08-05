---
title: Gradients Revisited and Linear Approximations
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
### Final Notes about Gradients (Geometric Properties of the gradient)

- As we are moving along a curve in space,**∇**f is ***perpendicular*** to **r̂'** 

![[PXL_20240521_141612570~2.jpg|400]]

---
### Linear Approximations 

- By using the tangent line of an earlier point, we can approximate a later point on a curve
- Maybe that isn't a great method of approximation.... so let's use higher derivatives to help!
- This is **Taylor Series**!

![[PXL_20240521_143221590.jpg]]

- What's cool, is we can also approximate a "tangent plane" in a similar way! 

![[PXL_20240521_143516616.jpg]]

- Usually, a first order approximation is... good enough. More so would be more accurate, but a pain to write out.

![[Pasted image 20240528212810.png]]

The Gradient is related to linear approximation!

![[PXL_20240521_144624809~2.jpg]]

---
### Extreme Values (Minimums and Maximums)

##### For a single variable function y=f(x)....

- Extreme Values of Y at x =c
	If f(x)<f(c) for x near c, *you have a local max*
	If f(x)>f(c) for x near c, *you have a local min*

- Extreme Values occur at 3 types of points

1) <span style="background:#ff4d4f">Critical Points</span> ⇒ df/dx = 0
2) <span style="background:#40a9ff">Singular Points </span>⇒ df/dx = undefined
3) <span style="background:#affad1">Boundaries</span> ⇒ The ends 

![[PXL_20240521_150145804.jpg]]

But what if we don't have a graph?

- To find critical points: 
	1)  Take the first derivative of a function
	2) Set df/dx =0 and solve for X 
	
- To determine minimum or maximum
	1) Take the second derivative of a function. This studies the rate of change of the rate of change
	2) 
	- If d<sup>2</sup>f/dx<sup>2</sup> < 0   ⇒ You have a local *max*
	- If d<sup>2</sup>f/dx<sup>2</sup> > 0   ⇒ You have a local *min*
	- If d<sup>2</sup>f/dx<sup>2</sup> = 0   ⇒ Your curve is flat, and you don't have enough information!
	
- If you have a case where d<sup>2</sup>f/dx<sup>2</sup> < 0 at some point before the critical point, and where If d<sup>2</sup>f/dx<sup>2</sup> > 0 after the critical point, or vice versa, you have an ***inflection point***

##### For a multivariable function y=f(x,y,z,....)....

Types of Extreme Values

1) <span style="background:#ff4d4f">Critical Points</span> ⇒ D<sub>u</sub>f (The directional derivative) **= 0** for all û (*for all directions*)
2) <span style="background:#40a9ff">Singular Points </span>⇒  D<sub>u</sub>f (The directional derivative)  = undefined
3) <span style="background:#affad1">Boundaries</span> ⇒ The ends 

$$
D_uf= \nabla f\cdot\hat{u}
$$ $$
\text{To have a critical point, } D_uf \text{ must equal 0} 
$$
$$
\text{If } \nabla f =0, \text{ that makes this true.}
$$


Finding critical points: **∇**f = 0,  solve for points

$$
(\frac{∂f}{∂x}, \frac{∂f}{∂y}, \frac{∂f}{∂z} ) = (0,0,0) 
$$
![[Pasted image 20240528213547.png|600]]



<span style="background:#fff88f">Second Order Directional Derivative</span><span style="background:#fff88f">!</span> (<font color="#3f3f3f">very bad</font>)

![[Pasted image 20240521113029.png]]

<u>Remember:</u>

- The Gradient nabla operator (**∇**) vectorizes scalars. That dot product multiplied by the nabla is a scalar, being vectorized. It doesn't visually mean anything, but makes things
- U<sub>x</sub> and U<sub>y</sub> are direction vectors 

- To determine minimum or maximum
	1) Take the second derivative of a function. This studies the rate of change of the rate of change
	2) 
	- If d<sup>2</sup><sub>u</sub>f< 0 for all û (*for all directions*)  ⇒ You have a local *max*
	- If d<sup>2</sup><sub>u</sub>f > 0 for all û (*for all directions*)  ⇒ You have a local *min*
	-  If d<sup>2</sup><sub>u</sub>f< 0 for all û (*for all directions*) = 0   ⇒ Your curve is flat, and you probably have a saddle point (think the dip in a horse saddle)

![[Pasted image 20240528213635.png|600]]

##### Restrictions 

- If you are given a restriction, such as x=2, the easiest way to solve the problem is to *reduce the dimensionality*.

	- Just plug whatever your restriction is into the function, and solve for the other variable's critical point. 

