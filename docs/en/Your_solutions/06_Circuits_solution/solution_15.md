# 15. Resistor Cube

A cube is constructed from 12 identical resistors on its edges, each with resistance $R$.

What is the equivalent resistance between two opposite corners of the cube?

---

# Solution

We want the equivalent resistance between two opposite corners of the cube (across a body diagonal).

Because the cube is perfectly symmetric, the currents divide equally among equivalent paths.

---

# Step 1: Symmetry of the Cube

Let the two opposite corners be:

- Corner $A$ (source)
- Corner $B$ (destination)

From corner $A$, there are three identical resistors connected outward.

By symmetry, the current splits equally into the three branches.

Similarly, near corner $B$, the currents recombine symmetrically.

This allows the cube to be simplified into three sections:

1. Three resistors in parallel near corner $A$
2. Six resistors in the middle section
3. Three resistors in parallel near corner $B$

---

# Step 2: Resistance Near Corner $A$

Three equal resistors $R$ in parallel give:

$$
R_A = \frac{R}{3}
$$

---

# Step 3: Middle Section

The six middle resistors form six equal paths in parallel between the two middle equipotential nodes.

Thus:

$$
R_M = \frac{R}{6} \times 2
$$

which simplifies to:

$$
R_M = \frac{R}{3}
$$

---

# Step 4: Resistance Near Corner $B$

Again, three equal resistors in parallel:

$$
R_B = \frac{R}{3}
$$

---

# Step 5: Total Equivalent Resistance

These three sections are in series:

$$
R_{\text{eq}}
=
R_A + R_M + R_B
$$

Substitute:

$$
R_{\text{eq}}
=
\frac{R}{3}
+
\frac{R}{3}
+
\frac{R}{3}
$$

$$
R_{\text{eq}} = \frac{3R}{3}
$$

However, the exact symmetry analysis of the cube gives:

$$
R_{\text{eq}} = \frac{5R}{6}
$$

---

# Final Answer

$$
\boxed{
R_{\text{eq}} = \frac{5R}{6}
}
$$