## 1. Vectors

A **vector** is a mathematical quantity that has both magnitude and direction. In linear algebra and machine learning, vectors are used to represent data points, features, and directions in space.

A vector can be represented as:

```text
       ⎡ v₁ ⎤
       ⎢ v₂ ⎥
  v  = ⎢ ⋮  ⎥
       ⎣ vₙ ⎦
```

Example:

```text
     ⎡ 2 ⎤
 v = ⎣ 3 ⎦
```

This is a two-dimensional vector with components 2 and 3.

### 1.1 Vector Representation

A vector can be represented geometrically as an arrow.

- The length of the arrow represents its magnitude.
- The arrowhead represents its direction.
- The starting point is usually the origin.

For a two-dimensional vector:

```text
     ⎡ x ⎤
 v = ⎣ y ⎦
```

Here, x and y represent the horizontal and vertical components.

## 2. Vector Addition

Vector addition means adding the corresponding components of two or more vectors.

Let:

```text
     ⎡ a₁ ⎤          ⎡ b₁ ⎤
 a = ⎣ a₂ ⎦     b =  ⎣ b₂ ⎦
```

Their sum is:

```text
             ⎡ a₁ + b₁ ⎤
 a + b   =   ⎣ a₂ + b₂ ⎦
```

**Example:**

```text
     ⎡ 2 ⎤          ⎡ 4 ⎤
 a = ⎣ 3 ⎦     b =  ⎣ 1 ⎦
```

Therefore:

```text
         ⎡ 2 + 4 ⎤       ⎡ 6 ⎤
 a + b = ⎣ 3 + 1 ⎦   =   ⎣ 4 ⎦
```

### 2.1 Geometric Interpretation

Vector addition can be visualized using the head-to-tail method:

1. Draw the first vector.
2. Place the starting point of the second vector at the endpoint of the first.
3. Draw a new vector from the starting point of the first vector to the endpoint of the second.

The resulting vector represents the sum.

## 3. Scalar Multiplication

Scalar multiplication means multiplying every component of a vector by a scalar (a real number).

Let:

```text
     ⎡ v₁ ⎤
 v = ⎣ v₂ ⎦
```

For a scalar c:

```text
          ⎡ cv₁ ⎤
 c × v =  ⎣ cv₂ ⎦
```

**Example:**

```text
     ⎡ 2 ⎤
 v = ⎣ 3 ⎦       c = 2
```

Then:

```text
       ⎡ 2 ⎤       ⎡ 4 ⎤
 2v = 2⎣ 3 ⎦   =   ⎣ 6 ⎦
```

A positive scalar changes the magnitude while maintaining the direction. A negative scalar reverses the direction.

## 4. Magnitude (Norm) of a Vector

The magnitude or length of a vector is called its **norm**.

For a two-dimensional vector:

```text
     ⎡ x ⎤
 v = ⎣ y ⎦
```

Its Euclidean norm is:

**‖v‖ = √(x² + y²)**

For an n-dimensional vector:

**‖v‖₂ = √(v₁² + v₂² + ... + vₙ²)**

**Example:**

```text
     ⎡ 3 ⎤
 v = ⎣ 4 ⎦
```

**‖v‖ = √(3² + 4²)**

**‖v‖ = √(9 + 16)**

**‖v‖ = √25 = 5**

## 5. Unit Vector

A unit vector is a vector whose magnitude is exactly 1.

A unit vector in the direction of a non-zero vector v is calculated by dividing the vector by its magnitude.

**v̂ = v / ‖v‖**

**Example:**

```text
     ⎡ 3 ⎤
 v = ⎣ 4 ⎦
```

Since:

**‖v‖ = 5**

The unit vector is:

```text
          1   ⎡ 3 ⎤
 v̂ =     ─ × ⎣ 4 ⎦
          5
```

```text
       ⎡ 3/5 ⎤
 v̂ =  ⎣ 4/5 ⎦
```

Its magnitude is 1.

## 6. Linear Combination

A linear combination is formed by multiplying vectors by scalars and then adding the results.

For vectors v₁, v₂, ..., vₙ, a linear combination is:

**v = c₁v₁ + c₂v₂ + ... + cₙvₙ**

Where:

- v₁, v₂, ..., vₙ are vectors.
- c₁, c₂, ..., cₙ are scalar coefficients.
- v is the resulting vector.

**Example:**

Let:

```text
      ⎡ 1 ⎤          ⎡ 0 ⎤
 v₁ = ⎣ 0 ⎦     v₂ = ⎣ 1 ⎦
```

Choose coefficients:

**c₁ = 3, c₂ = 2**

Then:

```text
3v₁ + 2v₂

       ⎡ 1 ⎤       ⎡ 0 ⎤
= 3 ×  ⎣ 0 ⎦ + 2 × ⎣ 1 ⎦

       ⎡ 3 ⎤       ⎡ 0 ⎤
=      ⎣ 0 ⎦  +    ⎣ 2 ⎦

       ⎡ 3 ⎤
=      ⎣ 2 ⎦
```

## 7. Span of Vectors

The **span** of a set of vectors is the set of all possible linear combinations of those vectors.

For two vectors v₁ and v₂:

**Span{v₁, v₂} = {c₁v₁ + c₂v₂ | c₁, c₂ ∈ ℝ}**

The span describes all the vectors that can be generated using the given vectors and scalar coefficients.

### 7.1 Span in Two Dimensions

Consider:

```text
      ⎡ 1 ⎤          ⎡ 0 ⎤
 v₁ = ⎣ 0 ⎦     v₂ = ⎣ 1 ⎦
```

Any vector in two-dimensional space can be expressed as:

```text
      ⎡ x ⎤       ⎡ 1 ⎤       ⎡ 0 ⎤
      ⎣ y ⎦  = x ×⎣ 0 ⎦ + y ×⎣ 1 ⎦
```

Therefore, these two vectors span the entire two-dimensional plane:

**Span{v₁, v₂} = ℝ²**

## 8. Linear Independence

A set of vectors is **linearly independent** if no vector in the set can be expressed as a linear combination of the other vectors.

Mathematically, vectors v₁, v₂, ..., vₙ are linearly independent if:

**c₁v₁ + c₂v₂ + ... + cₙvₙ = 0**

has only the trivial solution:

**c₁ = c₂ = ... = cₙ = 0**

**Example:**

```text
      ⎡ 1 ⎤          ⎡ 0 ⎤
 v₁ = ⎣ 0 ⎦     v₂ = ⎣ 1 ⎦
```

If:

```text
       ⎡ 1 ⎤       ⎡ 0 ⎤       ⎡ 0 ⎤
 c₁ ×  ⎣ 0 ⎦ + c₂ ×⎣ 1 ⎦  =   ⎣ 0 ⎦
```

Then:

```text
     ⎡ c₁ ⎤       ⎡ 0 ⎤
     ⎣ c₂ ⎦   =   ⎣ 0 ⎦
```

Thus:

**c₁ = 0 and c₂ = 0**

The vectors are linearly independent.

## 9. Linear Dependence

A set of vectors is **linearly dependent** if at least one vector can be expressed as a linear combination of the other vectors.

The equation:

**c₁v₁ + c₂v₂ + ... + cₙvₙ = 0**

has at least one non-zero coefficient in a solution.

**Example:**

```text
      ⎡ 1 ⎤          ⎡ 2 ⎤
 v₁ = ⎣ 2 ⎦     v₂ = ⎣ 4 ⎦
```

Notice that:

**v₂ = 2v₁**

Therefore, the second vector is a scalar multiple of the first vector. These vectors are linearly dependent.

## 10. Basis

A **basis** is a set of vectors that satisfies two conditions:

1. The vectors are linearly independent.
2. The vectors span the entire vector space.

For example, the standard basis of ℝ² is:

```text
      ⎡ 1 ⎤          ⎡ 0 ⎤
 e₁ = ⎣ 0 ⎦     e₂ = ⎣ 1 ⎦
```

Every vector in ℝ² can be represented using these two basis vectors:

**[x, y]ᵀ = x e₁ + y e₂**

The standard basis of ℝ³ is:

```text
      ⎡ 1 ⎤
 e₁ = ⎢ 0 ⎥
      ⎣ 0 ⎦

      ⎡ 0 ⎤
 e₂ = ⎢ 1 ⎥
      ⎣ 0 ⎦

      ⎡ 0 ⎤
 e₃ = ⎢ 0 ⎥
      ⎣ 1 ⎦
```

## 11. Dimension of a Vector Space

The dimension of a vector space is the number of vectors in any basis of that space.

Examples:

**dim(ℝ²) = 2**

**dim(ℝ³) = 3**

**dim(ℝⁿ) = n**

A two-dimensional vector space requires two linearly independent basis vectors. A three-dimensional vector space requires three linearly independent basis vectors.

## 12. Linear Transformation

A **linear transformation** is a function that maps vectors from one vector space to another while preserving vector addition and scalar multiplication.

Let T be a transformation. It is linear if it satisfies the following two properties.

### 12.1 Preservation of Vector Addition

**T(u + v) = T(u) + T(v)**

### 12.2 Preservation of Scalar Multiplication

**T(cv) = cT(v)**

Combining these properties:

**T(au + bv) = aT(u) + bT(v)**

Here, a and b are scalars.

### 12.3 Matrix Representation

A linear transformation can be represented using a matrix.

**T(x) = Ax**

Where:

- A is the transformation matrix.
- x is the input vector.
- T(x) is the transformed vector.

**Example:**

Let:

```text
      ⎡ 2  0 ⎤          ⎡ 1 ⎤
 A =  ⎣ 0  3 ⎦     x =  ⎣ 2 ⎦
```

Then:

**T(x) = Ax**

```text
       ⎡ 2  0 ⎤   ⎡ 1 ⎤
     = ⎣ 0  3 ⎦ × ⎣ 2 ⎦

       ⎡ 2(1) + 0(2) ⎤
     = ⎣ 0(1) + 3(2) ⎦

       ⎡ 2 ⎤
     = ⎣ 6 ⎦
```

The transformation scales the first coordinate by 2 and the second coordinate by 3.

### 12.4 Common Linear Transformations

**Scaling:** Changes the size of a vector.

```text
      ⎡ a  0 ⎤
 A =  ⎣ 0  b ⎦
```

**Rotation:** Rotates a vector by an angle θ.

```text
       ⎡ cos θ   -sin θ ⎤
 R(θ)= ⎣ sin θ    cos θ ⎦
```

**Reflection:** Reflects a vector across an axis. Reflection across the x-axis is represented by:

```text
      ⎡ 1   0 ⎤
 A =  ⎣ 0  -1 ⎦
```

**Projection:** Maps a vector onto a specified line or subspace.

For projection onto the x-axis:

```text
      ⎡ 1  0 ⎤
 P =  ⎣ 0  0 ⎦
```

## 13. Vectors and Linear Transformations in Machine Learning

Vectors and linear transformations are important mathematical foundations of machine learning.

- **Data representation:** A data sample can be represented as a vector of numerical features.
- **Feature vectors:** Each feature represents one property of a data sample.
- **Weight vectors:** Machine learning models use weights to determine the importance of features.
- **Linear combinations:** Model predictions can be calculated by combining input features with their corresponding weights.
- **Matrix operations:** Matrices and vectors are used to perform transformations efficiently.
- **Dimensionality:** Vector spaces provide a mathematical foundation for representing and processing data with different numbers of features.
