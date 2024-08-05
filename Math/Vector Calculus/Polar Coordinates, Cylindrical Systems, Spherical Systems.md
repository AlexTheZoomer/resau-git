---
title: Polar Coordinates, Cylindrical Systems, Spherical Systems
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
### Polar Coordinates

![[image002.gif]]

x = rcosθ
y = rsinθ

- Polar Coordinates are another way of representing graph systems 
- How to we apply polar coordinates to what we have been doing with double and triple integrals?

$$\iint_{Rxy}f(x,y)dxdy \space\space\space=\space\space\space \iint_{Rr\theta}g(r,\theta)rdrd\theta$$



- There is a proof for this, but this is what we feed into our double and triple integrals for polar coordinates!
- You can use polar coordinates for functions that are not nice with regular coordinates. 
- A classic example of such would be x<sup>2</sup> + y<sup>2</sup> = 1 

### Polar Coordinates for Double Integrals

Step One: Convert from f(x,y) to g(r, θ)

Step Two: Convert dx/dy to dArθ
	-  Tip for this, it will **ALWAYS** be rdrdθ

Step Three: Convert limits (Plug in and work out)
	- This can be a bit tricky.

Step Four: Now, integrate as normal. U-Sub may be needed 

---
### Polar Coordinates for Triple Integrals

Now, we are dealing with ***cylindrical coordinates***! (Polar in 3D)

x = rcosθ
y = rsinθ
z = z 

dVol ⇛ dxdydz ⇛ rdrdθdz

![[PXL_20240528_144733634.jpg|400]]

- Volume = ∫∫∫dVol 

---
### Spherical Coordinates (Globe)

x = rcosθsin**ϕ**
y = rsinθsin**ϕ**
z = rcos**ϕ**

r<sup>2</sup> = x<sup>2</sup> + y<sup>2</sup> +z<sup>2</sup>

- With Spherical Coordinates, you are going to have an R like usual
- However, you are going to have TWO angles 
- A polar angle along X and Y, and an azimuthal angle along Z
- The regular angle can stretch from 0 < θ < 2π
- The azimuthal angle can stretch from 0 < **ϕ** < π
	- It is not necessary for the full 2π, as you would be double accounting for each position

![[PXL_20240528_150918083.jpg]]

- Remember with U-sub, you can either change your limits in terms of U, or sub in for you after the integration with the original limits

---

END OF TEST 2 MATERIAL

### <u>Vector Spaces</u>

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
