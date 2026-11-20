Lecutre 2

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
