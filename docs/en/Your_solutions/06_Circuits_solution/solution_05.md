# 5. Kirchhoff's Laws

Using Kirchhoff’s laws, find the currents $I_1$, $I_2$, and $I_3$ (going through the resistors $R_1$, $R_2$, and the right branch respectively) in the following two-loop circuit.

Given:

- Left loop:
  - $R_1 = 20\,\Omega$
  - $\mathcal{E}_1 = 4.5\,\text{V}$
  - internal resistance $r_1 = 1\,\Omega$

- Right loop:
  - $\mathcal{E}_2 = 9\,\text{V}$
  - internal resistance $r_2 = 1\,\Omega$

- Shared branch:
  - $R_2 = 10\,\Omega$

---

# Solution

Let:

- $I_1$ = current in the left loop
- $I_3$ = current in the right loop
- $I_2$ = current through the shared resistor $R_2$

At the junction:

$$
I_2 = I_1 + I_3
$$

---

# Step 1: Left Loop Equation

Applying Kirchhoff’s Voltage Law (KVL) to the left loop:

The resistances in this loop are:

$$
R_1 + r_1 + R_2 = 20 + 1 + 10
$$

$$
= 31\,\Omega
$$

Voltage equation:

$$
20I_1 + 1I_1 + 10(I_1 + I_3) = 4.5
$$

Simplify:

$$
21I_1 + 10I_1 + 10I_3 = 4.5
$$

$$
31I_1 + 10I_3 = 4.5
$$

---

# Step 2: Right Loop Equation

Applying KVL to the right loop:

$$
1I_3 + 10(I_1 + I_3) = 9
$$

Simplify:

$$
10I_1 + 11I_3 = 9
$$

---

# Step 3: Solve the System

We now solve:

$$
31I_1 + 10I_3 = 4.5
$$

$$
10I_1 + 11I_3 = 9
$$

Multiply the second equation by $31$:

$$
310I_1 + 341I_3 = 279
$$

Multiply the first equation by $10$:

$$
310I_1 + 100I_3 = 45
$$

Subtract:

$$
241I_3 = 234
$$

$$
I_3 = \frac{234}{241}
$$

$$
I_3 \approx 0.971\,\text{A}
$$

Now substitute into:

$$
10I_1 + 11(0.971) = 9
$$

$$
10I_1 + 10.681 = 9
$$

$$
10I_1 = -1.681
$$

$$
I_1 \approx -0.168\,\text{A}
$$

The negative sign means the actual current direction is opposite to the assumed direction.

Now calculate $I_2$:

$$
I_2 = I_1 + I_3
$$

$$
I_2 = -0.168 + 0.971
$$

$$
I_2 \approx 0.803\,\text{A}
$$

---

# Final Answers

$$
\boxed{
I_1 \approx -0.168\,\text{A}
}
$$

(Current flows opposite to the assumed direction.)

$$
\boxed{
I_2 \approx 0.803\,\text{A}
}
$$

$$
\boxed{
I_3 \approx 0.971\,\text{A}
}
$$