## 1. Vectors

A **vector** is a mathematical quantity that has both magnitude and direction. In linear algebra and machine learning, vectors are used to represent data points, features, and directions in space.

A vector can be written as:

$$
\mathbf{v} =
\begin{bmatrix}
v_1 \\
v_2 \\
\vdots \\
v_n
\end{bmatrix}
$$

Example:

$$
\mathbf{v} =
\begin{bmatrix}
2 \\
3
\end{bmatrix}
$$

This is a two-dimensional vector with components 2 and 3.

### 1.1 Vector Representation

A vector can be represented geometrically as an arrow.

- The length of the arrow represents its magnitude.
- The arrowhead represents its direction.
- The starting point is usually the origin.

For a two-dimensional vector:

$$
\mathbf{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

Here, x and y represent the horizontal and vertical components.

## 2. Vector Addition

Vector addition means adding the corresponding components of two or more vectors.

Let:

$$
\mathbf{a} =
\begin{bmatrix}
a_1 \\
a_2
\end{bmatrix}
\qquad
\mathbf{b} =
\begin{bmatrix}
b_1 \\
b_2
\end{bmatrix}
$$

Their sum is:

$$
\mathbf{a} + \mathbf{b}
=
\begin{bmatrix}
a_1 + b_1 \\
a_2 + b_2
\end{bmatrix}
$$

**Example:**

$$
\mathbf{a} =
\begin{bmatrix}
2 \\
3
\end{bmatrix}
\qquad
\mathbf{b} =
\begin{bmatrix}
4 \\
1
\end{bmatrix}
$$

Therefore:

$$
\mathbf{a} + \mathbf{b}
=
\begin{bmatrix}
2 + 4 \\
3 + 1
\end{bmatrix}
=
\begin{bmatrix}
6 \\
4
\end{bmatrix}
$$

### 2.1 Geometric Interpretation

Vector addition can be visualized using the head-to-tail method:

1. Draw the first vector.
2. Place the starting point of the second vector at the endpoint of the first.
3. Draw a new vector from the starting point of the first vector to the endpoint of the second.

The resulting vector represents the sum.

## 3. Scalar Multiplication

Scalar multiplication means multiplying every component of a vector by a scalar (a real number).

Let:

$$
\mathbf{v} =
\begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
$$

For a scalar c:

$$
c\mathbf{v}
=
\begin{bmatrix}
cv_1 \\
cv_2
\end{bmatrix}
$$

**Example:**

$$
\mathbf{v} =
\begin{bmatrix}
2 \\
3
\end{bmatrix}
\qquad
c = 2
$$

Then:

$$
2\mathbf{v}
=
2
\begin{bmatrix}
2 \\
3
\end{bmatrix}
=
\begin{bmatrix}
4 \\
6
\end{bmatrix}
$$

A positive scalar changes the magnitude while maintaining the direction. A negative scalar reverses the direction.

## 4. Magnitude (Norm) of a Vector

The magnitude or length of a vector is called its **norm**.

For a two-dimensional vector:

$$
\mathbf{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

Its Euclidean norm is:

$$
\|\mathbf{v}\| = \sqrt{x^2 + y^2}
$$

For an n-dimensional vector:

$$
\|\mathbf{v}\|_2
=
\sqrt{\sum_{i=1}^{n} v_i^2}
$$

**Example:**

$$
\mathbf{v} =
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

$$
\|\mathbf{v}\|
=
\sqrt{3^2 + 4^2}
$$

$$
=
\sqrt{9 + 16}
=
\sqrt{25}
=
5
$$

## 5. Unit Vector

A unit vector is a vector whose magnitude is exactly 1.

A unit vector in the direction of a non-zero vector v is calculated by dividing the vector by its magnitude.

$$
\hat{\mathbf{v}}
=
\frac{\mathbf{v}}{\|\mathbf{v}\|}
$$

**Example:**

$$
\mathbf{v} =
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

Since:

$$
\|\mathbf{v}\| = 5
$$

The unit vector is:

$$
\hat{\mathbf{v}}
=
\frac{1}{5}
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
3/5 \\
4/5
\end{bmatrix}
$$

Its magnitude is 1.

## 6. Linear Combination

A linear combination is formed by multiplying vectors by scalars and then adding the results.

For vectors v₁, v₂, ..., vₙ, a linear combination is:

$$
\mathbf{v}
=
c_1\mathbf{v}_1
+
c_2\mathbf{v}_2
+
\cdots
+
c_n\mathbf{v}_n
$$

Where:

- v₁, v₂, ..., vₙ are vectors.
- c₁, c₂, ..., cₙ are scalar coefficients.
- v is the resulting vector.

**Example:**

Let:

$$
\mathbf{v}_1 =
\begin{bmatrix}
1 \\
0
\end{bmatrix}
\qquad
\mathbf{v}_2 =
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

Choose coefficients:

$$
c_1 = 3
\qquad
c_2 = 2
$$

Then:

$$
3\mathbf{v}_1 + 2\mathbf{v}_2
=
3
\begin{bmatrix}
1 \\
0
\end{bmatrix}
+
2
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
3 \\
0
\end{bmatrix}
+
\begin{bmatrix}
0 \\
2
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
3 \\
2
\end{bmatrix}
$$

## 7. Span of Vectors

The **span** of a set of vectors is the set of all possible linear combinations of those vectors.

For two vectors v₁ and v₂:

$$
\operatorname{Span}\{\mathbf{v}_1,\mathbf{v}_2\}
=
\left\{
c_1\mathbf{v}_1 + c_2\mathbf{v}_2
\mid
c_1,c_2 \in \mathbb{R}
\right\}
$$

The span describes all the vectors that can be generated using the given vectors and scalar coefficients.

### 7.1 Span in Two Dimensions

Consider:

$$
\mathbf{v}_1 =
\begin{bmatrix}
1 \\
0
\end{bmatrix}
\qquad
\mathbf{v}_2 =
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

Any vector in two-dimensional space can be expressed as:

$$
\begin{bmatrix}
x \\
y
\end{bmatrix}
=
x
\begin{bmatrix}
1 \\
0
\end{bmatrix}
+
y
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

Therefore, these two vectors span the entire two-dimensional plane:

$$
\operatorname{Span}\{\mathbf{v}_1,\mathbf{v}_2\}
=
\mathbb{R}^2
$$

## 8. Linear Independence

A set of vectors is **linearly independent** if no vector in the set can be expressed as a linear combination of the other vectors.

Mathematically, vectors v₁, v₂, ..., vₙ are linearly independent if:

$$
c_1\mathbf{v}_1
+
c_2\mathbf{v}_2
+
\cdots
+
c_n\mathbf{v}_n
=
\mathbf{0}
$$

has only the trivial solution:

$$
c_1 = c_2 = \cdots = c_n = 0
$$

**Example:**

$$
\mathbf{v}_1 =
\begin{bmatrix}
1 \\
0
\end{bmatrix}
\qquad
\mathbf{v}_2 =
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

If:

$$
c_1
\begin{bmatrix}
1 \\
0
\end{bmatrix}
+
c_2
\begin{bmatrix}
0 \\
1
\end{bmatrix}
=
\begin{bmatrix}
0 \\
0
\end{bmatrix}
$$

Then:

$$
\begin{bmatrix}
c_1 \\
c_2
\end{bmatrix}
=
\begin{bmatrix}
0 \\
0
\end{bmatrix}
$$

Thus:

$$
c_1 = 0
\qquad
c_2 = 0
$$

The vectors are linearly independent.

## 9. Linear Dependence

A set of vectors is **linearly dependent** if at least one vector can be expressed as a linear combination of the other vectors.

The equation:

$$
c_1\mathbf{v}_1
+
c_2\mathbf{v}_2
+
\cdots
+
c_n\mathbf{v}_n
=
\mathbf{0}
$$

has at least one non-zero coefficient in a solution.

**Example:**

$$
\mathbf{v}_1 =
\begin{bmatrix}
1 \\
2
\end{bmatrix}
\qquad
\mathbf{v}_2 =
\begin{bmatrix}
2 \\
4
\end{bmatrix}
$$

Notice that:

$$
\mathbf{v}_2 = 2\mathbf{v}_1
$$

Therefore, the second vector is a scalar multiple of the first vector. These vectors are linearly dependent.

## 10. Basis

A **basis** is a set of vectors that satisfies two conditions:

1. The vectors are linearly independent.
2. The vectors span the entire vector space.

For example, the standard basis of R² is:

$$
\mathbf{e}_1 =
\begin{bmatrix}
1 \\
0
\end{bmatrix}
\qquad
\mathbf{e}_2 =
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

Every vector in R² can be represented using these two basis vectors:

$$
\begin{bmatrix}
x \\
y
\end{bmatrix}
=
x\mathbf{e}_1 + y\mathbf{e}_2
$$

The standard basis of R³ is:

$$
\mathbf{e}_1 =
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$$

$$
\mathbf{e}_2 =
\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix}
$$

$$
\mathbf{e}_3 =
\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}
$$

## 11. Dimension of a Vector Space

The dimension of a vector space is the number of vectors in any basis of that space.

Examples:

$$
\dim(\mathbb{R}^2) = 2
$$

$$
\dim(\mathbb{R}^3) = 3
$$

$$
\dim(\mathbb{R}^n) = n
$$

A two-dimensional vector space requires two linearly independent basis vectors. A three-dimensional vector space requires three linearly independent basis vectors.

## 12. Linear Transformation

A **linear transformation** is a function that maps vectors from one vector space to another while preserving vector addition and scalar multiplication.

Let T be a transformation. It is linear if it satisfies the following two properties.

### 12.1 Preservation of Vector Addition

$$
T(\mathbf{u}+\mathbf{v})
=
T(\mathbf{u})+T(\mathbf{v})
$$

### 12.2 Preservation of Scalar Multiplication

$$
T(c\mathbf{v})
=
cT(\mathbf{v})
$$

Combining these properties:

$$
T(a\mathbf{u}+b\mathbf{v})
=
aT(\mathbf{u})+bT(\mathbf{v})
$$

Here, a and b are scalars.

### 12.3 Matrix Representation

A linear transformation can be represented using a matrix.

$$
T(\mathbf{x}) = A\mathbf{x}
$$

Where:

- A is the transformation matrix.
- x is the input vector.
- T(x) is the transformed vector.

**Example:**

Let:

$$
A =
\begin{bmatrix}
2 & 0 \\
0 & 3
\end{bmatrix}
\qquad
\mathbf{x} =
\begin{bmatrix}
1 \\
2
\end{bmatrix}
$$

Then:

$$
T(\mathbf{x}) = A\mathbf{x}
$$

$$
=
\begin{bmatrix}
2 & 0 \\
0 & 3
\end{bmatrix}
\begin{bmatrix}
1 \\
2
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
2(1)+0(2) \\
0(1)+3(2)
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
2 \\
6
\end{bmatrix}
$$

The transformation scales the first coordinate by 2 and the second coordinate by 3.

### 12.4 Common Linear Transformations

**Scaling:** Changes the size of a vector.

$$
A =
\begin{bmatrix}
a & 0 \\
0 & b
\end{bmatrix}
$$

**Rotation:** Rotates a vector by an angle θ.

$$
R(\theta) =
\begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
$$

**Reflection:** Reflects a vector across an axis. Reflection across the x-axis is represented by:

$$
A =
\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
$$

**Projection:** Maps a vector onto a specified line or subspace.

For projection onto the x-axis:

$$
P =
\begin{bmatrix}
1 & 0 \\
0 & 0
\end{bmatrix}
$$

## 13. Vectors and Linear Transformations in Machine Learning

Vectors and linear transformations are important mathematical foundations of machine learning.

- **Data representation:** A data sample can be represented as a vector of numerical features.
- **Feature vectors:** Each feature represents one property of a data sample.
- **Weight vectors:** Machine learning models use weights to determine the importance of features.
- **Linear combinations:** Model predictions can be calculated by combining input features with their corresponding weights.
- **Matrix operations:** Matrices and vectors are used to perform transformations efficiently.
- **Dimensionality:** Vector spaces provide a mathematical foundation for representing and processing data with different numbers of features.
