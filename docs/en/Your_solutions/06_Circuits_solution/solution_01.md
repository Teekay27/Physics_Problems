# 1. Series and Parallel Circuit

You have three resistors,  
$R_1 = 15\,\Omega$, $R_2 = 30\,\Omega$, and $R_3 = 50\,\Omega$ and a 12 V battery.

Consider the case when they are all connected in **series** and when all of them are connected in **parallel**.

Calculate:

1. The total equivalent resistance in each case.  
2. The current flowing from the battery in each case.

---

# Solution

## A. Series Connection

In a series circuit, resistances add directly:

$$
R_{\text{eq}} = R_1 + R_2 + R_3
$$

$$
R_{\text{eq}} = 15 + 30 + 50
$$

$$
R_{\text{eq}} = 95\,\Omega
$$

Using Ohm’s Law:

$$
I = \frac{V}{R}
$$

$$
I = \frac{12}{95}
$$

$$
I \approx 0.126\text{ A}
$$

### Answers for Series Circuit

- Equivalent Resistance:

$$
\boxed{95\,\Omega}
$$

- Current from the battery:

$$
\boxed{0.126\text{ A}}
$$

---

## B. Parallel Connection

For resistors in parallel:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}
$$

Substitute the values:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{15} + \frac{1}{30} + \frac{1}{50}
$$

Find a common denominator:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{10}{150} + \frac{5}{150} + \frac{3}{150}
$$

$$
\frac{1}{R_{\text{eq}}}
=
\frac{18}{150}
$$

$$
\frac{1}{R_{\text{eq}}}
=
0.12
$$

$$
R_{\text{eq}} = \frac{1}{0.12}
$$

$$
R_{\text{eq}} \approx 8.33\,\Omega
$$

Now calculate the current:

$$
I = \frac{V}{R}
$$

$$
I = \frac{12}{8.33}
$$

$$
I \approx 1.44\text{ A}
$$

### Answers for Parallel Circuit

- Equivalent Resistance:

$$
\boxed{8.33\,\Omega}
$$

- Current from the battery:

$$
\boxed{1.44\text{ A}}
$$

---

# Final Answers Summary

| Circuit Type | Equivalent Resistance | Current |
|---|---|---|
| Series | $95\,\Omega$ | $0.126\,\text{A}$ |
| Parallel | $8.33\,\Omega$ | $1.44\,\text{A}$ |