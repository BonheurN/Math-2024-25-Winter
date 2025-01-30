# 24. Integrals
 1.Compute



i) $\int_{1}^{d} x \, dx,$

we first note that the antiderivative of $x$ is $\frac{x^2}{2}$. Therefore,

$$
\int_{1}^{d} x \, dx 
= \left.\frac{x^2}{2}\right|_{1}^{d}
= \frac{d^2}{2} \;-\; \frac{1^2}{2}
= \frac{d^2 - 1}{2}.
$$

---

ii) $ \int (x^2 + 2)\,dx $

To integrate $ \int (x^2 + 2)\,dx $, handle each term separately:

1. $ \int x^2 \, dx = \frac{x^3}{3} $.
2. $ \int 2 \, dx = 2x $.

Combining these results gives:

$$
\int (x^2 + 2)\,dx = \frac{x^3}{3} + 2x + C,
$$
where $C$ is the constant of integration.

---

iii) $\int 2 \sin(x) \, dx$

The integral you provided is:

$$
\int 2 \sin(x) \, dx
$$

To compute the integral, we apply the following basic rule of integration for sine functions:

$$
\int \sin(x) \, dx = -\cos(x)
$$

Thus, for your integral:

$$
\int 2 \sin(x) \, dx = 2 \cdot (-\cos(x)) = -2 \cos(x) + C
$$

Where $ C $ is the constant of integration.

---

iv)  $ \int 3x \, dx $

To integrate $ \int 3x \, dx $, factor out the constant 3 and then integrate $x$:

$$
\int 3x \, dx = 3 \int x \, dx = 3 \cdot \frac{x^2}{2} = \frac{3x^2}{2} + C,
$$

where $C$ is the constant of integration.

---

v) $\int \frac{1}{x^2} \, dx,$

To integrate

$$
\int \frac{1}{x^2} \, dx,
$$


it often helps to rewrite $ \frac{1}{x^2} $ as $ x^{-2} $:

$$
\int \frac{1}{x^2} \, dx = \int x^{-2} \, dx.
$$

The integral of $x^n$ is $\frac{x^{n+1}}{n+1}$, as long as $n \neq -1$. Here, $n = -2$, so:

$$
\int x^{-2} \, dx = \frac{x^{-2 + 1}}{-2 + 1} = \frac{x^{-1}}{-1} = -x^{-1} + C.
$$

Rewriting $x^{-1}$ as $\frac{1}{x}$, we get:

$$
\int \frac{1}{x^2} \, dx = -\frac{1}{x} + C,
$$

where $C$ is the constant of integration.

---
vi)$\int \left( \frac{1}{3} x^4 - 5 \right) \, dx$

The integral you provided is:

$$
\int \left( \frac{1}{3} x^4 - 5 \right) \, dx
$$

We will compute the integral by handling each term separately:

 For the first term $\int \frac{1}{3} x^4 \, dx$, apply the power rule of integration: 
   $$
   \int x^n \, dx = \frac{x^{n+1}}{n+1}
   $$
   This gives us:
   $$
   \int \frac{1}{3} x^4 \, dx = \frac{1}{3} \cdot \frac{x^5}{5} = \frac{x^5}{15}
   $$

 For the second term $\int -5 \, dx$, simply multiply by $x$:
   $$
   \int -5 \, dx = -5x
   $$

Thus, the result of the integral is:

$$
\frac{x^5}{15} - 5x + C
$$

Where $C$ is the constant of integration.

---

vii) $\int \left( \sin^2(x) + \cos^2(x) \right) \, dx$

The integral you provided is:

$$
\int \left( \sin^2(x) + \cos^2(x) \right) \, dx
$$

Using the Pythagorean identity:

$$
\sin^2(x) + \cos^2(x) = 1
$$

The integral simplifies to:

$$
\int 1 \, dx
$$

The result is simply:

$$
x + C
$$

Where $ C $ is the constant of integration.

---

viii) The integral you provided is:

$$
\int \sqrt[3]{x} \, dx
$$

We can rewrite $\sqrt[3]{x}$ as $x^{1/3}$, so the integral becomes:

$$
\int x^{1/3} \, dx
$$

Using the power rule for integration:

$$
\int x^n \, dx = \frac{x^{n+1}}{n+1}
$$

For $n = \frac{1}{3}$, we get:

$$
\int x^{1/3} \, dx = \frac{x^{4/3}}{4/3} = \frac{3}{4} x^{4/3}
$$

Thus, the result of the integral is:

$$
\frac{3}{4} x^{4/3} + C
$$

Where $ C $ is the constant of integration.

viii) $\int \sqrt[3]{x} \, dx$

The integral you provided is:

$$
\int \sqrt[3]{x} \, dx
$$

We can rewrite $\sqrt[3]{x}$ as $x^{1/3}$, so the integral becomes:

$$
\int x^{1/3} \, dx
$$

Using the power rule for integration:

$$
\int x^n \, dx = \frac{x^{n+1}}{n+1}
$$

For $n = \frac{1}{3}$, we get:

$$
\int x^{1/3} \, dx = \frac{x^{4/3}}{4/3} = \frac{3}{4} x^{4/3}
$$

Thus, the result of the integral is:

$$
\frac{3}{4} x^{4/3} + C
$$

Where $ C $ is the constant of integration.