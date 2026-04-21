## 3. Superposition Principle

### Problem

Two waves are given by:

$$
y_1(x, t) = A \sin(kx - \omega t)
$$

$$
y_2(x, t) = A \sin(kx + \omega t)
$$

Find:
1. The equation of the resulting **standing wave**  
2. The positions of the **nodes**

---

### Solution

We use the trigonometric identity:

$$
\sin(a) + \sin(b) = 2 \sin\left(\frac{a + b}{2}\right)\cos\left(\frac{a - b}{2}\right)
$$

Let:

$$
a = kx - \omega t, \quad b = kx + \omega t
$$

---

### Step 1: Add the Waves

$$
y(x, t) = y_1 + y_2
$$

$$
y(x, t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)
$$

$$
y(x, t) = 2A \sin(kx)\cos(\omega t)
$$

---

### ✅ Standing Wave Equation

$$
y(x, t) = 2A \sin(kx)\cos(\omega t)
$$

---

### Step 2: Find Nodes

Nodes occur where displacement is always zero:

$$
\sin(kx) = 0
$$

$$
kx = n\pi
$$

Solve for $x$:

$$
x = \frac{n\pi}{k}
$$

Using:

$$
k = \frac{2\pi}{\lambda}
$$

we get:

$$
x = \frac{n\lambda}{2}
$$

---

### ✅ Final Answer

- Standing wave:
  
  $$
  y(x, t) = 2A \sin(kx)\cos(\omega t)
  $$

- Nodes at:
  
  $$
  x = \frac{n\lambda}{2}, \quad n = 0, 1, 2, 3, \dots
  $$
