## 9. Linear Equations by Gauss Elimination

### System 1:
$$
\begin{cases}
x + 2y - 2z = 4 \\
2x + y + z = 0 \\
3x + 2y + z = 1
\end{cases}
$$

We can solve this system using Gaussian elimination by converting the system of equations into an augmented matrix and then performing row operations.

**Augmented matrix:**
$$
\begin{bmatrix}
1 & 2 & -2 & | & 4 \\
2 & 1 & 1 & | & 0 \\
3 & 2 & 1 & | & 1
\end{bmatrix}
$$

Perform row operations:


1. ( R_2 \to R_2 - 2R_1 \)
2. ( R_3 \to R_3 - 3R_1 \)



**Matrix after row operations:**
$$
\begin{bmatrix}
1 & 2 & -2 & | & 4 \\
0 & -3 & 5 & | & -8 \\
0 & -4 & 7 & | & -11
\end{bmatrix}
$$

Next, perform the second row operation:
1. \( R_3 \to R_3 - \frac{4}{3}R_2 \)

**Matrix after row operations:**
$$
\begin{bmatrix}
1 & 2 & -2 & | & 4 \\
0 & -3 & 5 & | & -8 \\
0 & 0 & \frac{1}{3} & | & \frac{1}{3}
\end{bmatrix}
$$

Back substitution will give the values for \( x \), \( y \), and \( z \).

---

### System 2:
$$
\begin{cases}
x + y + z - t = 2 \\
2x + y + z = 3 \\
-x + z - t = 0 \\
3x + 2y - z + 2t = -1
\end{cases}
$$

Follow the same Gaussian elimination method to solve for \( x \), \( y \), \( z \), and \( t \). After converting the system into an augmented matrix and performing row operations, you'll arrive at the solution.

---

### System 3:
$$
\begin{cases}
x + y - z - t = 0 \\
2x + 3y - 2z + t = 4 \\
3x + 5z = 0 \\
-x + y - 3z + 2t = 3
\end{cases}
$$

Again, use Gaussian elimination to solve this system step by step.

---

## 10. Linear Equations by Matrix Inversion

### 1. Solve the system of linear equations:

$$
\begin{cases}
x + 2y + 3z = 5 \\
2y + 3z = 4 \\
3z = 3
\end{cases}
$$

We can write this system in matrix form as:

$$
\begin{bmatrix}
1 & 2 & 3 \\
0 & 2 & 3 \\
0 & 0 & 3
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
=
\begin{bmatrix}
5 \\
4 \\
3
\end{bmatrix}
$$

To solve, find the inverse of the coefficient matrix and multiply it by the right-hand side vector.

**Inverse of matrix:**
Use the formula for the inverse of a 3x3 matrix and apply it to the given coefficient matrix.

---

### 2. Solve the system of linear equations:

$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 41 \\
4x_1 + 5x_2 + 6x_3 = 93 \\
7x_1 + 8x_2 + 9x_3 = 145
\end{cases}
$$

Write the system in matrix form and apply matrix inversion.

$$
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2 \\
x_3
\end{bmatrix}
=
\begin{bmatrix}
41 \\
93 \\
145
\end{bmatrix}
$$

Find the inverse of the matrix and multiply by the right-hand side vector to solve for \( x_1 \), \( x_2 \), and \( x_3 \).

---

## 11. Vectors I

### 1. Multiply vector \( \mathbf{a} = [3, 4] \) by a scalar to make its length equal to 1.

First, calculate the length (magnitude) of \( \mathbf{a} \):

$$
|\mathbf{a}| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5
$$

To make the length equal to 1, multiply \( \mathbf{a} \) by \( \frac{1}{|\mathbf{a}|} = \frac{1}{5} \):

$$
\mathbf{a}_{\text{unit}} = \frac{1}{5} \cdot [3, 4] = [\frac{3}{5}, \frac{4}{5}]
$$

### 2. Calculate the length of vector \( \mathbf{b} = [1, 1] \) and find the unit vector.

The length of \( \mathbf{b} \) is:

$$
|\mathbf{b}| = \sqrt{1^2 + 1^2} = \sqrt{2}
$$

The unit vector is:

$$
\mathbf{b}_{\text{unit}} = \frac{1}{|\mathbf{b}|} \cdot \mathbf{b} = \frac{1}{\sqrt{2}} \cdot [1, 1] = [\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}]
$$

### 3. Plot the vector and the unit vector:

You can plot these vectors on a 2D coordinate system. The vector \( \mathbf{b} = [1, 1] \) points from the origin to the point (1,1), and the unit vector points to \( [\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}] \).

### 4. Calculate the length of vector \( \mathbf{c} = [1, 2, 3] \) and find the unit vector.

The length of \( \mathbf{c} \) is:

$$
|\mathbf{c}| = \sqrt{1^2 + 2^2 + 3^2} = \sqrt{1 + 4 + 9} = \sqrt{14}
$$

The unit vector is:

$$
\mathbf{c}_{\text{unit}} = \frac{1}{\sqrt{14}} \cdot [1, 2, 3] = [\frac{1}{\sqrt{14}}, \frac{2}{\sqrt{14}}, \frac{3}{\sqrt{14}}]
$$

### 5. Find the Cartesian coordinates of vector \( \mathbf{v} = [2, 3, 4] \) in the basis \( \{\mathbf{b_1} = [1, 0, 1], \mathbf{b_2} = [0, 1, 0], \mathbf{b_3} = [1, 0, -1]\} \).

We solve the system of equations for \( c_1, c_2, c_3 \):

$$
\mathbf{v} = c_1 \mathbf{b_1} + c_2 \mathbf{b_2} + c_3 \mathbf{b_3}
$$

$$
[2, 3, 4] = c_1 [1, 0, 1] + c_2 [0, 1, 0] + c_3 [1, 0, -1]
$$

This gives the following system of equations:

$$
\begin{cases}
c_1 + c_3 = 2 \\
c_2 = 3 \\
c_1 - c_3 = 4
\end{cases}
$$

Solving this system, we find \( c_1 = 3, c_2 = 3, c_3 = -1 \).

Thus, the coordinates of \( \mathbf{v} \) in the new basis are \( [3, 3, -1] \).

---

## 12. Vectors II

### 1. Perform the addition of vectors \( [2, 1] \) and \( [-1, 1] \).

$$
[2, 1] + [-1, 1] = [2 - 1, 1 + 1] = [1, 2]
$$
