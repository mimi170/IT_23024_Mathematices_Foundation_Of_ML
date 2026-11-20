# LINEAR COMBINATION, SPAN AND BASIS

## LECTURE 2 – LINEAR ALGEBRA

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

Lecture 3
## 1. Linear Transformation

A **linear transformation** is a function that maps vectors from one vector space to another while preserving vector addition and scalar multiplication.

A transformation T is linear if it satisfies two important properties.

### 1.1 Additivity

The transformation of the sum of two vectors must be equal to the sum of their individual transformations.

**T(u + v) = T(u) + T(v)**

### 1.2 Homogeneity

The transformation of a scalar multiplied by a vector must be equal to the scalar multiplied by the transformed vector.

**T(cv) = cT(v)**

Here:
- T represents a linear transformation.
- u and v represent vectors.
- c represents a scalar.

Both properties can be combined into:

**T(au + bv) = aT(u) + bT(v)**

## 2. Matrix Representation of Linear Transformation

A linear transformation can be represented using matrix multiplication.

The general form is:

**T(x) = Ax**

Where:

- T(x) = transformed vector
- A = transformation matrix
- x = input vector

For a two-dimensional vector:

```text
       ⎡ a  b ⎤   ⎡ x ⎤
T(x) = ⎣ c  d ⎦ × ⎣ y ⎦
```

After matrix multiplication:

```text
       ⎡ ax + by ⎤
T(x) = ⎣ cx + dy ⎦
```

Therefore, a matrix transforms an input vector into a new output vector.

## 3. Matrix Multiplication

Matrix multiplication is the mathematical operation used to apply a linear transformation.

Let:

```text
       ⎡ 2  1 ⎤
 A  =  ⎣ 1  3 ⎦

       ⎡ 4 ⎤
 x  =  ⎣ 2 ⎦
```

Then:

**T(x) = Ax**

```text
       ⎡ 2  1 ⎤   ⎡ 4 ⎤
     = ⎣ 1  3 ⎦ × ⎣ 2 ⎦
```

Multiplying each row by the input vector:

```text
       ⎡ (2 × 4) + (1 × 2) ⎤
     = ⎣ (1 × 4) + (3 × 2) ⎦
```

Therefore:

```text
       ⎡ 10 ⎤
T(x) = ⎣ 10 ⎦
```

The input vector [4, 2]ᵀ is transformed into [10, 10]ᵀ.

## 4. Transformation of Standard Basis Vectors

The standard basis vectors in two-dimensional space are:

```text
       ⎡ 1 ⎤
e₁  =  ⎣ 0 ⎦

       ⎡ 0 ⎤
e₂  =  ⎣ 1 ⎦
```

Every two-dimensional vector can be expressed as a linear combination of these basis vectors.

For a vector:

```text
       ⎡ x ⎤
v   =  ⎣ y ⎦
```

We can write:

**v = xe₁ + ye₂**

Applying a linear transformation:

**T(v) = T(xe₁ + ye₂)**

Using the properties of linear transformation:

**T(v) = xT(e₁) + yT(e₂)**

This means that the transformation of any vector can be determined from the transformations of the standard basis vectors.

## 5. Constructing a Transformation Matrix

A transformation matrix can be constructed by placing the transformed standard basis vectors as its columns.

For a two-dimensional transformation:

```text
          ⎡ |      | ⎤
      A = ⎢ T(e₁) T(e₂) ⎥
          ⎣ |      | ⎦
```

More clearly:

```text
       ⎡ T(e₁)ₓ   T(e₂)ₓ ⎤
A  =   ⎣ T(e₁)ᵧ   T(e₂)ᵧ ⎦
```

Where:

- First column represents T(e₁).
- Second column represents T(e₂).

### Example

Suppose a transformation maps the standard basis vectors as follows:

```text
       ⎡ 2 ⎤
T(e₁)= ⎣ 1 ⎦

       ⎡ 1 ⎤
T(e₂)= ⎣ 3 ⎦
```

The transformation matrix is:

```text
       ⎡ 2  1 ⎤
A  =   ⎣ 1  3 ⎦
```

For any input vector:

```text
       ⎡ x ⎤
v  =   ⎣ y ⎦
```

The output is:

```text
       ⎡ 2  1 ⎤   ⎡ x ⎤
T(v)=  ⎣ 1  3 ⎦ × ⎣ y ⎦
```

Therefore:

```text
       ⎡ 2x + y ⎤
T(v)=  ⎣ x + 3y ⎦
```

## 6. Linear Transformation in Three Dimensions

The same concept applies to three-dimensional vectors.

A three-dimensional input vector is:

```text
       ⎡ x ⎤
v  =   ⎢ y ⎥
       ⎣ z ⎦
```

A general 3 × 3 transformation matrix is:

```text
       ⎡ a  b  c ⎤
A  =   ⎢ d  e  f ⎥
       ⎣ g  h  i ⎦
```

The transformation is:

**T(v) = Av**

After multiplication:

```text
       ⎡ ax + by + cz ⎤
T(v)=  ⎢ dx + ey + fz ⎥
       ⎣ gx + hy + iz ⎦
```

The output is another three-dimensional vector.

## 7. Common Types of Linear Transformations

### 7.1 Scaling Transformation

Scaling changes the size of a vector.

A two-dimensional scaling matrix is:

```text
       ⎡ sₓ  0  ⎤
A  =   ⎣ 0   sᵧ ⎦
```

Where:
- sₓ = scaling factor along the x-axis.
- sᵧ = scaling factor along the y-axis.

The transformation is:

```text
       ⎡ sₓx ⎤
T(v)=  ⎣ sᵧy ⎦
```

### 7.2 Rotation Transformation

A rotation transformation rotates a vector by an angle θ.

The rotation matrix is:

```text
       ⎡ cos θ  -sin θ ⎤
R  =   ⎣ sin θ   cos θ ⎦
```

The transformed vector is:

**T(v) = Rv**

### 7.3 Reflection Transformation

Reflection changes the direction of a vector across a specified axis.

Reflection across the x-axis:

```text
       ⎡ 1   0 ⎤
A  =   ⎣ 0  -1 ⎦
```

Reflection across the y-axis:

```text
       ⎡ -1  0 ⎤
A  =   ⎣  0  1 ⎦
```

### 7.4 Projection Transformation

Projection maps a vector onto a line or subspace.

Projection onto the x-axis:

```text
       ⎡ 1  0 ⎤
P  =   ⎣ 0  0 ⎦
```

For an input vector:

```text
       ⎡ x ⎤
v  =   ⎣ y ⎦
```

The output is:

```text
       ⎡ x ⎤
P(v)=  ⎣ 0 ⎦
```

The y-coordinate becomes zero, while the x-coordinate remains unchanged.

## 8. Composition of Linear Transformations

Composition means applying one transformation after another.

Suppose there are two transformations:

**T₁(x) = A₁x**

**T₂(x) = A₂x**

Applying T₁ first and then T₂:

**T₂(T₁(x)) = A₂(A₁x)**

Using matrix multiplication:

**T₂(T₁(x)) = (A₂A₁)x**

Therefore, the combined transformation matrix is:

**A = A₂A₁**

The order of matrix multiplication is important. In general:

**A₂A₁ ≠ A₁A₂**

## 9. Identity Transformation

An identity transformation leaves every vector unchanged.

**T(v) = v**

Its matrix is called the identity matrix.

For two-dimensional space:

```text
       ⎡ 1  0 ⎤
I  =   ⎣ 0  1 ⎦
```

For three-dimensional space:

```text
       ⎡ 1  0  0 ⎤
I  =   ⎢ 0  1  0 ⎥
       ⎣ 0  0  1 ⎦
```

For any compatible vector:

**Iv = v**

## 10. Zero Transformation

A zero transformation maps every input vector to the zero vector.

**T(v) = 0**

Its matrix contains only zero elements.

For two-dimensional space:

```text
       ⎡ 0  0 ⎤
A  =   ⎣ 0  0 ⎦
```

For any input vector:

```text
       ⎡ x ⎤
v  =   ⎣ y ⎦
```

The output is:

```text
       ⎡ 0 ⎤
T(v)=  ⎣ 0 ⎦
```

## 11. Important Properties of Linear Transformations

A linear transformation satisfies the following properties:

1. **Preservation of Addition**

   T(u + v) = T(u) + T(v)

2. **Preservation of Scalar Multiplication**

   T(cv) = cT(v)

3. **Zero Vector Preservation**

   T(0) = 0

4. **Linear Combination Preservation**

   T(au + bv) = aT(u) + bT(v)

5. **Matrix Representation**

   Every linear transformation between finite-dimensional vector spaces can be represented by a matrix after choosing bases.



A common linear operation in a neural network is:

**z = Wx + b**

Where:

- x = input vector
- W = weight matrix
- b = bias vector
- z = output before activation

The activation function is then applied:

**a = f(z)**

Lecture 4
## 1. Three-Dimensional (3D) Vector

A three-dimensional vector represents a point or direction in 3D space using three coordinates: x, y, and z.

A 3D vector is represented as:

```text
       ⎡ x ⎤
v  =   ⎢ y ⎥
       ⎣ z ⎦
```

Where:
- x represents the position along the x-axis.
- y represents the position along the y-axis.
- z represents the position along the z-axis.

A 3D vector can also be written as:

**v = (x, y, z)**

## 2. Standard Basis Vectors in 3D

The standard basis vectors in three-dimensional space are:

```text
       ⎡ 1 ⎤
e₁ =   ⎢ 0 ⎥
       ⎣ 0 ⎦

       ⎡ 0 ⎤
e₂ =   ⎢ 1 ⎥
       ⎣ 0 ⎦

       ⎡ 0 ⎤
e₃ =   ⎢ 0 ⎥
       ⎣ 1 ⎦
```

These vectors represent the positive directions of the x, y, and z axes respectively.

Any 3D vector can be expressed as a linear combination of these three basis vectors.

**v = xe₁ + ye₂ + ze₃**

Therefore:

```text
       ⎡ x ⎤
v  =   ⎢ y ⎥
       ⎣ z ⎦
```

## 3. Linear Transformation in 3D

A 3D linear transformation maps an input vector in three-dimensional space to another vector in three-dimensional space.

The general form is:

**T(v) = Av**

Where:

- A is a 3 × 3 transformation matrix.
- v is the input vector.
- T(v) is the transformed vector.

A general 3 × 3 matrix is:

```text
       ⎡ a  b  c ⎤
A  =   ⎢ d  e  f ⎥
       ⎣ g  h  i ⎦
```

The input vector is:

```text
       ⎡ x ⎤
v  =   ⎢ y ⎥
       ⎣ z ⎦
```

After matrix multiplication:

```text
       ⎡ ax + by + cz ⎤
T(v)=  ⎢ dx + ey + fz ⎥
       ⎣ gx + hy + iz ⎦
```

## 4. Transformation of Standard Basis Vectors

The transformation of the standard basis vectors determines the entire linear transformation.

The three standard basis vectors are:

**e₁ = (1, 0, 0)**

**e₂ = (0, 1, 0)**

**e₃ = (0, 0, 1)**

For any vector:

**v = xe₁ + ye₂ + ze₃**

Applying the transformation:

**T(v) = T(xe₁ + ye₂ + ze₃)**

Using linearity:

**T(v) = xT(e₁) + yT(e₂) + zT(e₃)**

This means that if we know the transformed positions of the three standard basis vectors, we can determine the transformation of every vector in 3D space.

## 5. Constructing a 3D Transformation Matrix

A 3D transformation matrix is constructed by placing the transformed standard basis vectors into its columns.

**A = [T(e₁)  T(e₂)  T(e₃)]**

In matrix form:

```text
       ⎡ T(e₁)ₓ  T(e₂)ₓ  T(e₃)ₓ ⎤
A  =   ⎢ T(e₁)ᵧ  T(e₂)ᵧ  T(e₃)ᵧ ⎥
       ⎣ T(e₁)ᵤ  T(e₂)ᵤ  T(e₃)ᵤ ⎦
```

Here, each column represents the transformed version of one standard basis vector.

### Example

Suppose the transformation maps the standard basis vectors as follows:

```text
       ⎡ 2 ⎤
T(e₁)= ⎢ 0 ⎥
       ⎣ 1 ⎦

       ⎡ 1 ⎤
T(e₂)= ⎢ 3 ⎥
       ⎣ 0 ⎦

       ⎡ 0 ⎤
T(e₃)= ⎢ 1 ⎥
       ⎣ 2 ⎦
```

The transformation matrix is:

```text
       ⎡ 2  1  0 ⎤
A  =   ⎢ 0  3  1 ⎥
       ⎣ 1  0  2 ⎦
```

For an input vector:

```text
       ⎡ 1 ⎤
v  =   ⎢ 2 ⎥
       ⎣ 3 ⎦
```

The output is:

**T(v) = Av**

```text
       ⎡ 2  1  0 ⎤   ⎡ 1 ⎤
     = ⎢ 0  3  1 ⎥ × ⎢ 2 ⎥
       ⎣ 1  0  2 ⎦   ⎣ 3 ⎦
```

Calculating each component:

```text
       ⎡ (2×1) + (1×2) + (0×3) ⎤
     = ⎢ (0×1) + (3×2) + (1×3) ⎥
       ⎣ (1×1) + (0×2) + (2×3) ⎦
```

Therefore:

```text
       ⎡ 4 ⎤
T(v)=  ⎢ 9 ⎥
       ⎣ 7 ⎦
```

## 6. Common 3D Linear Transformations

### 6.1 Scaling Transformation

Scaling changes the size of a vector along the x, y, and z axes.

The 3D scaling matrix is:

```text
       ⎡ sₓ  0   0  ⎤
A  =   ⎢ 0   sᵧ  0  ⎥
       ⎣ 0   0   s𝓏 ⎦
```

Where:
- sₓ = scaling factor along the x-axis.
- sᵧ = scaling factor along the y-axis.
- s𝓏 = scaling factor along the z-axis.

The transformed vector is:

```text
       ⎡ sₓx ⎤
T(v)=  ⎢ sᵧy ⎥
       ⎣ s𝓏z ⎦
```

### 6.2 Rotation Around the X-Axis

A rotation around the x-axis changes the y and z coordinates while keeping the x-coordinate unchanged.

The rotation matrix is:

```text
       ⎡ 1    0        0      ⎤
Rₓ =   ⎢ 0   cos θ   -sin θ  ⎥
       ⎣ 0   sin θ    cos θ  ⎦
```

### 6.3 Rotation Around the Y-Axis

A rotation around the y-axis changes the x and z coordinates while keeping the y-coordinate unchanged.

The rotation matrix is:

```text
       ⎡ cos θ   0   sin θ ⎤
Rᵧ =   ⎢   0     1     0   ⎥
       ⎣-sin θ   0   cos θ ⎦
```

### 6.4 Rotation Around the Z-Axis

A rotation around the z-axis changes the x and y coordinates while keeping the z-coordinate unchanged.

The rotation matrix is:

```text
       ⎡ cos θ  -sin θ   0 ⎤
R𝓏 =   ⎢ sin θ   cos θ   0 ⎥
       ⎣   0       0     1 ⎦
```

### 6.5 Reflection Transformation

Reflection changes the direction of a vector across a specified plane.

Reflection across the XY-plane:

```text
       ⎡ 1   0   0  ⎤
A  =   ⎢ 0   1   0  ⎥
       ⎣ 0   0  -1  ⎦
```

Reflection across the YZ-plane:

```text
       ⎡ -1  0   0 ⎤
A  =   ⎢  0  1   0 ⎥
       ⎣  0  0   1 ⎦
```

Reflection across the XZ-plane:

```text
       ⎡ 1   0   0 ⎤
A  =   ⎢ 0  -1   0 ⎥
       ⎣ 0   0   1 ⎦
```

## 7. Composition of 3D Transformations

Composition means applying multiple transformations one after another.

Suppose two transformations are represented by:

**T₁(v) = A₁v**

**T₂(v) = A₂v**

Applying T₁ first and then T₂:

**T₂(T₁(v)) = A₂(A₁v)**

Using matrix multiplication:

**T₂(T₁(v)) = (A₂A₁)v**

Therefore, the combined transformation matrix is:

**A = A₂A₁**

The order of matrix multiplication is important.

In general:

**A₂A₁ ≠ A₁A₂**

## 8. Identity Transformation in 3D

An identity transformation leaves every vector unchanged.

**T(v) = v**

The 3D identity matrix is:

```text
       ⎡ 1  0  0 ⎤
I  =   ⎢ 0  1  0 ⎥
       ⎣ 0  0  1 ⎦
```

For any compatible vector:

**Iv = v**

## 9. Zero Transformation in 3D

A zero transformation maps every input vector to the zero vector.

**T(v) = 0**

The 3D zero matrix is:

```text
       ⎡ 0  0  0 ⎤
A  =   ⎢ 0  0  0 ⎥
       ⎣ 0  0  0 ⎦
```

For any input vector:

```text
       ⎡ x ⎤
v  =   ⎢ y ⎥
       ⎣ z ⎦
```

The output is:

```text
       ⎡ 0 ⎤
T(v)=  ⎢ 0 ⎥
       ⎣ 0 ⎦
```

## 10. Invertible Linear Transformation

A linear transformation is invertible if an inverse transformation exists that can recover the original input vector.

If:

**T(v) = Av**

Then the inverse transformation is:

**v = A⁻¹T(v)**

The inverse matrix satisfies:

**A⁻¹A = AA⁻¹ = I**

A square matrix is invertible if its determinant is non-zero.

**det(A) ≠ 0**

If the determinant is zero, the matrix is singular and does not have an inverse.

## 11. Determinant of a 3 × 3 Matrix

For a 3 × 3 matrix:

```text
       ⎡ a  b  c ⎤
A  =   ⎢ d  e  f ⎥
       ⎣ g  h  i ⎦
```

Its determinant is:

**det(A) = a(ei − fh) − b(di − fg) + c(dh − eg)**

The determinant provides information about how a linear transformation changes the volume of a three-dimensional region.

- If det(A) is positive, orientation is preserved.
- If det(A) is negative, orientation is reversed.
- If det(A) is zero, the transformation collapses the 3D space into a lower-dimensional space.

The absolute value of the determinant represents the volume scaling factor.

**Volume scaling factor = |det(A)|**

## 12. Volume and Linear Transformation

A 3D linear transformation can change the volume of a geometric object.

If the original volume is V, then the transformed volume is:

**V′ = |det(A)| × V**

Example:

If:

**det(A) = 3**

And the original volume is:

**V = 5**

Then:

**V′ = 3 × 5 = 15**

The transformed volume is 15 cubic units.

## 13. Linear Transformations in Machine Learning

Three-dimensional linear transformations are useful for understanding how data is transformed in higher-dimensional spaces.

- **Data representation:** Data points can be represented as vectors with multiple numerical features.
- **Feature transformation:** Matrix multiplication transforms input features into new representations.
- **Neural networks:** Weight matrices transform input vectors into new feature representations.
- **Computer vision:** 3D transformations are used in object positioning, rotation, and geometric operations.
- **Dimensionality reduction:** Linear transformations can map high-dimensional data into lower-dimensional representations.
- **Scientific computing:** Matrix transformations are used in simulations and numerical calculations.

A common linear operation in a machine learning model is:

**z = Wx + b**

Where:
- x = input vector.
- W = weight matrix.
- b = bias vector.
- z = transformed output before activation.

The activation function is then applied:

**a = f(z)**

# Product of Two Matrices = Composite Transformation
## Lecture 5 – Linear Algebra

### 1. Composite Transformation

A composite transformation is obtained by applying two or more linear transformations one after another.

Suppose:
- T₁ is the first transformation.
- T₂ is the second transformation.

If T₁ is applied first and T₂ is applied afterward, the composite transformation is:

T(x) = T₂(T₁(x))

If the matrix of T₁ is A and the matrix of T₂ is B, then:

**Composite Transformation Matrix = BA**

Therefore,

T(x) = B(Ax) = (BA)x

**Important:** The transformation applied first appears on the right side of the matrix product.

### 2. Matrix Multiplication as Composite Transformation

Suppose two linear transformations are represented by:

```text
A = | a  b |
    | c  d |

B = | e  f |
    | g  h |
```

The composite transformation is represented by:

```text
BA = | e  f | | a  b |
     | g  h | | c  d |
```

Multiplying the matrices:

```text
BA = | ea + fc   eb + fd |
     | ga + hc   gb + hd |
```

The resulting matrix represents both transformations performed sequentially.

### 3. Example: Scaling Followed by Rotation

Suppose the first transformation is scaling:

- x-coordinate is multiplied by 2.
- y-coordinate remains unchanged.

Its matrix is:

```text
A = | 2  0 |
    | 0  1 |
```

The second transformation is a 90° counterclockwise rotation.

Its matrix is:

```text
B = | 0  -1 |
    | 1   0 |
```

Since scaling is performed first and rotation afterward:

```text
Composite Matrix = BA
```

Now multiply:

```text
BA = | 0  -1 | | 2  0 |
     | 1   0 | | 0  1 |

   = | 0  -1 |
     | 2   0 |
```

Therefore, the composite transformation matrix is:

```text
C = | 0  -1 |
    | 2   0 |
```

For an input vector:

```text
x = | x |
    | y |
```

The output becomes:

```text
C x = | 0  -1 | | x |
      | 2   0 | | y |

    = | -y |
      | 2x |
```

Thus, the combined transformation is:

(x, y) → (−y, 2x)

### 4. Order of Matrix Multiplication

Matrix multiplication is generally not commutative.

This means:

AB ≠ BA

The order of transformations changes the final result.

For example, consider:

```text
A = | 2  0 |
    | 0  1 |

B = | 0  -1 |
    | 1   0 |
```

First calculate BA:

```text
BA = | 0  -1 |
     | 2   0 |
```

Now calculate AB:

```text
AB = | 2  0 | | 0  -1 |
     | 0  1 | | 1   0 |

   = | 0  -2 |
     | 1   0 |
```

Therefore:

```text
AB = | 0  -2 |
     | 1   0 |

BA = | 0  -1 |
     | 2   0 |
```

So,

AB ≠ BA

**Conclusion:** Changing the order of transformations can produce a different final transformation.

### 5. Associative Property of Matrix Multiplication

Matrix multiplication is associative.

For three matrices A, B, and C:

(AB)C = A(BC)

This means the grouping of matrix multiplication does not change the final result.

However, the order of the matrices must remain unchanged.

### 6. Identity Matrix in Composite Transformation

The identity matrix represents a transformation that does not change the input vector.

For a 2D transformation:

```text
I = | 1  0 |
    | 0  1 |
```

For any compatible matrix A:

AI = IA = A

Applying an identity transformation before or after another transformation does not change the result.

### 7. Inverse Transformation

An inverse transformation reverses the effect of a given transformation.

If A represents a transformation, its inverse matrix is denoted by A⁻¹.

The relationship is:

```text
AA⁻¹ = A⁻¹A = I
```

If a transformation is represented by A, applying A followed by A⁻¹ returns the original vector:

```text
A⁻¹(Ax) = Ix = x
```

A matrix has an inverse only when it is invertible.

For a square matrix, the condition is:

det(A) ≠ 0

### 8. Composite Transformation of Multiple Matrices

Suppose three transformations are applied in the following order:

1. First transformation: A
2. Second transformation: B
3. Third transformation: C

The final transformation is:

```text
T(x) = C(B(Ax))
```

Using matrix multiplication:

```text
T(x) = CBAx
```

Therefore, the composite transformation matrix is:

```text
Composite Matrix = CBA
```

The rightmost matrix is applied first, and the leftmost matrix is applied last.

### 9. Important Properties

| Property | Mathematical Expression |
|---|---|
| Associative | (AB)C = A(BC) |
| Identity | AI = IA = A |
| Non-commutative | AB ≠ BA (generally) |
| Inverse | AA⁻¹ = A⁻¹A = I |
| Composition | T₂(T₁(x)) = BAx |
| Multiple transformations | T₃(T₂(T₁(x))) = CBAx |

# A Simple Physical Intuition for Determinants
## Lecture 6 – Linear Algebra

### 1. Determinant

The determinant is a scalar value calculated from a square matrix.

It provides information about how a linear transformation changes the area or volume of a geometric object.

For a 2 × 2 matrix:

```text
A = | a  b |
    | c  d |
```

The determinant is:

det(A) = ad − bc

It is also written as:

det(A) = |A|

### 2. Geometric Meaning of Determinant

A determinant represents the factor by which a linear transformation scales area in 2D or volume in 3D.

- If |det(A)| > 1, area or volume increases.
- If 0 < |det(A)| < 1, area or volume decreases.
- If det(A) = 0, area or volume becomes zero.
- If |det(A)| = 1, area or volume remains unchanged.

The absolute value of the determinant represents the scaling factor.

### 3. Area of a Parallelogram

Suppose two vectors are:

```text
u = | a |       v = | b |
    | c |           | d |
```

These two vectors form a parallelogram.

The area of the parallelogram is:

Area = |ad − bc|

Therefore:

Area = |det(A)|

where A is the matrix formed using the two vectors as columns.

### 4. Example: Calculating Area

Consider the matrix:

```text
A = | 3  1 |
    | 1  2 |
```

The determinant is:

det(A) = (3 × 2) − (1 × 1)

det(A) = 6 − 1

det(A) = 5

Therefore, the area of the parallelogram formed by the column vectors is:

Area = |5| = 5 square units.

### 5. Determinant and Area Scaling

Suppose a unit square has an area of 1 square unit.

A linear transformation represented by matrix A changes the area of the square by a factor of |det(A)|.

For example, if:

det(A) = 3

Then:

New Area = 3 × Original Area

If the original area is 1:

New Area = 3 square units.

Similarly, if:

det(A) = 0.5

Then:

New Area = 0.5 × Original Area

### 6. Positive and Negative Determinants

The sign of the determinant indicates whether the transformation preserves or reverses orientation.

**Positive determinant:**

- Orientation is preserved.
- The direction or ordering of the basis vectors remains consistent.

**Negative determinant:**

- Orientation is reversed.
- The transformation includes an orientation-reversing effect, such as reflection.

**Zero determinant:**

- The transformed vectors become linearly dependent.
- The area collapses to zero.
- The transformation is not invertible.

### 7. Determinant of a 3 × 3 Matrix

For a 3 × 3 matrix:

```text
A = | a  b  c |
    | d  e  f |
    | g  h  i |
```

The determinant is:

det(A) = a(ei − fh) − b(di − fg) + c(dh − eg)

In 3D, the absolute value of the determinant represents the volume scaling factor.

### 8. Volume of a Parallelepiped

Three vectors in 3D space form a parallelepiped.

If these vectors are the columns of matrix A, then:

Volume = |det(A)|

For example, if:

det(A) = −6

Then:

Volume = |−6| = 6 cubic units.

The negative sign indicates reversed orientation, not negative physical volume.

### 9. Determinant and Linear Independence

The determinant helps determine whether the column vectors of a square matrix are linearly independent.

If:

det(A) ≠ 0

Then:
- The columns are linearly independent.
- The matrix is invertible.
- The transformation preserves dimensionality.

If:

det(A) = 0

Then:
- The columns are linearly dependent.
- The matrix is not invertible.
- The transformation collapses the space into a lower-dimensional space.

### 10. Determinant of Special Matrices

**Identity Matrix**

```text
I = | 1  0 |
    | 0  1 |
```

det(I) = 1

**Scaling Matrix**

```text
A = | sₓ  0  |
    | 0   sᵧ |
```

det(A) = sₓ × sᵧ

**Rotation Matrix**

```text
R = | cosθ  −sinθ |
    | sinθ   cosθ |
```

det(R) = cos²θ + sin²θ = 1

A rotation preserves area and orientation.

**Reflection Matrix**

```text
A = | −1  0 |
    |  0  1 |
```

det(A) = −1

A reflection preserves area but reverses orientation.

### 11. Determinant of a Product of Matrices

For two square matrices A and B:

det(AB) = det(A) × det(B)

This means the total area or volume scaling factor of a composite transformation is the product of the individual scaling factors.

For three matrices:

det(ABC) = det(A) × det(B) × det(C)

### 12. Important Properties

| Property | Formula |
|---|---|
| 2 × 2 determinant | ad − bc |
| Area scaling | New Area = |det(A)| × Original Area |
| Volume scaling | New Volume = |det(A)| × Original Volume |
| Identity matrix | det(I) = 1 |
| Singular matrix | det(A) = 0 |
| Invertible matrix | det(A) ≠ 0 |
| Product of matrices | det(AB) = det(A)det(B) |
| Inverse matrix | det(A⁻¹) = 1/det(A) |
| Transpose | det(Aᵀ) = det(A) |
| Rotation matrix | det(R) = 1 |
| Reflection matrix | det(A) = −1 |

# Transformation with Non-Square Matrices: 2D to 3D
## Lecture 7 – Linear Algebra

### 1. Non-Square Matrix

A non-square matrix is a matrix in which the number of rows and columns is different.

Examples:

**2 × 3 Matrix**

```text
A = | 1  2  3 |
    | 4  5  6 |
```

**3 × 2 Matrix**

```text
B = | 1  2 |
    | 3  4 |
    | 5  6 |
```

A matrix with m rows and n columns represents a linear transformation from an n-dimensional input space to an m-dimensional output space.

### 2. Transformation from 2D to 3D

A 2D vector contains two coordinates:

```text
x = | x₁ |
    | x₂ |
```

A 3D vector contains three coordinates:

```text
y = | y₁ |
    | y₂ |
    | y₃ |
```

To transform a 2D vector into a 3D vector, we need a 3 × 2 matrix.

The transformation is:

y = Ax

Where:

- A is a 3 × 2 transformation matrix.
- x is a 2D input vector.
- y is a 3D output vector.

### 3. General Form of a 2D to 3D Transformation

Let the transformation matrix be:

```text
A = | a  b |
    | c  d |
    | e  f |
```

The input vector is:

```text
x = | x₁ |
    | x₂ |
```

Multiplying A by x:

```text
y = Ax

  = | a  b | | x₁ |
    | c  d | | x₂ |
    | e  f |

  = | ax₁ + bx₂ |
    | cx₁ + dx₂ |
    | ex₁ + fx₂ |
```

Therefore, the output is a 3D vector.

### 4. Example of 2D to 3D Transformation

Consider the transformation matrix:

```text
A = | 1  0 |
    | 0  1 |
    | 1  1 |
```

Input vector:

```text
x = | 2 |
    | 3 |
```

Now calculate:

```text
y = Ax

  = | 1  0 | | 2 |
    | 0  1 | | 3 |
    | 1  1 |

  = | 2 |
    | 3 |
    | 5 |
```

Therefore:

```text
Input  = (2, 3)
Output = (2, 3, 5)
```

The 2D input vector is transformed into a 3D output vector.

### 5. Standard Basis Vectors

In 2D, the standard basis vectors are:

```text
e₁ = | 1 |       e₂ = | 0 |
     | 0 |            | 1 |
```

Any 2D vector can be expressed as a linear combination of these basis vectors:

```text
x = x₁e₁ + x₂e₂
```

For a linear transformation T:

```text
T(x) = x₁T(e₁) + x₂T(e₂)
```

This means the transformation of the standard basis vectors determines the transformation of every vector.

### 6. Constructing a Transformation Matrix Using Basis Vectors

Suppose a transformation maps 2D vectors into 3D vectors.

Let:

```text
T(e₁) = | a |
        | b |
        | c |

T(e₂) = | d |
        | e |
        | f |
```

The transformation matrix is constructed by placing the transformed basis vectors as columns:

```text
A = | a  d |
    | b  e |
    | c  f |
```

Therefore:

```text
T(x) = Ax
```

**Important:** The columns of a transformation matrix represent the images of the standard basis vectors.

### 7. Geometric Meaning of 2D to 3D Transformation

A 2D vector belongs to a two-dimensional input space.

A 3 × 2 matrix maps this vector into a three-dimensional output space.

However, the output does not necessarily fill the entire 3D space.

The output vectors lie in the span of the two columns of the transformation matrix.

Therefore, the image of the transformation can be:

- A plane through the origin, if the two columns are linearly independent.
- A line through the origin, if the two columns are linearly dependent.
- A single point at the origin, if both columns are zero.

### 8. Rank of a Non-Square Matrix

The rank of a matrix is the maximum number of linearly independent columns or rows.

For a 3 × 2 matrix:

```text
Maximum possible rank = 2
```

Possible ranks are:

- Rank 2: The two columns are linearly independent. The image is a plane in 3D.
- Rank 1: The columns are linearly dependent, but at least one is nonzero. The image is a line.
- Rank 0: All entries are zero. The image contains only the origin.

The rank determines the dimension of the image of the transformation.

### 9. Matrix Dimensions and Multiplication

For matrix multiplication, the number of columns in the first matrix must equal the number of rows in the second matrix.

If:

```text
A = 3 × 2
x = 2 × 1
```

Then:

```text
Ax = (3 × 2)(2 × 1)

   = 3 × 1
```

The resulting vector has three rows and one column.

General rule:

```text
(m × n)(n × p) = (m × p)
```

### 10. Composition of Non-Square Transformations

Suppose:

- A transforms a 2D vector into a 3D vector.
- B transforms a 3D vector into another 3D vector.

Their dimensions are:

```text
A = 3 × 2
B = 3 × 3
```

The composite transformation is:

```text
BA
```

The dimensions are:

```text
(3 × 3)(3 × 2) = 3 × 2
```

Therefore, the combined transformation still maps 2D input vectors into 3D output vectors.

The rightmost matrix is applied first.

# Matrix Inverse – Physical Meaning in Transformations
## Lecture 8 – Linear Algebra

### 1. Inverse of a Matrix

The inverse of a matrix is a matrix that reverses the effect of the original matrix transformation.

If A is a square matrix, its inverse is denoted by A⁻¹.

The fundamental property is:

```text
AA⁻¹ = A⁻¹A = I
```

Where:
- A = Original matrix
- A⁻¹ = Inverse matrix
- I = Identity matrix

If a vector x is transformed by A:

```text
y = Ax
```

To recover the original vector:

```text
x = A⁻¹y
```

### 2. Physical Meaning of Matrix Inverse

A matrix transformation changes the position or direction of vectors.

The inverse transformation reverses that change and brings the transformed vector back to its original position.

For example:

```text
Original Vector → Transformation A → New Vector
New Vector      → Transformation A⁻¹ → Original Vector
```

Mathematically:

```text
A⁻¹(Ax) = x
```

The inverse transformation undoes the original transformation.

### 3. Inverse of a 2 × 2 Matrix

For a 2 × 2 matrix:

```text
A = | a  b |
    | c  d |
```

Its determinant is:

```text
det(A) = ad − bc
```

The inverse is:

```text
       1       |  d  −b |
A⁻¹ = ───────  |        |
      ad − bc  | −c   a |
```

This formula is valid only when:

```text
ad − bc ≠ 0
```

### 4. Example of Matrix Inverse

Consider:

```text
A = | 2  1 |
    | 1  1 |
```

Step 1: Calculate the determinant.

```text
det(A) = (2 × 1) − (1 × 1)

       = 2 − 1

       = 1
```

Step 2: Interchange the diagonal elements.

Step 3: Change the signs of the off-diagonal elements.

```text
|  1  −1 |
| −1   2 |
```

Step 4: Divide by the determinant.

```text
       1     |  1  −1 |
A⁻¹ = ───    |        |
       1     | −1   2 |
```

Therefore:

```text
A⁻¹ = |  1  −1 |
      | −1   2 |
```

### 5. Verifying the Inverse

To verify the inverse, multiply A by A⁻¹.

```text
AA⁻¹ = | 2  1 | |  1  −1 |
       | 1  1 | | −1   2 |
```

Multiplying:

```text
     = | (2×1)+(1×−1)   (2×−1)+(1×2) |
       | (1×1)+(1×−1)   (1×−1)+(1×2) |

     = | 1  0 |
       | 0  1 |
```

Therefore:

```text
AA⁻¹ = I
```

The inverse is correct.

### 6. Inverse Transformation: Scaling

Consider a scaling matrix:

```text
A = | 2  0 |
    | 0  3 |
```

This transformation:
- Doubles the x-coordinate.
- Triples the y-coordinate.

Its inverse is:

```text
A⁻¹ = | 1/2   0   |
      |  0   1/3  |
```

If the original vector is:

```text
x = | 2 |
    | 3 |
```

After applying A:

```text
y = Ax

  = | 2  0 | | 2 |
    | 0  3 | | 3 |

  = | 4 |
    | 9 |
```

Now apply the inverse:

```text
A⁻¹y = | 1/2   0  | | 4 |
       |  0   1/3 | | 9 |

     = | 2 |
       | 3 |
```

The original vector is recovered.

### 7. Inverse of a Rotation Matrix

A 2D rotation matrix is:

```text
R(θ) = | cosθ  −sinθ |
       | sinθ   cosθ |
```

The inverse rotation matrix is:

```text
R⁻¹(θ) = | cosθ   sinθ |
         | −sinθ  cosθ |
```

Therefore:

```text
R⁻¹(θ) = R(−θ)
```

This means that the inverse of a rotation by θ is a rotation by −θ.

For example:
- Rotate 90° counterclockwise.
- Apply the inverse rotation of 90° clockwise.
- The original vector is recovered.

### 8. Inverse of Composite Transformations

Suppose two transformations are represented by matrices A and B.

Their composite transformation is:

```text
C = BA
```

The inverse of the composite matrix is:

```text
C⁻¹ = (BA)⁻¹
```

The inverse reverses both transformations in reverse order:

```text
(BA)⁻¹ = A⁻¹B⁻¹
```

**Important:** The order of matrices is reversed when taking the inverse of a product.

For three matrices:

```text
(ABC)⁻¹ = C⁻¹B⁻¹A⁻¹
```

### 9. Determinant and Invertibility

The determinant determines whether a square matrix has an inverse.

For a square matrix A:

**Case 1: Nonzero determinant**

```text
det(A) ≠ 0
```

- The matrix is invertible.
- The inverse exists.
- The transformation is reversible.
- The transformation does not collapse the space into a lower dimension.

**Case 2: Zero determinant**

```text
det(A) = 0
```

- The matrix is singular.
- The inverse does not exist.
- The transformation is not reversible.
- The transformation collapses the space into a lower dimension.

### 10. Geometric Meaning of a Non-Invertible Transformation

Consider the matrix:

```text
A = | 1  0 |
    | 0  0 |
```

For an input vector:

```text
x = | x₁ |
    | x₂ |
```

The output is:

```text
Ax = | x₁ |
     |  0 |
```

The y-coordinate is always mapped to zero.

Different input vectors can produce the same output vector.

For example:

```text
A | 2 | = | 2 |
  | 3 |   | 0 |

A | 2 | = | 2 |
  | 5 |   | 0 |
```

Both inputs produce the same output.

Therefore, the original input cannot be uniquely recovered.

The determinant is:

```text
det(A) = (1 × 0) − (0 × 0)

       = 0
```

Thus, A has no inverse.

### 11. Important Properties of Matrix Inverse

| Property | Formula |
|---|---|
| Identity | AA⁻¹ = I |
| Inverse of inverse | (A⁻¹)⁻¹ = A |
| Product inverse | (AB)⁻¹ = B⁻¹A⁻¹ |
| Transpose of inverse | (Aᵀ)⁻¹ = (A⁻¹)ᵀ |
| Determinant of inverse | det(A⁻¹) = 1/det(A) |
| Identity inverse | I⁻¹ = I |
| Inverse of rotation | R⁻¹(θ) = R(−θ) |

# Relation Between Dot Product and Transformation
## Lecture 9 – Linear Algebra

### 1. Dot Product

The dot product is an operation between two vectors that produces a scalar value.

For two vectors:

```text
u = | u₁ |       v = | v₁ |
    | u₂ |           | v₂ |
```

The dot product is:

u · v = u₁v₁ + u₂v₂

For 3D vectors:

u · v = u₁v₁ + u₂v₂ + u₃v₃

### 2. Geometric Meaning of Dot Product

The dot product measures how much two vectors point in the same direction.

The geometric formula is:

u · v = ||u|| ||v|| cos θ

Where:

- ||u|| = Magnitude of vector u
- ||v|| = Magnitude of vector v
- θ = Angle between the two vectors

From this formula:

- If θ = 0°, the dot product is positive and maximum.
- If θ = 90°, the dot product is zero.
- If θ = 180°, the dot product is negative.

### 3. Dot Product and Orthogonality

Two vectors are orthogonal when they are perpendicular to each other.

For orthogonal vectors:

u · v = 0

Example:

```text
u = | 1 |
    | 0 |

v = | 0 |
    | 1 |
```

Their dot product is:

u · v = (1 × 0) + (0 × 1)

u · v = 0

Therefore, the vectors are orthogonal.

### 4. Dot Product as a Projection

The dot product is closely related to the projection of one vector onto another.

The scalar projection of u onto v is:

Scalar Projection = (u · v) / ||v||

The vector projection of u onto v is:

```text
             u · v
projᵥ(u) = ───────── v
              ||v||²
```

The projection represents the component of one vector along the direction of another vector.

### 5. Dot Product as Matrix Multiplication

Two vectors can be represented as a row vector and a column vector.

```text
uᵀ = | u₁  u₂ |

v  = | v₁ |
     | v₂ |
```

Their dot product is:

```text
uᵀv = | u₁  u₂ | | v₁ |
                     | v₂ |

    = u₁v₁ + u₂v₂
```

Therefore:

u · v = uᵀv

This shows that the dot product can be expressed using matrix multiplication.

### 6. Transformation of a Vector

A linear transformation changes a vector using a matrix.

If A is a transformation matrix and x is an input vector:

y = Ax

Where:

- x = Original vector
- A = Transformation matrix
- y = Transformed vector

### 7. Dot Product After Transformation

Suppose two vectors x and y are transformed using the same matrix A.

Their transformed vectors are:

```text
x' = Ax

y' = Ay
```

The dot product of the transformed vectors is:

```text
x' · y' = (Ax)ᵀ(Ay)
```

Using the transpose property:

```text
(AB)ᵀ = BᵀAᵀ
```

Therefore:

```text
x' · y' = xᵀAᵀAy
```

This is an important relationship between dot product and linear transformation.

### 8. Orthogonal Transformation

An orthogonal transformation preserves the dot product between vectors.

For an orthogonal matrix A:

```text
AᵀA = I
```

The transformed dot product becomes:

```text
x' · y' = xᵀAᵀAy

        = xᵀIy

        = xᵀy
```

Therefore:

```text
(Ax) · (Ay) = x · y
```

An orthogonal transformation preserves:

- Vector lengths
- Angles between vectors
- Dot products
- Orthogonality

### 9. Rotation and Dot Product

A rotation matrix is an example of an orthogonal matrix.

For a 2D rotation:

```text
R(θ) = | cosθ  −sinθ |
       | sinθ   cosθ |
```

Its transpose is:

```text
Rᵀ(θ) = | cosθ   sinθ |
        | −sinθ  cosθ |
```

Multiplying:

```text
RᵀR = I
```

Therefore, rotation preserves the dot product.

If two vectors are rotated by the same angle, the angle between them remains unchanged.

### 10. Scaling and Dot Product

Consider a scaling matrix:

```text
A = | 2  0 |
    | 0  3 |
```

Let:

```text
x = | 1 |
    | 1 |

y = | 1 |
    | 1 |
```

Original dot product:

```text
x · y = (1 × 1) + (1 × 1)

      = 2
```

After transformation:

```text
Ax = | 2 |
     | 3 |

Ay = | 2 |
     | 3 |
```

New dot product:

```text
(Ax) · (Ay) = (2 × 2) + (3 × 3)

            = 4 + 9

            = 13
```

Therefore:

```text
Original Dot Product = 2

Transformed Dot Product = 13
```

Scaling does not generally preserve the dot product.

### 11. Important Properties of Dot Product

| Property | Formula |
|---|---|
| Commutative | u · v = v · u |
| Distributive | u · (v + w) = u · v + u · w |
| Scalar multiplication | (cu) · v = c(u · v) |
| Self dot product | u · u = ||u||² |
| Orthogonality | u · v = 0 |
| Geometric formula | u · v = ||u|| ||v|| cos θ |
| Matrix form | u · v = uᵀv |

### 12. Important Properties of Orthogonal Matrices

For an orthogonal matrix A:

```text
AᵀA = AAᵀ = I
```

Other properties:

- A⁻¹ = Aᵀ
- det(A) = ±1
- Lengths are preserved.
- Angles are preserved.
- Dot products are preserved.
- Orthogonal vectors remain orthogonal.
# Eigenvalues and Eigenvectors
## Lecture 10 – Linear Algebra

### 1. Eigenvectors

An eigenvector is a non-zero vector whose direction does not change when a linear transformation is applied to it.

A transformation may change the magnitude of the vector, but its direction remains along the same line.

Mathematically:

Av = λv

Where:

- A = Square transformation matrix
- v = Eigenvector
- λ = Eigenvalue
- Av = Transformed vector

An eigenvector must be non-zero.

### 2. Eigenvalues

An eigenvalue is a scalar value that represents how much an eigenvector is scaled during a linear transformation.

For an eigenvector v:

Av = λv

The eigenvalue λ determines the scaling factor.

- λ > 1: The vector is stretched.
- 0 < λ < 1: The vector is compressed.
- λ = 1: The vector remains unchanged.
- λ = 0: The vector is mapped to the zero vector.
- λ < 0: The vector's direction is reversed.

### 3. Geometric Meaning of Eigenvectors and Eigenvalues

In a linear transformation, most vectors may change both magnitude and direction.

However, eigenvectors are special because their direction remains unchanged or reversed along the same line.

The eigenvalue tells us how the eigenvector is scaled.

```text
Original eigenvector: v

After transformation: Av = λv
```

If λ is positive, the transformed vector points in the same direction.

If λ is negative, the transformed vector points in the opposite direction.

### 4. Example of Eigenvalues and Eigenvectors

Consider the matrix:

```text
A = | 2  0 |
    | 0  3 |
```

Let the first vector be:

```text
v₁ = | 1 |
     | 0 |
```

Applying the transformation:

```text
Av₁ = | 2  0 | | 1 |
      | 0  3 | | 0 |

    = | 2 |
      | 0 |
```

Therefore:

```text
Av₁ = 2v₁
```

So:

- Eigenvector: v₁ = (1, 0)
- Eigenvalue: λ₁ = 2

Now consider:

```text
v₂ = | 0 |
     | 1 |
```

Applying the transformation:

```text
Av₂ = | 2  0 | | 0 |
      | 0  3 | | 1 |

    = | 0 |
      | 3 |
```

Therefore:

```text
Av₂ = 3v₂
```

So:

- Eigenvector: v₂ = (0, 1)
- Eigenvalue: λ₂ = 3

### 5. Finding Eigenvalues

The eigenvalue equation is:

Av = λv

Rearranging:

Av − λv = 0

Taking v as a common factor:

(A − λI)v = 0

For a non-zero eigenvector to exist, the matrix must be singular.

Therefore:

det(A − λI) = 0

This equation is called the **characteristic equation**.

Solving it gives the eigenvalues.

### 6. Finding Eigenvalues of a 2 × 2 Matrix

Consider:

```text
A = | a  b |
    | c  d |
```

The identity matrix is:

```text
I = | 1  0 |
    | 0  1 |
```

Then:

```text
A − λI = | a − λ    b   |
         |   c     d − λ |
```

The characteristic equation is:

```text
det(A − λI) = 0
```

Therefore:

```text
| a − λ    b   |
|   c     d − λ | = 0
```

Expanding:

```text
(a − λ)(d − λ) − bc = 0
```

Simplifying:

```text
λ² − (a + d)λ + (ad − bc) = 0
```

This is the characteristic polynomial of a 2 × 2 matrix.

### 7. Example: Calculating Eigenvalues

Consider:

```text
A = | 2  0 |
    | 0  3 |
```

Step 1: Write the characteristic equation.

```text
det(A − λI) = 0
```

Step 2: Subtract λI from A.

```text
| 2 − λ    0   |
|   0     3 − λ |
```

Step 3: Calculate the determinant.

```text
(2 − λ)(3 − λ) = 0
```

Step 4: Solve the equation.

```text
2 − λ = 0  →  λ₁ = 2

3 − λ = 0  →  λ₂ = 3
```

Therefore, the eigenvalues are:

```text
λ₁ = 2
λ₂ = 3
```

### 8. Finding Eigenvectors

After finding the eigenvalues, substitute each eigenvalue into:

(A − λI)v = 0

Consider:

```text
A = | 2  0 |
    | 0  3 |
```

**For λ₁ = 2:**

```text
(A − 2I)v = 0

| 0  0 | | x | = | 0 |
| 0  1 | | y |   | 0 |
```

From the second equation:

y = 0

The value of x can be any non-zero number.

Choosing x = 1:

```text
v₁ = | 1 |
     | 0 |
```

**For λ₂ = 3:**

```text
(A − 3I)v = 0

| −1  0 | | x | = | 0 |
|  0  0 | | y |   | 0 |
```

From the first equation:

x = 0

The value of y can be any non-zero number.

Choosing y = 1:

```text
v₂ = | 0 |
     | 1 |
```

Therefore, the eigenvectors are:

```text
v₁ = | 1 |       v₂ = | 0 |
     | 0 |            | 1 |
```

### 9. Eigenvectors Are Not Unique

If v is an eigenvector corresponding to eigenvalue λ, then any non-zero scalar multiple of v is also an eigenvector corresponding to the same eigenvalue.

If:

Av = λv

Then:

A(cv) = λ(cv)

Where c is any non-zero scalar.

For example, if:

```text
v = | 1 |
    | 0 |
```

Then these are also eigenvectors for the same eigenvalue:

```text
| 2 |       | 5 |       | −3 |
| 0 |       | 0 |       |  0 |
```

All non-zero scalar multiples represent the same eigenvector direction.

### 10. Trace and Determinant of a Matrix

For a 2 × 2 matrix:

```text
A = | a  b |
    | c  d |
```

The trace is the sum of the diagonal elements:

```text
tr(A) = a + d
```

The determinant is:

```text
det(A) = ad − bc
```

For a 2 × 2 matrix, the eigenvalues satisfy:

```text
λ₁ + λ₂ = tr(A)
```

And:

```text
λ₁ × λ₂ = det(A)
```

### 11. Important Properties

| Property | Formula |
|---|---|
| Eigenvalue equation | Av = λv |
| Characteristic equation | det(A − λI) = 0 |
| Eigenvector equation | (A − λI)v = 0 |
| Sum of eigenvalues | Sum = tr(A) |
| Product of eigenvalues | Product = det(A) |
| Scalar multiple | A(cv) = λ(cv) |
| Zero eigenvalue | det(A) = 0, if A is square |
| Identity matrix | All eigenvalues are 1 |


