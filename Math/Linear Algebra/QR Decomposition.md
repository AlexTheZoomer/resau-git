---
title: QR Decomposition
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---

$$
A = QR
$$

- This is what makes up QR Decomposition! 
- ***Q*** is a Orthogonal Matrix. (It has orthonormal column vectors!)
- ***R*** is a Upper Triangular Matrix

To get a QR decomposition:

1) Take ***A***, and [apply the Gram-Schmidt process](https://youtu.be/J41Ypt6Mftc?feature=shared) to the vectors inside it. 
2) Once you have found the orthonormal vectors of ***A***, load them into a matrix by column. <u>You now have</u> ***Q***
3) Now, to find ***R***. This is where some theory comes in. 

- We have ***A*** and we have ***Q***. We will multiply both sides of this equation to get 
$$
Q^\perp A = Q^\perp QR
$$
- Now, due to the properties of the *orthogonal basis,* and the *orthonormal columns*, we find this
$$
Q *Q^\perp = I
$$
- This leaves us with ***I***. The ***I*** (identity matrix) is left on the right side!

$$
Q^\perp A = IR
$$
- So, to find R, we just have to solve 
$$
Q^\perp A = R
$$

Done! The R matrix has been solved for. 

![[Pasted image 20240409212747.png|400]]


--
