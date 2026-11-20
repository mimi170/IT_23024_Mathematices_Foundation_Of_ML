# IT_23024_Mathematices_Foundation_Of_ML
# Foundations for Machine Learning
## Lecture 2: Linear Algebra — Vector, Transformation, Span and Basis

---

# 1. Introduction to Linear Algebra

Linear Algebra is an important branch of mathematics that deals with vectors, matrices, linear equations and transformations.

It is one of the fundamental mathematical foundations of Machine Learning.

### Why is Linear Algebra important in Machine Learning?

Machine Learning models work with numerical data.

For example, a student dataset may contain:

- Age = 22
- Study hours = 6
- CGPA = 3.80

We can represent this information using a vector:

\[
x=\begin{bmatrix}22\\6\\3.80\end{bmatrix}
\]

In Machine Learning:

- Features are represented as vectors.
- Model parameters or weights are represented using vectors and matrices.
- Matrix multiplication is used to perform transformations.
- Vector spaces help us understand data dimensions.

Therefore, understanding Linear Algebra is essential for understanding Machine Learning and Deep Learning.

---

# 2. Understanding Vectors

### 2.1 What is a Vector?

A vector is a mathematical object that has:

1. Magnitude (length)
2. Direction

A vector can represent a physical quantity, a point in space or a list of numerical features.

In Linear Algebra, vectors are commonly represented as column vectors.

Example:

\[
v=\begin{bmatrix}3\\4\end{bmatrix}
\]

Here:
- Horizontal component = 3
- Vertical component = 4

This vector starts at the origin (0,0) and ends at (3,4).

### 2.2 Magnitude of a Vector

Magnitude means the length of a vector.

For a 2D vector:

\[
v=\begin{bmatrix}a\\b\end{bmatrix}
\]

Magnitude:

\[
\|v\|=\sqrt{a^2+b^2}
\]

Example:

\[
v=\begin{bmatrix}3\\4\end{bmatrix}
\]

\[
\|v\|=\sqrt{3^2+4^2}
\]

\[
=\sqrt{9+16}=\sqrt{25}=5
\]

Therefore, the magnitude is 5.

### 2.3 Vector Representation

A vector can be represented in different dimensions.

2D vector:

\[
v=\begin{bmatrix}2\\3\end{bmatrix}
\]

3D vector:

\[
v=\begin{bmatrix}2\\3\\4\end{bmatrix}
\]

n-dimensional vector:

\[
v=\begin{bmatrix}v_1\\v_2\\v_3\\ \vdots\\v_n\end{bmatrix}
\]

In Machine Learning, a dataset containing n features can be represented by an n-dimensional vector.

---

# 3. Vector Addition

### 3.1 Definition

Vector addition means adding the corresponding components of two or more vectors.

Suppose:

\[
x=\begin{bmatrix}3\\4\end{bmatrix}
\]

\[
y=\begin{bmatrix}2\\-1\end{bmatrix}
\]

Then:

\[
x+y=
\begin{bmatrix}3\\4\end{bmatrix}
+
\begin{bmatrix}2\\-1\end{bmatrix}
\]

\[
=\begin{bmatrix}3+2\\4-1\end{bmatrix}
\]

\[
=\begin{bmatrix}5\\3\end{bmatrix}
\]

### 3.2 Geometric Interpretation

Geometrically, vector addition can be understood as moving along one vector and then moving along another vector.

The resultant vector represents the final displacement from the starting point.

Important:
- Vector addition is performed component-wise.
- Both vectors must have the same dimensions.

### 3.3 Properties of Vector Addition

**Commutative property**

\[
x+y=y+x
\]

**Associative property**

\[
(x+y)+z=x+(y+z)
\]

**Zero vector property**

\[
x+0=x
\]

**Additive inverse**

\[
x+(-x)=0
\]

---

# 4. Scalar Multiplication

### 4.1 Definition

Scalar multiplication means multiplying every component of a vector by a scalar number.

A scalar is a single numerical value.

Suppose:

\[
v=\begin{bmatrix}2\\-1\end{bmatrix}
\]

Multiply by scalar 2:

\[
2v=2\begin{bmatrix}2\\-1\end{bmatrix}
\]

\[
=\begin{bmatrix}4\\-2\end{bmatrix}
\]

### 4.2 Geometric Interpretation

Scalar multiplication changes the magnitude of a vector.

- If scalar > 1: vector becomes longer.
- If 0 < scalar < 1: vector becomes shorter.
- If scalar = 0: vector becomes zero vector.
- If scalar < 0: vector reverses its direction.

Example:

\[
v=\begin{bmatrix}2\\3\end{bmatrix}
\]

\[
-2v=\begin{bmatrix}-4\\-6\end{bmatrix}
\]

The direction is reversed and the magnitude becomes twice as large.

### 4.3 Properties

\[
a(u+v)=au+av
\]

\[
(a+b)v=av+bv
\]

\[
a(bv)=(ab)v
\]

\[
1v=v
\]

---

# 5. Unit Vectors and Standard Basis

### 5.1 What is a Unit Vector?

A unit vector is a vector whose magnitude is exactly 1.

\[
\|v\|=1
\]

In 2D, the standard unit vectors are:

\[
i=\begin{bmatrix}1\\0\end{bmatrix}
\]

\[
j=\begin{bmatrix}0\\1\end{bmatrix}
\]

Here:
- i represents the horizontal x-direction.
- j represents the vertical y-direction.

### 5.2 Expressing a Vector Using Unit Vectors

Consider:

\[
v=\begin{bmatrix}3\\4\end{bmatrix}
\]

It can be expressed as:

\[
v=3i+4j
\]

Because:

\[
3\begin{bmatrix}1\\0\end{bmatrix}
+
4\begin{bmatrix}0\\1\end{bmatrix}
=
\begin{bmatrix}3\\4\end{bmatrix}
\]

This is called expressing a vector as a linear combination of other vectors.

---

# 6. Linear Combination

### Definition

A linear combination is an expression formed by multiplying vectors by scalar coefficients and then adding the results.

For vectors u and v:

\[
w=au+bv
\]

Where:
- a and b are scalars.
- u and v are vectors.
- w is the resulting vector.

Example:

\[
u=\begin{bmatrix}1\\0\end{bmatrix}
,\quad
v=\begin{bmatrix}0\\1\end{bmatrix}
\]

Let a = 3 and b = 4.

\[
w=3u+4v
\]

\[
=\begin{bmatrix}3\\0\end{bmatrix}
+
\begin{bmatrix}0\\4\end{bmatrix}
\]

\[
=\begin{bmatrix}3\\4\end{bmatrix}
\]

Therefore, the vector (3,4) is a linear combination of u and v.

---

# 7. Span of Vectors

### 7.1 Definition

The span of a set of vectors is the set of all possible vectors that can be obtained through their linear combinations.

For vectors u and v:

\[
Span(u,v)=\{au+bv\mid a,b\in\mathbb R\}
\]

In simple words, span describes all the positions that we can reach using the given vectors and their scalar multiples.

### 7.2 Span in 2D

**Case 1: Two non-parallel vectors**

Two non-parallel vectors in 2D span the entire 2D plane.

For example:

\[
u=\begin{bmatrix}1\\0\end{bmatrix}
,\quad
v=\begin{bmatrix}0\\1\end{bmatrix}
\]

Any 2D vector can be expressed as:

\[
w=au+bv
\]

Therefore:

\[
Span(u,v)=\mathbb R^2
\]

**Case 2: Two parallel vectors**

If two vectors are parallel, they span only a line passing through the origin.

Example:

\[
u=\begin{bmatrix}1\\2\end{bmatrix}
,\quad
v=\begin{bmatrix}2\\4\end{bmatrix}
\]

Because:

\[
v=2u
\]

Both vectors point in the same direction.

Therefore, their span is a one-dimensional line, not the entire 2D plane.

### 7.3 Span in 3D

In 3D:

- One non-zero vector generally spans a line.
- Two linearly independent vectors span a plane through the origin.
- Three linearly independent vectors span the entire 3D space.

Example:

\[
u=\begin{bmatrix}1\\0\\0\end{bmatrix}
\]

\[
v=\begin{bmatrix}0\\1\\0\end{bmatrix}
\]

\[
w=\begin{bmatrix}0\\0\\1\end{bmatrix}
\]

These three vectors span the entire 3D space.

---

# 8. Linear Independence and Linear Dependence

### 8.1 Linear Independence

A set of vectors is linearly independent if none of its vectors can be expressed as a linear combination of the remaining vectors.

Mathematically:

\[
a_1v_1+a_2v_2+\cdots+a_nv_n=0
\]

The vectors are linearly independent if the only solution is:

\[
a_1=a_2=\cdots=a_n=0
\]

Example:

\[
v_1=\begin{bmatrix}1\\0\end{bmatrix}
,\quad
v_2=\begin{bmatrix}0\\1\end{bmatrix}
\]

Neither vector can be obtained by scaling the other.

Therefore, they are linearly independent.

### 8.2 Linear Dependence

A set of vectors is linearly dependent if at least one vector can be represented as a linear combination of the others.

Example:

\[
v_1=\begin{bmatrix}1\\2\end{bmatrix}
\]

\[
v_2=\begin{bmatrix}2\\4\end{bmatrix}
\]

Here:

\[
v_2=2v_1
\]

Therefore, the vectors are linearly dependent.

### 8.3 Important Geometric Understanding

In 2D:
- Two non-parallel vectors are independent.
- Two parallel non-zero vectors are dependent.

In 3D:
- Three vectors that lie in the same plane through the origin are dependent.
- Three vectors that do not lie in the same plane are independent.

Important: Linear independence means that no vector in the set is redundant.

---

# 9. Basis of a Vector Space

### 9.1 Definition

A basis is a set of vectors that satisfies two conditions:

1. The vectors are linearly independent.
2. The vectors span the entire vector space.

Both conditions are necessary.

### 9.2 Standard Basis in 2D

The standard basis vectors are:

\[
e_1=\begin{bmatrix}1\\0\end{bmatrix}
\]

\[
e_2=\begin{bmatrix}0\\1\end{bmatrix}
\]

They are linearly independent and span the entire 2D plane.

Therefore:

\[
\{e_1,e_2\}
\]

is a basis for \(\mathbb R^2\).

### 9.3 Standard Basis in 3D

\[
e_1=\begin{bmatrix}1\\0\\0\end{bmatrix}
\]

\[
e_2=\begin{bmatrix}0\\1\\0\end{bmatrix}
\]

\[
e_3=\begin{bmatrix}0\\0\\1\end{bmatrix}
\]

These vectors form a basis for \(\mathbb R^3\).

### 9.4 Different Bases

A vector space can have different possible bases.

For example, consider:

\[
u=\begin{bmatrix}1\\1\end{bmatrix}
,\quad
v=\begin{bmatrix}1\\-1\end{bmatrix}
\]

These vectors are not parallel, so they are linearly independent.

They also span the entire 2D plane.

Therefore, they form another valid basis for \(\mathbb R^2\).

A vector can have different coordinates depending on which basis is used.

---

# 10. Dimension of a Vector Space

### Definition

The dimension of a vector space is the number of vectors in any basis of that space.

Examples:

\[
dim(\mathbb R^2)=2
\]

\[
dim(\mathbb R^3)=3
\]

\[
dim(\mathbb R^n)=n
\]

Important points:

- Dimension depends on the number of independent directions.
- Adding a redundant vector does not increase dimension.
- Adding a vector outside the existing span can increase dimension.

For example:
- A line has dimension 1.
- A plane has dimension 2.
- 3D space has dimension 3.

---

# 11. Linear Transformation — Basic Understanding

A linear transformation is a mapping between vector spaces that preserves vector addition and scalar multiplication.

Let T be a transformation.

It must satisfy:

### Addition property

\[
T(u+v)=T(u)+T(v)
\]

### Scalar multiplication property

\[
T(cv)=cT(v)
\]

These two properties define a linear transformation.

### Example: Scaling Transformation

Suppose:

\[
T(x,y)=(2x,2y)
\]

For vector:

\[
v=\begin{bmatrix}3\\4\end{bmatrix}
\]

Then:

\[
T(v)=\begin{bmatrix}6\\8\end{bmatrix}
\]

The vector becomes twice as long, but its direction remains the same.

### Transformation in Machine Learning

In Machine Learning, a transformation can change the representation of input data.

For example:

\[
y=Wx
\]

Where:
- x = input feature vector
- W = weight matrix
- y = transformed output vector

Matrix multiplication is an important way to represent linear transformations.

This concept becomes especially important in neural networks.

---

# 12. Connection Between These Concepts and Machine Learning

| Linear Algebra Concept | Machine Learning Application |
|---|---|
| Vector | Feature representation |
| Vector Addition | Combining numerical representations |
| Scalar Multiplication | Scaling feature values |
| Linear Combination | Combining features |
| Span | Understanding representable feature space |
| Linear Independence | Detecting redundant features |
| Basis | Representing a space efficiently |
| Dimension | Number of independent features |
| Linear Transformation | Neural network operations |

### Practical Example

Suppose a dataset contains three features:

\[
x=\begin{bmatrix}
Age\\
StudyHours\\
CGPA
\end{bmatrix}
\]

A Machine Learning model can transform this feature vector using a weight matrix:

\[
y=Wx
\]

This produces a new numerical representation.

Understanding vectors, bases, spans and transformations helps us understand what happens mathematically inside ML models.

---

# 13. Important Formulas — Quick Revision

**Vector magnitude**

\[
\|v\|=\sqrt{x^2+y^2}
\]

**Vector addition**

\[
\begin{bmatrix}a\\b\end{bmatrix}
+
\begin{bmatrix}c\\d\end{bmatrix}
=
\begin{bmatrix}a+c\\b+d\end{bmatrix}
\]

**Scalar multiplication**

\[
k\begin{bmatrix}a\\b\end{bmatrix}
=
\begin{bmatrix}ka\\kb\end{bmatrix}
\]

**Linear combination**

\[
w=au+bv
\]

**Span**

\[
Span(v_1,\ldots,v_n)
=
\left\{\sum_{i=1}^{n}a_iv_i\right\}
\]

**Linear independence**

\[
\sum_{i=1}^{n}a_iv_i=0
\]

Only the trivial solution is possible.

**Linear transformation**

\[
T(u+v)=T(u)+T(v)
\]

\[
T(cv)=cT(v)
\]

**Matrix transformation**

\[
y=Wx
\]

---

# 14. Important Viva Questions and Answers

**Q1. What is a vector?**

A vector is a mathematical quantity that has magnitude and direction.

**Q2. What is a scalar?**

A scalar is a single numerical value that has magnitude but no direction.

**Q3. What is vector addition?**

It is the operation of adding corresponding components of two vectors.

**Q4. What is scalar multiplication?**

It means multiplying every component of a vector by a scalar.

**Q5. What is a unit vector?**

A vector whose magnitude is exactly 1.

**Q6. What is a linear combination?**

A combination of vectors formed by scalar multiplication and addition.

**Q7. What is span?**

Span is the set of all possible linear combinations of a given set of vectors.

**Q8. What is linear independence?**

A set of vectors is linearly independent if no vector can be represented as a linear combination of the others.

**Q9. What is linear dependence?**

A set of vectors is dependent if at least one vector can be represented using the others.

**Q10. What is a basis?**

A basis is a linearly independent set of vectors that spans the entire vector space.

**Q11. What is the dimension of a vector space?**

It is the number of vectors in a basis of that space.

**Q12. Can a vector space have multiple bases?**

Yes. A vector space can have many different valid bases.

**Q13. How many vectors are required to form a basis of R²?**

Two linearly independent vectors.

**Q14. How many vectors are required to form a basis of R³?**

Three linearly independent vectors.

**Q15. Why is Linear Algebra important in ML?**

It helps represent data, perform transformations, combine features and understand neural network computations.

---

# 15. Practice Problems

### Problem 1: Vector Addition

Given:

\[
u=\begin{bmatrix}2\\3\end{bmatrix},
v=\begin{bmatrix}4\\1\end{bmatrix}
\]

Find u + v.

**Answer:**

\[
u+v=\begin{bmatrix}6\\4\end{bmatrix}
\]

### Problem 2: Scalar Multiplication

Given:

\[
v=\begin{bmatrix}3\\5\end{bmatrix}
\]

Find 3v.

**Answer:**

\[
3v=\begin{bmatrix}9\\15\end{bmatrix}
\]

### Problem 3: Magnitude

Given:

\[
v=\begin{bmatrix}6\\8\end{bmatrix}
\]

Find its magnitude.

**Answer:**

\[
\|v\|=\sqrt{36+64}=10
\]

### Problem 4: Linear Dependence

Given:

\[
u=\begin{bmatrix}1\\2\end{bmatrix}
,\quad
v=\begin{bmatrix}3\\6\end{bmatrix}
\]

Are these vectors independent?

**Answer:**

No.

Because:

\[
v=3u
\]

They are linearly dependent.

### Problem 5: Basis

Do the following vectors form a basis of R²?

\[
u=\begin{bmatrix}1\\0\end{bmatrix},
v=\begin{bmatrix}0\\1\end{bmatrix}
\]

**Answer:** Yes. They are linearly independent and span R².

---

# 16. Final Summary

The most important concepts from this lecture are:

1. Vectors represent numerical information and directions.
2. Vector addition combines vectors.
3. Scalar multiplication changes vector magnitude and possibly direction.
4. Linear combinations express vectors using other vectors.
5. Span describes all possible vectors reachable through linear combinations.
6. Linear independence means there are no redundant vectors.
7. Basis is a linearly independent set that spans a vector space.
8. Dimension counts the number of vectors in a basis.
9. Linear transformations map vectors while preserving addition and scalar multiplication.

**Most important relationship:**

Basis = Linear Independence + Span

These concepts are the foundation for understanding matrix operations, neural networks, dimensionality reduction and Machine Learning.
