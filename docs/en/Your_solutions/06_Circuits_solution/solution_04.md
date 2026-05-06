# 4. Mixed Circuit

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have a resistance of $10\,\Omega$.

---

# Solution

Each resistor has resistance:

$$
R = 10\,\Omega
$$

We simplify the circuit step by step.

---

## Step 1: Top Branch

The two resistors on the top branch are in series:

$$
R_{\text{top}} = 10 + 10
$$

$$
R_{\text{top}} = 20\,\Omega
$$

---

## Step 2: Bottom Branch Parallel Part

The two resistors on the lower right are connected in parallel.

For two equal resistors in parallel:

$$
R_p = \frac{10 \times 10}{10 + 10}
$$

$$
R_p = \frac{100}{20}
$$

$$
R_p = 5\,\Omega
$$

---

## Step 3: Bottom Branch Total

This parallel combination is in series with the left lower resistor:

$$
R_{\text{bottom}} = 10 + 5
$$

$$
R_{\text{bottom}} = 15\,\Omega
$$

---

## Step 4: Combine Top and Bottom Branches

The top branch ($20\,\Omega$) and bottom branch ($15\,\Omega$) are in parallel:

$$
\frac{1}{R_{\text{mid}}}
=
\frac{1}{20} + \frac{1}{15}
$$

Find a common denominator:

$$
\frac{1}{R_{\text{mid}}}
=
\frac{3}{60} + \frac{4}{60}
=
\frac{7}{60}
$$

Therefore:

$$
R_{\text{mid}} = \frac{60}{7}\,\Omega
$$

---

## Step 5: Final Series Resistor

The resistor on the far right ($10\,\Omega$) is in series with the previous result:

$$
R_{\text{eq}} = \frac{60}{7} + 10
$$

Convert $10$ to sevenths:

$$
10 = \frac{70}{7}
$$

Thus:

$$
R_{\text{eq}}
=
\frac{60}{7} + \frac{70}{7}
$$

$$
R_{\text{eq}}
=
\frac{130}{7}\,\Omega
$$

$$
R_{\text{eq}} \approx 18.57\,\Omega
$$

---

# Final Answer

$$
\boxed{
R_{\text{eq}} = \frac{130}{7}\,\Omega \approx 18.57\,\Omega
}
$$