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

Split the integral:

```math
a_0
=
\frac{1}{\pi}
\left(
\int_{-\pi}^{\pi}x\,dx
+
\int_{-\pi}^{\pi}\pi\,dx
\right)
```

Since

```math
\int_{-\pi}^{\pi}x\,dx=0
```


and


```math
\int_{-\pi}^{\pi}\pi\,dx
=
2\pi^2
```

we get


```math
a_0=2\pi
```


thus


```math
\frac{a_0}{2}=\pi
```

---
## Step 3:Determination of Cosine Coefficients (aₙ)

Using the definition of

```math
a_n
```

```math
a_n
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
(x+\pi)\cos(nx)\,dx
```

Split the integral:

```math
a_n
=
\frac{1}{\pi}
\left[
\int_{-\pi}^{\pi}
x\cos(nx)\,dx
+
\pi
\int_{-\pi}^{\pi}
\cos(nx)\,dx
\right]
```

Because

```math
x
```

is odd and

```math
\cos(nx)
```

is even,

```math
x\cos(nx)
```

is an odd function.



Therefore,

```math
\int_{-\pi}^{\pi}
x\cos(nx)\,dx
=
0
```

Also,

```math
\int_{-\pi}^{\pi}
\cos(nx)\,dx
=
\left[
\frac{\sin(nx)}{n}
\right]_{-\pi}^{\pi}
=
0
```

Thus,

```math
a_n=0
```

---

## Step 4: Set Up the Sine Coefficient Formula

Using the definition of

```math
b_n
```

```math
b_n
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
(x+\pi)\sin(nx)\,dx
```

The constant term contributes nothing because

```math
\int_{-\pi}^{\pi}
\sin(nx)\,dx
=
0
```

Therefore,


```math
b_n
=
\frac{1}{\pi}
\int_{-\pi}^{\pi}
x\sin(nx)\,dx
```


Since both

```math
x
```

and


```math
\sin(nx)
```


are odd functions, their product is even:


```math
b_n
=
\frac{2}{\pi}
\int_{0}^{\pi}
x\sin(nx)\,dx
```

---

## Step 5: Apply Integration by Parts

Let

```math
u=x
```

and

```math
dv=\sin(nx)\,dx
```

Then

```math
du=dx
```

```math
v=-\frac{\cos(nx)}{n}
```

Applying integration by parts:

```math
\int_{0}^{\pi}
x\sin(nx)\,dx
=
-\frac{x\cos(nx)}{n}
\Bigg|_{0}^{\pi}
+
\frac{1}{n}
\int_{0}^{\pi}
\cos(nx)\,dx
```

The remaining integral is

```math
\int_{0}^{\pi}
\cos(nx)\,dx
=
\frac{\sin(n\pi)}{n}
=
0
```

Therefore,

```math
\int_{0}^{\pi}
x\sin(nx)\,dx
=
-\frac{\pi\cos(n\pi)}{n}
```

---

## Step 6: Simplify the Expression for bₙ

Using

```math
\cos(n\pi)=(-1)^n
```
