# 6. Kirchhoff's Laws Again

Calculate the current flowing through the ammeter.

---

# Given

- Source $\mathcal{E}_1 = 9\,\text{V}$ with internal resistance $r_1 = 1\,\Omega$
- Source $\mathcal{E}_2 = 4.5\,\text{V}$ with internal resistance $r_2 = 1\,\Omega$
- Resistor $R_1 = 10\,\Omega$
- Resistor $R_2 = 20\,\Omega$

The ammeter is in the branch containing $R_2$.

---

# Step 1: Define Mesh Currents

Let:

- $I_1$ = current in the outer loop
- $I_2$ = current in the upper loop (through the ammeter and $R_2$)

The resistor $R_1$ belongs only to the outer loop.

---

# Step 2: Apply Kirchhoff’s Voltage Law

## Outer Loop

Traversing the outer loop:

$$
-9 + 1I_1 + 10I_1 + 20(I_1 - I_2) = 0
$$

Simplify:

$$
-9 + 11I_1 + 20I_1 - 20I_2 = 0
$$

$$
31I_1 - 20I_2 = 9
$$

---

## Upper Loop

Traversing the upper loop:

$$
-4.5 + 1I_2 + 20(I_2 - I_1) = 0
$$

Simplify:

$$
-4.5 + I_2 + 20I_2 - 20I_1 = 0
$$

$$
-20I_1 + 21I_2 = 4.5
$$

---

# Step 3: Solve the Equations

We now solve:

$$
31I_1 - 20I_2 = 9
$$

$$
-20I_1 + 21I_2 = 4.5
$$

Multiply the first equation by $21$:

$$
651I_1 - 420I_2 = 189
$$

Multiply the second equation by $20$:

$$
-400I_1 + 420I_2 = 90
$$

Add the equations:

$$
251I_1 = 279
$$

$$
I_1 = \frac{279}{251}
$$

$$
I_1 \approx 1.11\,\text{A}
$$

Substitute into:

$$
-20(1.11) + 21I_2 = 4.5
$$

$$
-22.2 + 21I_2 = 4.5
$$

$$
21I_2 = 26.7
$$

$$
I_2 \approx 1.27\,\text{A}
$$

---

# Step 4: Ammeter Current

The ammeter measures the current in the upper branch:

$$
I_A = I_2
$$

Therefore:

$$
\boxed{
I_A \approx 1.27\,\text{A}
}
$$

---

# Final Answer

$$
\boxed{
1.27\,\text{A}
}
$$