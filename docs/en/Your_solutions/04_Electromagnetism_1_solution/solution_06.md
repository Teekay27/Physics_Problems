## 6. Field at a Point from a System of Charges — Solution

Two charges:
- $+q$ at $(-a,0)$  
- $+2q$ at $(a,0)$  

Using superposition:
$$
\vec E = \vec E_1 + \vec E_2
$$

---

## 1. General Field $\vec E(x,y)$

Position vectors from charges:

$$
\vec r_1 = (x + a, y), \quad r_1 = \sqrt{(x+a)^2 + y^2}
$$

$$
\vec r_2 = (x - a, y), \quad r_2 = \sqrt{(x-a)^2 + y^2}
$$

Electric field:

$$
\vec E(x,y) =
kq \frac{(x+a, y)}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
k(2q) \frac{(x-a, y)}{\left[(x-a)^2 + y^2\right]^{3/2}}
$$

---

## Special Cases

### (a) Along $y$-axis: $\vec E(0,y)$

$$
E_x = kq \frac{a}{(a^2 + y^2)^{3/2}} - 2kq \frac{a}{(a^2 + y^2)^{3/2}}
= -kq \frac{a}{(a^2 + y^2)^{3/2}}
$$

$$
E_y = kq \frac{y}{(a^2 + y^2)^{3/2}} + 2kq \frac{y}{(a^2 + y^2)^{3/2}}
= 3kq \frac{y}{(a^2 + y^2)^{3/2}}
$$

---

### (b) Along $x$-axis: $\vec E(x,0)$

$$
E_x = kq \frac{x+a}{|x+a|^3} + 2kq \frac{x-a}{|x-a|^3}
$$

$$
E_y = 0
$$

---

## 2. Conditions

### $E_y = 0$
From general form:
$$
y = 0
$$

---

### $E_x = 0$ (on x-axis)

Solve:
$$
\frac{q}{(x+a)^2} = \frac{2q}{(x-a)^2}
$$

$$
(x-a)^2 = 2(x+a)^2
$$

This gives equilibrium point between charges.

---

### $\vec E = 0$

Occurs only on the $x$-axis between the charges (since $E_y=0$ required).

---

## 3. Numerical Calculation

Given:
- $a = 0.2\,\text{m}$
- $y = 0.3\,\text{m}$
- $q = 2 \times 10^{-6}\,\text{C}$
- $k = 8.99 \times 10^9$

First compute:
$$
r^2 = a^2 + y^2 = 0.04 + 0.09 = 0.13
$$

$$
r^3 = (0.13)^{3/2} \approx 0.0469
$$

---

### Components:

$$
E_x = -kq \frac{a}{r^3}
= - (8.99 \times 10^9)(2 \times 10^{-6}) \frac{0.2}{0.0469}
$$

$$
E_x \approx -7.7 \times 10^4\,\text{N/C}
$$

---

$$
E_y = 3kq \frac{y}{r^3}
= 3(8.99 \times 10^9)(2 \times 10^{-6}) \frac{0.3}{0.0469}
$$

$$
E_y \approx 3.4 \times 10^5\,\text{N/C}
$$

---

### Result:

$$
\vec E \approx (-7.7 \times 10^4,\; 3.4 \times 10^5)\,\text{N/C}
$$

---

## 4. Limit $y \gg a$

When $y \gg a$, both charges appear as one:

Total charge:
$$
q_{\text{tot}} = 3q
$$

Field becomes:

$$
E \approx k \frac{3q}{y^2}
$$

Directed upward along $y$.

---

## Final Summary

- General field given by superposition formula  
- Zero field occurs between charges on x-axis  
- Numerical field:
$$
\vec E \approx (-7.7 \times 10^4,\; 3.4 \times 10^5)\,\text{N/C}
$$
- For $y \gg a$:
$$
E \approx k \frac{3q}{y^2}
$$