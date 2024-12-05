# Mathematics Exercises 2024/2025 - Solutions

---

## 1. Basic Operations on Matrices

### Given Matrices:

$$
A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}, 
B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}, 
C = \begin{bmatrix} -1 & 2 \\ 3 & 0 \end{bmatrix}
$$


---

### Matrix Addition:

1. **\( A + B \):**
$$
A + B = \begin{bmatrix} 6 & 8 \\ 10 & 12 \end{bmatrix}
$$

2. **\( B - A \):**
$$
B - A = \begin{bmatrix} 4 & 4 \\ 4 & 4 \end{bmatrix}
$$

---

### Scalar Multiplication:
1. **\( \frac{1}{2}A \):**
$$
\frac{1}{2}A = \begin{bmatrix} 0.5 & 1.0 \\ 1.5 & 2.0 \end{bmatrix}
$$

---

### Matrix Multiplication:
1. **\( A \cdot B \):**
$$
A \cdot B = \begin{bmatrix} 19 & 22 \\ 43 & 50 \end{bmatrix}
$$

---

## 2. Determinants (2x2 Matrices)

### Given Matrices:
$$
A = \begin{bmatrix} 2 & 3 \\ 1 & 4 \end{bmatrix}, 
B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}, 
C = \begin{bmatrix} -1 & 2 \\ 3 & 0 \end{bmatrix}
$$

### Calculations:
1. **\( \text{det}(A) \):**
$$
\text{det}(A) = 2 \cdot 4 - 3 \cdot 1 = 5
$$

2. **\( \text{det}(B) \):**
$$
\text{det}(B) = 5 \cdot 8 - 6 \cdot 7 = -2
$$

3. **\( \text{det}(C) \):**
$$
\text{det}(C) = (-1) \cdot 0 - 2 \cdot 3 = -6
$$

---

## 3. Determinants Using Laplace's Expansion
Given matrix \( A \):
$$
A = \begin{bmatrix} 2 & 3 & 1 \\ 1 & 4 & 0 \\ 3 & 2 & 1 \end{bmatrix}
$$

### Solution:
$$
\text{det}(A) = 14
$$

---
## 4. Determinants via Gauss Method

Given matrix \( A \):
$$
A = \begin{bmatrix} 12 & 3 \\ -18 & -4 \end{bmatrix}
$$

### Step 1: Recall the Gauss Method
The determinant of a matrix can be computed by reducing the matrix to an upper triangular form using row operations. For a \( 2 \times 2 \) matrix:

$$
A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}
$$

The determinant is given by:

$$
\text{det}(A) = ad - bc
$$

### Step 2: Identify Row Operations
The determinant remains unchanged under the following operations:
- Adding or subtracting a multiple of one row from another.

However, the determinant changes in the following ways:
1. Swapping two rows multiplies the determinant by \( -1 \).
2. Scaling a row by a factor \( k \) multiplies the determinant by \( k \).

### Step 3: Apply Row Operations
Given matrix \( A \):
$$
A = \begin{bmatrix} 12 & 3 \\ -18 & -4 \end{bmatrix}
$$

#### Step 3.1: Make the bottom-left entry (\( -18 \)) zero
We aim to make \( c = 0 \) in the second row (\( R_2 \)) using row operations.

Perform the row operation:

$$
R_2 \rightarrow R_2 + \frac{18}{12} R_1 = R_2 + 1.5 R_1
$$

This gives:

$$
A' = \begin{bmatrix} 12 & 3 \\ 0 & 0.5 \end{bmatrix}
$$

#### Step 3.2: Compute the determinant
The determinant of an upper triangular matrix is the product of the diagonal elements. For \( A' \):

$$
\text{det}(A') = 12 \cdot 0.5 = 6
$$

### Final Answer
The determinant of the matrix \( A \) is:

$$
\text{det}(A) = 6
$$

---

## 5. Inverse of a Matrix
Matrix \( A \):
$$
A = \begin{bmatrix} 2 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 2 & 0 \end{bmatrix}
$$

### Solution:
$$
A^{-1} = \begin{bmatrix} 0 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & -2 & -2 \end{bmatrix}
$$

---

## 6. Inverse Using Gauss Method
Matrix \( B \):
$$
B = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 1 \\ 2 & 3 & 2 \end{bmatrix}
$$

### Solution:
$$
B^{-1} = \begin{bmatrix} -7 & 8 & -1 \\ 3 & -4 & 1 \\ 1 & -1 & 0 \end{bmatrix}
$$

---
