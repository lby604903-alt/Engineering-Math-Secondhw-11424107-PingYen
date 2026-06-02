# 11424107: Laplace Transformation (2)

Condition:

```math
f(x)=x+\pi
```

```math
-\pi \le x \le \pi
```

---
## Step 1: Fourier Series Formula

The given function is

```math
f(x)=x+\pi
```

defined on the interval

```math
[-\pi,\pi]
```

the Fourier series is

```math
f(x)
=
\frac{a_0}{2}
+
\sum_{n=1}^{\infty}
\left(
a_n\cos(nx)
+
b_n\sin(nx)
\right)
```

The coefficients are defined as:

```math
a_n
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
f(x)\cos(nx)\,dx
```

```math
b_n
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
f(x)\sin(nx)\,dx
```

```math
a_0
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
f(x)\,dx
```
---

## Step 2:Computation of the Constant Coefficient (a₀)

```math
a_0
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
(x+\pi)\,dx
```
