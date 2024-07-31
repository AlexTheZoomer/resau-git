---
title: Linear Algebra Review - ENGM 1041
draft: false
tags:
  - Mathematics ➗
---
Before we begin!

I would like to give a special thank you to

[Josh Latka](https://www.dal.ca/faculty/engineering/math-internetworking/people/people-profiles/josh-latka.html), Professor of Engineering Mathematics 

[Prime Newtons](https://www.youtube.com/c/PrimeNewtons), Mathematical Education on YouTube

[David James "Dave" Farina](https://www.youtube.com/professordaveexplains) Mathematical Education 

For their contributions in Mathematical education, and provision of knowledge for this document.

---
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

### <u>Linear Combination, Span, Linear Independence</u>

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

### <u>Basis and Dimension</u>

#### Basis  

- Basis are the vectors which make up a dimension 

![[Pasted image 20240409110012.png|400]]

- If you are given a vector set, like this, you have to check for linear independence. Just because you have four vectors, doesn't mean that one, two or even three could be dependent on the first.

- To solve for the basis vectors, or the ones that actually matter to the system, you have to do REF to see if you have a zero row.

![[Pasted image 20240409110225.png]]

- So here, only the first three vectors matter (They are inserted by row here)

$$
\begin{bmatrix}
1 &1 &-2 &0 &-1 \\
1 &2 &0 &-4 &1 \\
0 &1 &3 &-3 &2
\end{bmatrix}
$$

As such! 
- These are our basis vectors. The last one is dependent. 

#### Row Space

- Row space is loading the vectors into the matrix by ***ROW*** and doing REF to find the amount of not zero rows

- The amount of pivot rows denote the amount of basis vectors. 

![[Pasted image 20240409110225.png]]

The example used just now was row space! 
- The vectors given post REF are the **basis for row space**. 

#### Column Space

- Row space is loading the vectors into the matrix by ***COLUMN*** and doing REF to find the amount of pivots

![[Pasted image 20240409112430.png|400]]

- Here! The **final row** does not have a pivot. Therefore, it is not a basis! ℝ<sup>3</sup>
- You must go back to the original vectors to give, as column space does not give REF'ed vectors.

---
#### Dimension

Dimension is easy! The dimension, ℝ<sup>n</sup> is defined by the number of basis vectors. 

### <u>Orthogonal Sets in Rn</u>

 To begin, it is important to know that "Orthogonal" just means to be perpendicular to something. 

![[Pasted image 20240409174616.png|300]]

- Here, **b̂** and **â** are orthogonal, perpendicular!

To check if two vectors are orthogonal, one can take the dot product. 
- If the dot product does not equal zero, well... **b̂** and **â** aren't orthogonal
- However, if it **does**, then **b̂** and **â** are orthogonal! 
- This occurs, because the cos term in the dot product operation is at **90°**. Cos(90) = 0


![[Pasted image 20240409175233.png|400]]

- Here is an example where that is the case!

##### Orthonormality 

If vectors **b̂** and **â** are:
1) A unit vector (length of 1)
2) Orthogonal 

They are what is known as **orthonormal**

- A reminder, to get the unit vector, it is the vector divided by its magnitude

$$
\frac{\vec{a}}{\sqrt{\vec{a^2}}} = \hat{a}
$$
- Example!

![[Pasted image 20240409180703.png|400]]

---
Now, you can also have ***spaces*** that are orthogonal to each other.
- Pretty cool!

![[Pasted image 20240409181007.png|400]]

What is happening here, is that we have a subspace ***A*** and a subspace ***B***
- Subspace ***A*** is only taking up the first row of the vector defining the space.
- Subspace ***B*** is only is only taking up the second and third row of the vector defining the space.

So, if we take the dot product of the **b̂** and **â** vectors making up ***A*** and ***B***, as Dave does here, we will get zero! 
- If you remember from before, this makes them orthogonal!

--
##### Orthogonal Square Matrices

You can also check to see if square matrices are orthogonal

![[Pasted image 20240409181629.png|400]]

- This involves taking the dot products of each vector put into the matrix, and ensuring that they are orthonormal (*i.e. length of one, and orthogonal (dot product equals zero)*

##### Orthogonal Sets

An Orthogonal Set is pretty easy. 
- An orthogonal set is a set of vectors (two or more), that are all orthogonal!

![[Pasted image 20240409191028.png||400]]
*some steps skipped here, but each row is being multiplied, then they are all being added (dot product)

Every single vector has to be orthogonal to each other, with ***no exceptions***
- In this case, V<sub>2</sub> and V<sub>3</sub> failed, even if the rest are good, this is not an orthogonal set.

- Get the idea?

##### What you are REALLY here to see

- Well, that's cool and all, but what is the point in finding all of this? 
- The reason why is pretty unique, and quite helpful.

**For an orthogonal matrix (A) its inverse (A<sup>-1</sup>) is simply the same as its transpose (A<sup>T</sup>)**

![[Pasted image 20240409182823.png|400]]
![[Pasted image 20240409182844.png|400]]

- This makes it ***REALLY*** easy to find the inverse of an orthogonal matrix, quickly. You can just make the columns the rows, and the rows the columns 

--
<u>Last topic for Orthogonality!</u>

Another cool thing you can do, is find the orthogonality of ***functions***
- This is done by defining a new operation known as the <font color="#c00000">inner product</font>

Given ***f(x)***, and another function ***g(x)***, from a point ***a*** to a point ***b*** ~

- The operation looks like this
$$
<f,g>
$$
- <f,g> is equal to the integral of ***f(x)*g(x)*** from point ***a*** to ***b***

$$
<f,g> = \int_{a}^{b}f(x)g(x)dx
$$
- Cool stuff!

- Now, if this <font color="#c00000">inner product</font> is = 0, then the <u>functions are orthogonal</u> over the range **a** to **b**

Example!

![[Pasted image 20240409184739.png|400]]

- Here, ***f(x)*** and ***g(x)*** are orthogonal over the range of (*-1 to 1*), but <font color="#ffff00">not</font> (*0 to 1*)
---
Wrapping up here, but as a hint for later, another ***w(x)*** function can be thrown in here (weight function) to vary things up. 

We will see this later!!!
### <u>Gram-Schmidt, QR Decomposition, Orthogonal Sets and Subspaces</u>

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

---
##### QR Decomposition 

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
Why is this useful?
### <u>Best Approximation and Complex Numbers</u>

##### Complex Numbers

Complex numbers are a funny thing. Complex numbers are numbers that are made up a "real component", and an "imaginary component".

Let Z = A complex number

$$
Z = X + iY
$$

There also exists what is known as the ***complex conjugate***. The complex conjugate is described as:

$$
\bar{Z} = X - iY
$$


- X and Y are real numbers, with i being an *imaginary component*. Y here is scaling the imaginary component.

 To find the magnitude of Z, you can 
 $$
 |Z| = \sqrt{a^2 +b^2}
 $$

![[Pasted image 20240410120050.png|300]]
$$
i = \sqrt{-1}
$$
$$
i^2 = -1
$$
Complex numbers can be:

- Added
- Subtracted
- Multiplied 
- Divided

Complex numbers can also be found in **polar form**. **Polar form is made up of:**
$$
z = |z|e^{i\theta}
$$

The magnitude of Z, times *Euler's formula*. *Euler's formula* is:
$$
e^{i\theta}=cos\theta + isin\theta
$$
-

The last thing to talk about here, is **Demoivre's Theorem**.
$$
(e^{i\theta})^n = e^{in\theta}
$$ 
It is a method of proving trigonometric identities.

![[Pasted image 20240410122534.png]]

 ---
##### Best Approximation

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
### <u>General Vector Spaces </u>

- LeGrange polynomials 
- 
![[Pasted image 20240411115654.png|400]]

LaGrange polynomials are a funny thing, and come with a little bit of work.

![[Pasted image 20240411171356.png|300]]

What is happening, is you are creating a polynomial for each point on the plane, and adding them all up. You can literally create the original polynomial from these other ones. Each point in the LeGrange polynomial process starts at a magnitude of one, and you multiply it by a scalar (Y value) to fit it. 

- You will be given X points, and a Y = Sin(x), or (X,Y) coordinate points
- The Y value given, or found, is representative of the scalar. 

![[Pasted image 20240411172935.png|400]]

- Plug in X values like this, in this order. 
- I don't know how to explain this 😭

### Differential Equations, and Inner Products 
![[Pasted image 20240411113246.png|400]]

### Weighted Least Squares, Best Approximations of Functions

##### Best Approximations of Functions

- The same thing as before, but using polynomials turned into vectors, and inner product. 
- Remember, you are projecting a vector onto a known basis. G.S. is needed to find a basis.

![[Pasted image 20240411113450.png|400]]

## <font color="#ffff00">Extras (MATLAB, Past Material, ETC)</font>

[MATLAB® Basic Functions Reference](https://www.mathworks.com/content/dam/mathworks/fact-sheet/matlab-basic-functions-reference.pdf)

#### Addition

|   |   |
|---|---|
|[`+`](https://www.mathworks.com/help/matlab/ref/plus.html)|Add numbers, append strings|
|[`sum`](https://www.mathworks.com/help/matlab/ref/sum.html)|Sum of array elements|
|[`cumsum`](https://www.mathworks.com/help/matlab/ref/cumsum.html)|Cumulative sum|
|[`movsum`](https://www.mathworks.com/help/matlab/ref/movsum.html)|Moving sum|

#### Subtraction

|   |   |
|---|---|
|[`-`](https://www.mathworks.com/help/matlab/ref/minus.html)|Subtraction|
|[`diff`](https://www.mathworks.com/help/matlab/ref/diff.html)|Differences and approximate derivatives|

#### Multiplication

|   |   |
|---|---|
|[`.*`](https://www.mathworks.com/help/matlab/ref/times.html)|Multiplication|
|[`*`](https://www.mathworks.com/help/matlab/ref/mtimes.html)|Matrix multiplication|
|[`prod`](https://www.mathworks.com/help/matlab/ref/prod.html)|Product of array elements|
|[`cumprod`](https://www.mathworks.com/help/matlab/ref/cumprod.html)|Cumulative product|
|[`pagemtimes`](https://www.mathworks.com/help/matlab/ref/pagemtimes.html)|Page-wise matrix multiplication _(Since R2020b)_|
|[`tensorprod`](https://www.mathworks.com/help/matlab/ref/tensorprod.html)|Tensor products between two tensors _(Since R2022a)_|

#### Division

|   |   |
|---|---|
|[`./`](https://www.mathworks.com/help/matlab/ref/rdivide.html)|Right array division|
|[`.\`](https://www.mathworks.com/help/matlab/ref/ldivide.html)|Left array division|
|[`/`](https://www.mathworks.com/help/matlab/ref/mrdivide.html)|Solve systems of linear equations _xA = B_ for _x_|
|[`\`](https://www.mathworks.com/help/matlab/ref/mldivide.html)|Solve systems of linear equations _Ax = B_ for _x_|
|[`pagemldivide`](https://www.mathworks.com/help/matlab/ref/pagemldivide.html)|Page-wise left matrix divide _(Since R2022a)_|
|[`pagemrdivide`](https://www.mathworks.com/help/matlab/ref/pagemrdivide.html)|Page-wise right matrix divide _(Since R2022a)_|

#### Powers

|   |   |
|---|---|
|[`.^`](https://www.mathworks.com/help/matlab/ref/power.html)|Element-wise power|
|[`^`](https://www.mathworks.com/help/matlab/ref/mpower.html)|Matrix power|

#### Transpose

|   |   |
|---|---|
|[`.'`](https://www.mathworks.com/help/matlab/ref/transpose.html)|Transpose vector or matrix|
|[`'`](https://www.mathworks.com/help/matlab/ref/ctranspose.html)|Complex conjugate transpose|
|[`pagetranspose`](https://www.mathworks.com/help/matlab/ref/pagetranspose.html)|Page-wise transpose _(Since R2020b)_|
|[`pagectranspose`](https://www.mathworks.com/help/matlab/ref/pagectranspose.html)                                                                                                                                 | ---------------------------------------------------------------------------------------------------------------- | ----------- |---------------- | ----------- |--------------------------- | ------                                                - |
| [`uminus`]( <br>v<br><br><br><br><br><br><br><br><br><br><br>[`uplus`](https://www.mathworks.com/help/matlab/ref/uplus.html) m/help/matlab/ref/uplus.html) athworks.com/help/matlab/ref/uplus.html)   | Unary plus  |





[Derivations](https://dal.brightspace.com/d2l/le/content/307009/viewContent/4239831/View)
