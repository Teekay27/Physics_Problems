# 14. RLC Circuit

Write down the differential equation for a series RLC circuit with a voltage source $V$, a resistor $R$, an inductor $L$, and a capacitor $C$.

Assume the current is $I(t)$ and the voltage across the capacitor is $V_C(t)$.

Compare this to the equation of a damped harmonic oscillator. What are the analogies between the terms in the two equations?

---

# Solution

## Step 1: Apply Kirchhoff’s Voltage Law

For a series RLC circuit, the sum of the voltage drops equals the applied voltage:

$$
V(t) = V_R + V_L + V_C
$$

The voltage across each element is:

### Resistor

$$
V_R = RI
$$

### Inductor

$$
V_L = L\frac{dI}{dt}
$$

### Capacitor

$$
V_C = \frac{1}{C}\int I\,dt
$$

Substitute into Kirchhoff’s law:

$$
V(t) = RI + L\frac{dI}{dt} + \frac{1}{C}\int I\,dt
$$

---

# Step 2: Differential Equation in Terms of Current

Differentiate both sides with respect to time:

$$
\frac{dV}{dt}
=
R\frac{dI}{dt}
+
L\frac{d^2 I}{dt^2}
+
\frac{1}{C}I
$$

Rearrange:

$$
L\frac{d^2 I}{dt^2}
+
R\frac{dI}{dt}
+
\frac{1}{C}I
=
\frac{dV}{dt}
$$

This is the differential equation for the series RLC circuit.

---

# Special Case: No External Source

If there is no applied voltage after the circuit is started:

$$
V(t)=0
$$

then:

$$
L\frac{d^2 I}{dt^2}
+
R\frac{dI}{dt}
+
\frac{1}{C}I
=
0
$$

---

# Step 3: Compare with the Damped Harmonic Oscillator

The equation for a damped harmonic oscillator is:

$$
m\frac{d^2 x}{dt^2}
+
b\frac{dx}{dt}
+
kx
=
0
$$

where:

- $m$ = mass
- $b$ = damping coefficient
- $k$ = spring constant
- $x(t)$ = displacement

---

# Analogies Between the Two Equations

| Mechanical Oscillator | RLC Circuit |
|---|---|
| Displacement $x$ | Current $I$ |
| Mass $m$ | Inductance $L$ |
| Damping coefficient $b$ | Resistance $R$ |
| Spring constant $k$ | $\frac{1}{C}$ |
| Inertia of mass | Magnetic energy in inductor |
| Frictional damping | Resistive energy loss |
| Spring restoring force | Capacitor restoring effect |

---

# Interpretation

- The **inductor** behaves like **mass**, resisting changes in current.
- The **resistor** behaves like **friction**, dissipating energy.
- The **capacitor** behaves like a **spring**, storing energy and providing a restoring effect.

Thus, a series RLC circuit mathematically behaves exactly like a damped harmonic oscillator.

---

# Final Differential Equation

$$
\boxed{
L\frac{d^2 I}{dt^2}
+
R\frac{dI}{dt}
+
\frac{1}{C}I
=
\frac{dV}{dt}
}
$$

For the unforced case:

$$
\boxed{
L\frac{d^2 I}{dt^2}
+
R\frac{dI}{dt}
+
\frac{1}{C}I
=
0
}
$$