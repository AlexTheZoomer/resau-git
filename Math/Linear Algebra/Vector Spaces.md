---
title: Vector Spaces
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
- A vector spaces is a set of vectors 

- Addition and Scalar multiplication can be used!

- Vector spaces can be anything, vectors, polynomials, functions

- If I have two polynomials of the first degree , `u = x + 1` and `v = 2x - 3`, they both share the same vector space, because they are same degree 

- If I add the polynomials `u = x + 1` and `v = 2x - 3` together, I get `uv = 3x - 2` 

- The resulting `uv = 3x - 2` is ***also*** a polynomial of degree one, so we're still in that original vector space!

- The same is true if I multiplied `u = x + 1` by **5**. I would get `5u = 5x +5`. `5u` is still a polynomial of degree one, so we're still in that first degree polynomial space!

--

- The same is true of I have the two matrices 
$$
\hat{u}=\begin{bmatrix}
2 &1 \\
1 &3
\end{bmatrix}
$$
and
 $$
\hat{v}=\begin{bmatrix}
-1 &0 \\
1 &1
\end{bmatrix}
$$
- If I add  and `v̂`, I get `û + v̂`
 $$
\hat{u} + \hat{v}=\begin{bmatrix}
1 &1 \\
2 &4
\end{bmatrix}
$$

- This results in a 2D vector, meaning that we are staying in the same 2D vector space. 
- `5û` would result in the same thing, another 2D vector. We're good here.

--
##### **These are known as the <font color="#00b050">properties of closure</font>**. 
- Given `û`ε***V*** (`û` is a vector in the vector space ***V***)  and scalar `C`, then `Cû`ε ***V***  (The multiplied scalar will also be in vector space V)

-  Given `û`ε***V***  and `v̂`ε***V***  , then `û + v̂`**ϵ** ***V***  (The new added vector is also in vector space ***V***!)

The dimension of the vector is usually noted by ℝ<sup>n</sup>. The amount of non zero rows in a vector will give you that.

--
#### What are Axioms? What are the 8 Axioms? 

Axioms are a bunch of rules which hold true inside of a vector space. There are 10 of  which hold true in any vector space ***V***

With vectors û, v̂ and ŵ, and scalars **a** and **b**

<u>Addition</u>
1)  `û + v̂` = `v̂ + û`                               This is known as the **commutative property of addition!** 

2) `û + (v̂ + ŵ)` = `(û + v̂) + ŵ`          This is known as the **associative property**

3) `û + 0 = û + 0`                                 There is a zero vector. This is known as the **additive                                                                                identity**

4) `û + û'`                                              For every vector in a vector space, there is another                                                                                  vector that can bring it back to **zero**. This property is                                                                               known as the **additive inverse**! 
<u>Multiplication</u>
5) For û**ϵ******V*** `1û = u`                                 For every single vector in the vector space ***V***,  1* û will                                                                            equal û. This is known as the **multiplicative identity** 

6) `a * (bu) = (ab) * u`                     This property does not seem to have a name, but is used                                                                         to combine scalars. Scalars can be combined as such.

7) `(a + b)u = au + bu`                       This is known as **distributivity of scalar multiplication                                                                             with respect to field addition**. Vectors can distribute like                                                                        this!

8) `a(u+v) = au + av`                           This is known as **distributivity of scalar multiplication                                                                             with respect to vector addition**. Just like the last                                                                                     property, this works as well!  

#### Vector Subspaces

- Vector Subspaces are, you guessed it, a ***vector space inside of another vector space***.

- If there is a subspace ***S*** inside of a vector space ***V***, the subspace ***S*** must follow all of ***V***'s rules.

- The earlier Addition and Scalar multiplication rules ([<font color="#2DC26B">properties of closure</font>]([[Final Linear Algebra Review]])) can be used to ensure conformance to the new subspace

![[Pasted image 20240407131512.png |500]]

##### Plane in a Three-Dimensional Space

- If you know that you have a plane in a 3D space, you DON'T know that it immediately is a subspace. 
- This is because of the possibility of having a scalar of "0" creating a "zero vector". 
- If you know that the plane passes through (0,0,0), you're good, because that condition works. 
- If you don't know that it passes through the origin (0,0,0), you don't have enough information to determine whether the plane is a subspace of the 3D space. 

##### Null Space

- Null Space is a situation to where all of the vectors in AX=B, are AX=0 
- Null Space is noted by N(A) (<font color="#595959">A being the matrix</font>)
- This occurs when you have a A matrix, transformed by an "X vector" to make it equal to zero. 

$$
A =\begin{bmatrix}
2 &1 \\
1 &3
\end
{bmatrix}
$$
$$
\begin{bmatrix}
2 &1 \\
1 &3
\end
{bmatrix}
\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix} =B
$$
To solve for the X's which make B=0, we can set up a homogenous solution with matrix augmentation.

$$
\begin{bmatrix}
2 &1 |0 \\
1 &3 |0
\end
{bmatrix}
=B
$$

- Do REF, or RREF, and solve for the unknown X's!
(keep in mind, this matrix is just:
$$
2x_1 + x_2 = 0
$$
$$
1x_1 + 3x_2 = 0
$$
)

A weird thing to think about, is that the null space is actually a subspace of A! It meets all of the criteria! 

- What is happening, is that the subspace is being crushed into zero by a transformation, and becomes a zero vector 

 ![[4ZL8s_ 1.gif]]
