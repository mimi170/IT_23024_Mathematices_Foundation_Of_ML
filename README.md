# IT_23024_Mathematices_Foundation_Of_ML
# Linear Algebra – Lecture 2
## Foundations for Machine Learning

### 1. Introduction to Vectors

A vector is a mathematical object that has both magnitude and direction. It is commonly represented as an ordered list of numbers.

For example:

$$
\vec{x}=\begin{bmatrix}3\\4\end{bmatrix}
$$

Here, the vector has two components: 3 and 4.

**Geometrical Representation of a Vector**

<p align="center">
  <img src="./images/01_vector.png" width="650" alt="Vector Representation">
</p>

---

### 2. Vector Addition

Vector addition means adding the corresponding components of two or more vectors.

Let,

$$
\vec{x}=\begin{bmatrix}3\\4\end{bmatrix},
\quad
\vec{y}=\begin{bmatrix}2\\-1\end{bmatrix}
$$

Then,

$$
\vec{x}+\vec{y}
=
\begin{bmatrix}3+2\\4+(-1)\end{bmatrix}
=
\begin{bmatrix}5\\3\end{bmatrix}
$$

**Geometrical Representation of Vector Addition**

<p align="center">
  <img src="./images/02_vector_addition.png" width="650" alt="Vector Addition">
</p>

---

### 3. Scalar Multiplication

Scalar multiplication means multiplying a vector by a real number (scalar). Each component of the vector is multiplied by that scalar.

Let,

$$
\vec{y}=\begin{bmatrix}2\\-1\end{bmatrix}
$$

Multiplying by 2:

$$
2\vec{y}
=
2\begin{bmatrix}2\\-1\end{bmatrix}
=
\begin{bmatrix}4\\-2\end{bmatrix}
$$

**Geometrical Representation of Scalar Multiplication**

<p align="center">
  <img src="./images/03_scalar_multiplication.png" width="650" alt="Scalar Multiplication">
</p>

---

### 4. Standard Basis Vectors

In two-dimensional space, the standard basis consists of two unit vectors:

$$
\vec{i}=\begin{bmatrix}1\\0\end{bmatrix},
\quad
\vec{j}=\begin{bmatrix}0\\1\end{bmatrix}
$$

Every vector in 2D space can be represented as a linear combination of these two basis vectors.

For example:

$$
\begin{bmatrix}3\\4\end{bmatrix}
=3\vec{i}+4\vec{j}
$$

**Geometrical Representation of Standard Basis Vectors**

<p align="center">
  <img src="./images/04_standard_basis.png" width="650" alt="Standard Basis Vectors">
</p>

---

### 5. Span of Vectors

The span of a set of vectors is the set of all possible linear combinations of those vectors.

If two vectors are linearly independent in 2D space, they can span the entire 2D plane.

For example:

$$
\vec{v_1}=\begin{bmatrix}1\\0\end{bmatrix},
\quad
\vec{v_2}=\begin{bmatrix}0\\1\end{bmatrix}
$$

Their linear combinations are:

$$
a\vec{v_1}+b\vec{v_2}
=
\begin{bmatrix}a\\b\end{bmatrix}
$$

Therefore, they span the entire 2D plane.

**Geometrical Representation of Span in 2D**

<p align="center">
  <img src="./images/05_span_plane.png" width="650" alt="Span of Independent Vectors">
</p>

---

### 6. Linearly Dependent Vectors

Two vectors are linearly dependent if one vector can be expressed as a scalar multiple of the other.

For example:

$$
\vec{v_1}=\begin{bmatrix}1\\2\end{bmatrix},
\quad
\vec{v_2}=\begin{bmatrix}2\\4\end{bmatrix}
$$

Here,

$$
\vec{v_2}=2\vec{v_1}
$$

These vectors are parallel and their span forms a line instead of the entire 2D plane.

**Geometrical Representation of Linearly Dependent Vectors**

<p align="center">
  <img src="./images/06_span_line.png" width="650" alt="Span of Parallel Vectors">
</p>

---

### 7. Basis in Three-Dimensional Space

In three-dimensional space, the standard basis consists of three linearly independent vectors:

$$
\vec{e_1}=\begin{bmatrix}1\\0\\0\end{bmatrix}
$$

$$
\vec{e_2}=\begin{bmatrix}0\\1\\0\end{bmatrix}
$$

$$
\vec{e_3}=\begin{bmatrix}0\\0\\1\end{bmatrix}
$$

These three vectors span the entire 3D space.

Any vector in 3D space can be represented as:

$$
\vec{v}=a\vec{e_1}+b\vec{e_2}+c\vec{e_3}
$$

**Geometrical Representation of 3D Basis Vectors**

<p align="center">
  <img src="./images/07_3d_basis.png" width="650" alt="Three Dimensional Basis">
</p>

---

### Conclusion

Vectors are fundamental elements of linear algebra. Vector addition and scalar multiplication help us perform basic vector operations. Span describes all possible linear combinations of vectors, while basis represents a set of linearly independent vectors that can generate a vector space. These concepts are important foundations for understanding machine learning and other mathematical applications.</WriteingBlock>

