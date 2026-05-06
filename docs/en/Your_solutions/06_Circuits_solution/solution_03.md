# 3. Mixed Circuit

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have a resistance of $5\,\Omega$.

---

# Solution

Each resistor has resistance:

$$
R = 5\,\Omega
$$

We simplify the circuit step by step.

---

## Step 1: Left Upper Branch

The left vertical resistor and the top horizontal resistor are in series:

$$
R_1 = 5 + 5
$$

$$
R_1 = 10\,\Omega
$$

---

## Step 2: Middle Branch

The two vertical middle resistors are in series:

$$
5 + 5 = 10\,\Omega
$$

This combination is also in series with the lower horizontal resistor:

$$
R_2 = 10 + 5
$$

$$
R_2 = 15\,\Omega
$$

---

## Step 3: Parallel Combination

The two branches between the same nodes are now:

- $10\,\Omega$
- $15\,\Omega$

So they are in parallel:

$$
\frac{1}{R_p}
=
\frac{1}{10} + \frac{1}{15}
$$

Find a common denominator:

$$
\frac{1}{R_p}
=
\frac{3}{30} + \frac{2}{30}
=
\frac{5}{30}
=
\frac{1}{6}
$$

Therefore:

$$
R_p = 6\,\Omega
$$

---

## Step 4: Right Branch

The two resistors on the right side are in series:

$$
R_3 = 5 + 5
$$

$$
R_3 = 10\,\Omega
$$

This is in series with the previous equivalent resistance:

$$
R_{\text{top}} = 6 + 10
$$

$$
R_{\text{top}} = 16\,\Omega
$$

---

## Step 5: Final Parallel Combination

The bottom resistor of $5\,\Omega$ is in parallel with the entire top branch of $16\,\Omega$.

Thus:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{5} + \frac{1}{16}
$$

$$
\frac{1}{R_{\text{eq}}}
=
\frac{16}{80} + \frac{5}{80}
=
\frac{21}{80}
$$

Therefore:

$$
R_{\text{eq}}
=
\frac{80}{21}\,\Omega
$$

$$
R_{\text{eq}}
\approx 3.81\,\Omega
$$

---

# Final Answer

$$
\boxed{
R_{\text{eq}} = \frac{80}{21}\,\Omega \approx 3.81\,\Omega
}
$$