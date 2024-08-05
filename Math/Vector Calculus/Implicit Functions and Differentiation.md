---
title: Implicit Functions and Differentiation
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
Explicit Functions:   y=F(x)

Implicit Functions:    F(x,y)=0
- All X's and Y's are on one side!

- Explicit functions can *always* be written as implicit functions 
- When looking for the rate of change of an implicit function, we have to to *implicit differentiation*

### Implicit Differentiation

<u>Example </u>

![[PXL_20240515_142331945.jpg|500]]

Remember, that y=f(x), or whatever term you are differentiating in terms of.

- Where we are differentiating by dx, Y acts as a functions f(x).
- From there, we chain rule our f(x) function, by derivative of outside times derivative of inside
---

<u>Example</u>

- Here, look at the tree!
- F is a function of x, y and z
- X stands on its own (first term)
- Y does not depend on X! So it has zero rate of change (second term)
- Z depends on both X and Y, but we are differentiating in terms of X, so it's all we care about! (Last term)
- Re-arrange and solve for dz/dx!

![[PXL_20240515_143306777.jpg]]

Example to try for later!

$$
z^2y+3y^2x-4x^3z=0
$$

- Solve for (dx/dz)

![[Pasted image 20240515115116.png]]

---
### Gradients and Directional Derivatives

#### Gradients

- Gradient of a function is a ***vector*** whose components are partial derivatives!

$$\nabla_f$$
(The upside down triangle is known as the "nabla", which is the gradient of F)

2D
$$
f(x,y) = \nabla_f = (\frac{∂f}{∂x},\frac{∂f}{∂y})
$$
3D
$$
f(x,y,z) = \nabla_f = (\frac{∂f}{∂x},\frac{∂f}{∂y},\frac{∂f}{∂z})
$$

Example

w = f(x,y,z) = xy +cos(z)

$$
\nabla_w = (\frac{∂w}{∂x},\frac{∂w}{∂y},\frac{∂w}{∂z})
$$
$$
= y,z,-sin(z)
$$

#### Directional Derivatives

- Rate of change of F in a direction of û
- û can be anything chosen!
$$
D_uf  \text{  if  }\hat{u} = \hat{i} \Rightarrow D_uf = \frac{∂f}{∂x}
$$
Generally, 

$$
D_uf = \nabla_f \cdot \hat{u}
$$

<u>Example</u>

![[PXL_20240515_151107563~2.jpg]]![[PXL_20240515_151250145 1.jpg]]

- Gradients are perpendicular to your level curves, and point to higher levels!
	- Unless the directional derivative is **NEGATIVE**. It then means you are pointing downwards
	- Which in this case, -(6/5)<sup>th</sup> ***is***. 

![[PXL_20240515_151853199.jpg|400]]

Here's a slightly squished graph of that problem!

- <span style="background:#40a9ff">Blue</span> lines are the level curves lines
- <span style="background:#affad1">Green</span> lines are the upwards gradient lines
- <span style="background:#d4b106">Orange</span> arrows are the û vectors calculated

Some quick questions about it..
1) What is the direction of steepest ascent here?
		Parallel to the <span style="background:#affad1">gradient</span>, going upwards!
		Direction of gradient ➟ (2x, 2y)
				I'm at (1,1) ➟ (2,2)
		
2) What is the direction of steepest decent here?
		Antiparallel to the <span style="background:#affad1">gradient</span>, going downwards!
		Direction of gradient ➟ (-2x, -2y)
				I'm at (1,1) ➟ (-2,-2)

1) What is the direction of no ascent or decent here?
		Perpendicular to <span style="background:#affad1">gradient</span> tangent to level curve
		$$
		\hat{u}\cdot\nabla{f} = 0
		$$
		You'll have F, and you'll need to solve for û



The equation of a plane that contains the point (x0,y0,z0) with normal vector →n=⟨a,b,c⟩ is given by,

a(x−x<sub>0</sub>)+b(y−y<sub>0</sub>)+c(z−z<sub>0</sub>)=0