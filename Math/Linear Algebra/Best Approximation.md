---
title: Best Approximation
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---


Best Approximation isn't all that bad!  

- Best approximation uses the projection formula to approximate fits of lines

An example of projecting Y onto U, a vector perpendicular with W.
$$
\hat{Y}= proj_u\vec{Y} = \frac{\vec{u} \vec{Y}}{\vec{u}\vec{u}}[u]
$$

Here is an easy example of such!

![[Pasted image 20240411102746.png|500]]

What is happening here, is you are projecting a vector on to **a, or a series of basis vectors**. 
- You might be given those vectors, but you'll most likely have to get them with G.S.
- "Those vectors" are the **orthogonal basis** 

In a 3D space, you'll have a bunch of those orthogonal basis's 

![[Pasted image 20240411103112.png|400]]

- Here, you can see what she is doing. <font color="#92d050">In green</font> she is defining her two <font color="#92d050">basis vectors</font>, and her <font color="#92d050">other Y vector.</font>
- In <font color="#ffc000">orange</font>, she is setting up a <font color="#ffc000">projection formula for each basis vector</font>, summing them up. 

What you receive, is the best approximation of the subspace, or the closest point to the subspace. 