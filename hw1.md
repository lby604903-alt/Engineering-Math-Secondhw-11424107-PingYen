# 11424107: Laplace Transformation (2)

Solve the differential equation

```math
2\frac{d^2x}{dt^2}
+
7\frac{dx}{dt}
+
3x
=
0
```

with the initial conditions

```math
x(0)=0
```

```math
x'(0)=1
```

---
# Step 1: Transform the Equation into the s-Domain

Let

```math
X(s)=\mathcal{L}\{x(t)\}
```

Using the Laplace transform formulas

```math
\mathcal{L}\{x'(t)\}
=
sX(s)-x(0)
```

```math
\mathcal{L}\{x''(t)\}
=
s^2X(s)-sx(0)-x'(0)
```
Substitute the initial conditions

```math
x(0)=0
```

```math
x'(0)=1
```

Then


```math
\mathcal{L}\{x''(t)\}
=
s^2X(s)-1
```

```math
\mathcal{L}\{x'(t)\}
=
sX(s)
```

Substituting into the differential equation gives

```math
2(s^2X(s)-1)
+
7sX(s)
+
3X(s)
=
0
```
---

# Step 2: Determine the Expression for X(s)

Expand:

```math
2s^2X(s)
-
2
+
7sX(s)
+
3X(s)
=
0
```

Factor out $X(s)$:

```math
X(s)
\left(
2s^2+7s+3
\right)
=
2
```

Therefore

```math
X(s)
=
\frac{2}
{2s^2+7s+3}
```

Factor the denominator:

```math
2s^2+7s+3
=
(2s+1)(s+3)
```

Hence

```math
X(s)
=
\frac{2}
{(2s+1)(s+3)}
```

---

# Step 3: Simplify Using Partial Fractions

Assume

```math
\frac{2}
{(2s+1)(s+3)}
=
\frac{A}{2s+1}
+
\frac{B}{s+3}
```

Multiply both sides by $(2s+1)(s+3)$:

```math
2
=
A(s+3)
+
B(2s+1)
```

Expand:

```math
2
=
(A+2B)s
+
(3A+B)
```

Compare coefficients:

```math
A+2B=0
```

```math
3A+B=2
```

From

```math
A=-2B
```

Substitute into the second equation:

```math
3(-2B)+B=2
```

```math
-5B=2
```

```math
B=-\frac{2}{5}
```

Thus

```math
A=\frac{4}{5}
```

Therefore

```math
X(s)
=
\frac{\frac45}{2s+1}
-
\frac{\frac25}{s+3}
```

Rewrite as

```math
X(s)
=
\frac25
\frac1{s+\frac12}
-
\frac25
\frac1{s+3}
```

---

# Step 4: Recover the Solution in the Time Domain
