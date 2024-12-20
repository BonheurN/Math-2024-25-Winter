---
format:
  html:
    toc: true
    toc-location: left
    toc-depth: 3
    page-layout: full
    grid:
      body-width: 1000px
      sidebar-width: 300px
      margin-width: 300px
      gutter-width: 2rem
    theme:
      light: [flatly, custom.scss]
      dark: [darkly, custom.scss]
    self-contained: true
---

## What is a function?

**Set-theory definition of a function** states that a function $f$ is a special case of a relation. A relation is simply any set of ordered pairs. A function, on the other hand, is a relation $f \subseteq X \times Y$ that satisfies an additional condition: for each element $x \in X$, there is **exactly one** element $y \in Y$ assigned to it.

Formally, a function $f$ is a relation that satisfies the following condition:

$$
\forall x_1, x_2 \in X, \, \forall y_1, y_2 \in Y \, \left( (x_1, y_1) \in f \land (x_2, y_2) \in f : (x_1 = x_2) \Rightarrow (y_1 = y_2) \right)
$$

This means that if for the same $x_1$ we have two pairs $(x_1, y_1)$ and $(x_1, y_2)$, then $y_1$ must be equal to $y_2$. In other words, no element from $X$ can be "associated" with more than one element from $Y$.

#### Important Points:
1. **Relation** in set theory is simply a set of ordered pairs $(x, y)$, where $x$ comes from set $X$ and $y$ comes from set $Y$.
2. **Function** is a relation that additionally satisfies the condition that for every $x$ there is exactly one pair $(x, y)$ in this relation.

Thus, a function $f \subseteq X \times Y$ is a relation that satisfies the additional condition that for each $x \in X$ there is exactly one $y \in Y$ such that $(x, y) \in f$.

#### Examples

**Example 1**

$$
f=\{(\text{dog}, \text{pies}), (\text{cat}, \text{kot}), (\text{horse}, \text{ko\'n})\}
$$

**Example 2**

$$
f=\{(1,2), (2,3), (3,4)\}
$$

This means that $f(1)=2$, $f(2)=3$, and $f(3)=4$.

**Example 3**

$$
f=\{(1,1),(2,1/2),(3,1/3),...\}=\{(n,1/n): n \in \mathbb{N}\}
$$

```python
import numpy as np
import matplotlib.pyplot as plt

def f(n):
    return 1/n

fig, ax = plt.subplots(figsize=(6,4))
n=np.arange(1,20)
plt.scatter(n,f(n))
plt.xlabel('n')
plt.ylabel('f(n)')
plt.xticks(np.arange(1,20,1))
plt.show()
```

where $\mathbb{N}$ denotes the set of natural numbers. This function assigns each $n$ the value $1/n$.

We often denote sequences using $f(n)=1/n$.

**Example 4**

The quadratic function often written as $f(x)=x^2$ is a function that assigns each $x$ the value $x^2$. In our notation, we write this as

$$
f=\{(x,x^2): x \in \mathbb{R}\}
$$

where $\mathbb{R}$ denotes the set of real numbers.

```python
def f(x):
    return x**2

fig, ax = plt.subplots(figsize=(6,4))
x=np.linspace(-10,10,100)
plt.plot(x,f(x))
plt.xlabel('x')
plt.ylabel('f(x)')
plt.show()
```

**Example 5**

The determinant of a matrix is a function that assigns each matrix a number. In our notation, we write this as

$$
f=\{(M,\text{det}(M)): M \text{ is a square matrix}\}
$$

**Example 6**

A matrix itself is also a function that assigns each pair of indices $(i,j)$ where $i,j \in \{1,2,...,n\}$ the element of the matrix at position $(i,j)$. In our notation, we write this as

$$
M=\{((i,j),M_{ij}): i,j \in \{1,2,...,n\}\}
$$

for convenience, we write this as a two-dimensional array:

$$
M=\begin{bmatrix}
M_{11} & M_{12} & \cdots & M_{1n} \\
M_{21} & M_{22} & \cdots & M_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
M_{n1} & M_{n2} & \cdots & M_{nn}
\end{bmatrix}
$$

**Example 7**

Matrix addition is a function that assigns each pair of matrices their sum. In our notation, we write this as

$$
f=\{((A,B),A+B): A,B \text{ are matrices of the same dimensions}\}
$$

where $A+B$ is the matrix whose elements are the sums of the elements of matrices $A$ and $B$, that is, for each $i,j$ we have 
$$
(A+B)_{ij}=A_{ij}+B_{ij}
$$

**Example 8**

A dictionary in Python is also a function that assigns each key a value. In our notation, we write this as:

```python
d={'a':1, 'b':2, 'c':3}
```

## Limits of functions

### Sequences

An idea of a limit of sequence is very simple. It is a number that the sequence approaches as we take more and more elements of the sequence. For example, the sequence $a_n=\frac{1}{n}$ approaches 0 as we take more and more elements of the sequence. We write this as

$$
\lim_{n \to \infty} a_n=0
$$

Formal definition of a limit of a sequence is as follows:

 {.definition}
**Definition: Limit of a sequence**

A number $g$ is the limit of a sequence $a_n$ if for every $\varepsilon>0$ there exists $N$ such that for every $n>N$ we have $|a_n-g|<\epsilon$. 
We write this as $$\lim_{n \to \infty} a_n=g$$.


# Visualization of Limit of a Sequence

The following Python script visualizes the behavior of the sequence $( a(n) = \frac{3n^2}{n^2 + 1} $) as $( n \to \infty $), demonstrating its convergence to the limit $( L = 3 $).

# Visualization of Limit of a Sequence

The following Python script visualizes the behavior of the sequence $( a(n) = \frac{3n^2}{n^2 + 1} $) as $( n \to \infty $), demonstrating its convergence to the limit $( L = 3 $).

```python
import numpy as np
import matplotlib.pyplot as plt

# Function definition
def a(n):
    return 3 * n**2 / (n**2 + 1)

# Parameters for visualization
epsilon = 0.1  # Epsilon value to represent the "margin" around the limit
N = 6  # Chosen N for the definition of limit

# Generate data points
n = np.arange(1, 20)  # Range of n values for plotting
a_values = a(n)  # Compute the function values

# Compute the limit for large n (L = 3)
limit = 3

# Create the plot
fig, ax = plt.subplots(figsize=(8, 5))
plt.scatter(n, a_values, label="Sequence $a(n) = \\frac{3n^2}{n^2 + 1}$", color="blue")  # Sequence points
plt.axhline(y=limit, color="green", linestyle="-", label="Limit $L = 3$")  # The limit line
plt.axhline(y=limit + epsilon, color="red", linestyle="--", label="$L + \\varepsilon$")  # Upper epsilon bound
plt.axhline(y=limit - epsilon, color="red", linestyle="--", label="$L - \\varepsilon$")  # Lower epsilon bound
plt.axvline(x=N, color="orange", linestyle="--", label="$N = 6$")  # Vertical line for N

# Annotate the plot
plt.title("Visualization of Limit of $a(n)$ as $n \\to \\infty$")
plt.xlabel("$n$")
plt.ylabel("$a(n)$")
plt.legend()
plt.grid()
plt.show()
