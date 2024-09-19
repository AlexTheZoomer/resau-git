---
title: Gram-Schmidt, QR Decomposition, Orthogonal Sets and Subspaces
draft: false
tags:
  - Mathematics
aliases:
  - Alexandre DesAulniers
---
##### Gram-Schmidt (Or G.S. for Short....)

Before we begin with G.S. I love [this](https://www.youtube.com/watch?v=KOkuTXrv5Gg) video explaining what is going on while doing G.S.  Specifically the [2D part](https://youtu.be/KOkuTXrv5Gg?feature=shared&t=113)

- Dan starts with 2 vectors

![[Pasted image 20240409204705.png|300]]

- He wants to find the orthonormal to vector V<sub>1</sub>, using his vector V<sub>2</sub>
- He begins by converting V<sub>1</sub> into a unit vector, to satisfy the *normal* part. This is actually known as normalizing a vector. 
- He then projects V<sub>2</sub> on to the span of V<sub>1</sub>. *Dan now has his parallel component*

 ![[Pasted image 20240409205038.png|200]]

- Next, he subtracts his parallel projection from his V<sub>2</sub> vector, to find the *orthogonal part*

![[Pasted image 20240409205236.png|200]]

- From here, Dan normalizes his V<sub>2</sub> perpendicular vector (he also puts it on the Y axis now for clarity)

![[Pasted image 20240409205435.png|200]]

And just like that, it's done. **That is visually what is happening during the Gram-Schmidt Process**.

--

**Now, for the math/formula.** 

- Start with a series of basis vectors, defining a vector space. 
$$
\vec{v_1},\vec{v_2}...\vec{v_n} 
$$
- Now, for a solving pattern.

![[Pasted image 20240409210014.png|550]]

1) The first orthogonal basis is equal to the first basis vector. Makes sense.

2) The second orthogonal basis is equal to the second vector, **MINUS** the parts that are not orthogonal to the first basis! (shown earlier, what dan was doing!!)
		- An important thing to note here, is notice that the term being shaved off is just dot product! 

4) Rinse and repeat. It's the same thing over and over again, just adding another term of non-orthogonal parts to shave off!

Here is an [example.](https://youtu.be/zHbfZWZJTGc?feature=shared&t=263)

It is good to know, that when it's all said and done, the thing that you are solving for with G.S, the **Orthogonal Basis**, is just this:

![[vector.jpeg|500]]
Orthonormal Basis!  **⮵**

Just a fun way to transform two basis vectors into orthogonal vectors. Cool!