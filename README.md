# IT_23024_Mathematices_Foundation_Of_ML
# Foundations for Machine Learning
## Lecture 2: Linear Algebra

**Source:** [Vizuara – Lecture 2](https://youtu.be/llV4uj58wuA)

---

## 1. Vector

A vector is a mathematical object that has both magnitude and direction. It is represented by an ordered collection of numbers.

For example,

$$
x = \begin{bmatrix}3\\4\end{bmatrix}
$$

Here, 3 represents the horizontal component and 4 represents the vertical component.

A vector can be represented geometrically as an arrow starting from the origin (0,0) and ending at the point (3,4).

**Magnitude of a Vector:**

The magnitude or length of a vector is calculated using:

$$
|x| = \sqrt{x_1^2+x_2^2}
$$

For the given example:

$$
|x| = \sqrt{3^2+4^2}
$$

$$
= \sqrt{25}=5
$$



## 2. Vector Addition

Vector addition is the operation of adding two or more vectors by adding their corresponding components.

Suppose,

$$
x = \begin{bmatrix}3\\4\end{bmatrix},
\quad
y = \begin{bmatrix}2\\-1\end{bmatrix}
$$

Then,

$$
x+y =
\begin{bmatrix}
3+2\\
4+(-1)
\end{bmatrix}
$$

$$
\boxed{x+y=\begin{bmatrix}5\\3\end{bmatrix}}
$$

Geometrically, vector addition can be represented using the head-to-tail method. The resultant vector connects the starting point of the first vector to the endpoint of the second vector.



## 3. Scalar Multiplication

Scalar multiplication means multiplying a vector by a single numerical value called a scalar.

Suppose,

$$
y = \begin{bmatrix}2\\-1\end{bmatrix}
$$

Multiplying by scalar 2:

$$
2y = 2\begin{bmatrix}2\\-1\end{bmatrix}
$$

$$
\boxed{2y=\begin{bmatrix}4\\-2\end{bmatrix}}
$$

Scalar multiplication changes the magnitude of a vector. A positive scalar preserves its direction, while a negative scalar reverses its direction.



## 4. Unit Vectors and Vector Decomposition

A unit vector is a vector whose magnitude is exactly equal to 1.

In a two-dimensional coordinate system, the standard unit vectors are:

$$
\hat{i}=\begin{bmatrix}1\\0\end{bmatrix}
$$

$$
\hat{j}=\begin{bmatrix}0\\1\end{bmatrix}
$$

Here, $\hat{i}$ represents the horizontal direction (x-axis), and $\hat{j}$ represents the vertical direction (y-axis).

**Vector Decomposition:**

Any two-dimensional vector can be expressed as a linear combination of these two unit vectors.

$$
v=\begin{bmatrix}a\\b\end{bmatrix}
=a\hat{i}+b\hat{j}
$$

For example,

$$
v=\begin{bmatrix}3\\4\end{bmatrix}
=3\hat{i}+4\hat{j}
$$

This process is called vector decomposition because the vector is expressed through its individual components.



## 5. Basis Vectors

A basis is a set of linearly independent vectors that can generate the entire vector space through linear combinations.

The standard basis of two-dimensional space consists of:

$$
e_1=\begin{bmatrix}1\\0\end{bmatrix},
\quad
e_2=\begin{bmatrix}0\\1\end{bmatrix}
$$

Any vector in 2D space can be represented using these two basis vectors.

$$
v=\begin{bmatrix}a\\b\end{bmatrix}
=ae_1+be_2
$$

A basis must satisfy two conditions:

1. Its vectors must be linearly independent.
2. Its vectors must span the entire vector space.

## 6. Span of Vectors

The span of a set of vectors is the set of all possible vectors that can be obtained through linear combinations of those vectors.

For two vectors $v_1$ and $v_2$:

$$
Span(v_1,v_2)=
\{av_1+bv_2\mid a,b\in\mathbb{R}\}
$$

**Example 1: Two Independent Vectors**

Suppose,

$$
v_1=\begin{bmatrix}1\\0\end{bmatrix},
\quad
v_2=\begin{bmatrix}0\\1\end{bmatrix}
$$

Any vector $(a,b)$ can be generated using:

$$
(a,b)=a(1,0)+b(0,1)
$$

Therefore, these two vectors span the entire two-dimensional plane.

![Span of Independent Vectors](images/05_span_plane.png)

**Example 2: Two Parallel Vectors**

Suppose,

$$
v_1=\begin{bmatrix}1\\2\end{bmatrix},
\quad
v_2=\begin{bmatrix}2\\4\end{bmatrix}
$$

Since,

$$
v_2=2v_1
$$

Both vectors lie along the same direction. Therefore, their span is only a straight line rather than the entire 2D plane.



## 7. Linear Independence and Dependence

Linear independence means that no vector in a set can be represented as a linear combination of the other vectors.

For example,

$$
v_1=(1,0), \quad v_2=(0,1)
$$

These vectors are linearly independent because neither vector can be generated from the other.

Linear dependence occurs when at least one vector can be represented as a linear combination of the other vectors.

For example,

$$
v_1=(1,2), \quad v_2=(2,4)
$$

Since,

$$
v_2=2v_1
$$

The vectors are linearly dependent.

Mathematically, a set of vectors is linearly independent if:

$$
a_1v_1+a_2v_2+\cdots+a_nv_n=0
$$

has only the trivial solution:

$$
a_1=a_2=\cdots=a_n=0
$$

If a non-zero solution exists, the vectors are linearly dependent.

## 8. Dimension of a Vector Space

The dimension of a vector space is the number of vectors in its basis.

Examples:

- A line has dimension 1.
- A two-dimensional plane has dimension 2.
- Three-dimensional space has dimension 3.

The dimension of a span is determined by the number of linearly independent vectors that generate it.

Adding a redundant vector does not increase the dimension.

## 9. Basis of Three-Dimensional Space

The standard basis vectors in three-dimensional space are:

$$
e_1=\begin{bmatrix}1\\0\\0\end{bmatrix}
$$

$$
e_2=\begin{bmatrix}0\\1\\0\end{bmatrix}
$$

$$
e_3=\begin{bmatrix}0\\0\\1\end{bmatrix}
$$

These three vectors represent the x, y and z directions respectively.

Any vector in 3D space can be represented as:

$$
v=ae_1+be_2+ce_3
$$

Therefore, three linearly independent vectors are required to form a basis of three-dimensional space.



