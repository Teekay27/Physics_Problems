## 9. Vector Lorentz Force — Solution

We use the magnetic Lorentz force:

$$
\vec F = q\, \vec v \times \vec B
$$

---

## 1. Compute Cross Product $\vec v \times \vec B$

$$
\vec v = (2, -4, 1), \quad \vec B = (1, 2, -1)
$$

$$
\vec v \times \vec B =
\begin{vmatrix}
\hat i & \hat j & \hat k \\
2 & -4 & 1 \\
1 & 2 & -1
\end{vmatrix}
$$

Expand:

$$
= \hat i((-4)(-1) - (1)(2))
- \hat j((2)(-1) - (1)(1))
+ \hat k((2)(2) - (-4)(1))
$$

$$
= \hat i(4 - 2)
- \hat j(-2 - 1)
+ \hat k(4 + 4)
$$

$$
= (2, 3, 8)
$$

---

## 2. Magnitude of Cross Product

$$
|\vec v \times \vec B| = \sqrt{2^2 + 3^2 + 8^2}
= \sqrt{4 + 9 + 64}
= \sqrt{77}
$$

---

## 3. Multiply by Charge

For a proton:
$$
q = 1.6 \times 10^{-19}\,\text{C}
$$

$$
F = q |\vec v \times \vec B|
= (1.6 \times 10^{-19}) \sqrt{77}
$$

$$
F \approx (1.6 \times 10^{-19})(8.77)
\approx 1.4 \times 10^{-18}\,\text{N}
$$

---

## Final Answer

$$
\boxed{F \approx 1.4 \times 10^{-18}\,\text{N}}
$$