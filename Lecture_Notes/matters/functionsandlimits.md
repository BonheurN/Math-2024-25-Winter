# Functions to Draw in a Single Geogebra Notebook

The following functions should be plotted in a single Geogebra notebook:

1. Quadratic function:
   $$
   f(x) = x^2
   $$
   For \( x = 2 \):
   $$
   f(2) = 2^2 = 4
   $$

2. Linear function:
   $$
   g(x) = x
   $$
 For \( x = 2 \):
   $$
   g(2) = 2
   $$
3. Reciprocal function:
   $$
   h(x) = \frac{1}{x}
   $$
 For \( x = 2 \):
   $$
   h(4) = \frac{1}{2} = 0.5
   $$

4. Sine function:
   $$
   j(x) = \sin(x)
   $$
for \(x = 2 \):
$$
j(2) = sin(2) = 1
$$
Let \( f(x) = 3x - 1 \) and \( g(x) = x \). Find the following:

### 1. $( f(g(x)) $)
Substitute $( g(x) = x $) into $( f(x) = 3x - 1 $):

$[
f(g(x)) = f(x) = 3x - 1
$]

**Solution**: $( f(g(x)) = 3x - 1 $)

---

### 2. $( g(f(x)) $)
Substitute $( f(x) = 3x - 1 $) into $( g(x) = x $):

$[
g(f(x)) = g(3x - 1) = 3x - 1
$]

**Solution**: $( g(f(x)) = 3x - 1 $)

---

### 3. $( f(f(x)) $)
Substitute $( f(x) = 3x - 1 $) into itself:

$[
f(f(x)) = f(3x - 1) = 3(3x - 1) - 1 = 9x - 3 - 1 = 9x - 4
$]

**Solution**: $( f(f(x)) = 9x - 4 $)

---

### 4. $( g(g(x)) $)
Substitute $( g(x) = x $) into itself:

$[
g(g(x)) = g(x) = x
$]

**Solution**: $( g(g(x)) = x $)


![mixed functions](mixe.png)
----

Here's the solution in Markdown with the math environment enclosed in `$$`.

---

### Problem 1: Composite Functions with \( f(x) = e^x \) and \( g(x) = \ln(x) \)
#### Given:
\( f(x) = e^x \)  
\( g(x) = \ln(x) \)

#### To Check:
1. \( f(g(x)) \):  
   Substitute \( g(x) = \ln(x) \) into \( f(x) \):  
   $$ f(g(x)) = f(\ln(x)) = e^{\ln(x)} = x $$

2. \( g(f(x)) \):  
   Substitute \( f(x) = e^x \) into \( g(x) \):  
   $$ g(f(x)) = g(e^x) = \ln(e^x) = x $$

#### Notice:
Both \( f(g(x)) \) and \( g(f(x)) \) return \( x \). This shows that \( f \) and \( g \) are inverses of each other.

---

### Problem 2: Inverse of the Function \( f = \{(1, 7), (2, 9), (3, 11)\} \)

#### To Find \( f^{-1} \):  
Swap the \( x \)- and \( y \)-values:  
$$ f^{-1} = \{(7, 1), (9, 2), (11, 3)\} $$

---

### Problem 3: Inverse of the Function $( f = ${(1, 7), (2, 7), (3, 11)$} $)

#### To Find ( f^{-1} $):  
Swap the $( x $)- and \( y \)-values:  
$$ f^{-1} = ${(7, 1), (7, 2), (11, 3)$} $$  

#### Note:  
Since $( f $) is not one-to-one (two $( x $)-values map to the same $( y $)-value, e.g., $( 1 \to 7 $) and $( 2 \to 7 $)), $( f^{-1} $) is not a function.

---

### Problem 4: Inverse of the Function $( f(x) = x - 1 $)

#### Given:  
$( f(x) = x - 1 $)

#### To Find $( f^{-1}(x) $):  
1. Set $( y = f(x) $):  
   $$ y = x - 1 $$

2. Solve for $( x $):  
   $$ x = y + 1 $$

3. Replace $( x $) with $( f^{-1}(x) $):  
   $$ f^{-1}(x) = x + 1 $$

#### Show Both Functions in GeoGebra:
- Plot $( f(x) = x - 1 $) and $( f^{-1}(x) = x + 1 $) in GeoGebra.  
- The two functions are reflections of each other across the line $( y = x $).

---
