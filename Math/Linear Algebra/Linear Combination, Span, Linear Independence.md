---
title: Linear Combination, Span, Linear Independence
tags:
  - Mathematics
draft: false
aliases:
  - Alexandre DesAulniers
---
#### Linear Combination 

- A linear combination is something you can make by adding scalars to each of the given vectors, and adding them up.

- The sum of all vectors, with a scalar

- That's all!

![[Pasted image 20240408131343.png |500]]

#### Span

- The span is the area that can be reached by any linear combination

For a non zero single vector, the span would look kind of like this 

![[Pasted image 20240408143315.png|500]]

- The span is anywhere that this line can get too! There's only a single vector here.

**Here, we've got two vectors.** 

 - Two vectors are usually visualized as a plane, as with giving those two vectors scalars, you can get anywhere on that plane. 

![[Pasted image 20240408143554.png|500]]

This can go on, and on and ***on***... for n vectors (meaning it can be in ℝ<sup>n</sup>)
- Sometimes, "span" can be a verb, and it can "span ℝ<sup>n</sup>". 
- That would mean that the span of the set of given vectors covers ***everywhere*** in that dimension 
#### Linear Independence

- Any set is linearly independent If no element in the set is a linear combination of other elements in the set.

Example of Dependence

![[Pasted image 20240408151000.png|400]]

Example of Independence 

![[Pasted image 20240408151219.png|400]]


What can also be done to solve for linear independence/dependence is:
1) Put vectors into a matrix 
2) Do RREF 
3) If there is a row of zeros, you now have a "free parameter" and you have linear **dependence**. 

Examples of 2D and 3D linear dependence and dependence!

![[NKvYQ.gif|400]]
![[linear-dependence-3d.png|400]]