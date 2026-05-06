# 2. Resistors

You have a supply of exactly three $1\,\Omega$ resistors. What are all the possible equivalent resistances you can create by combining them? List all unique values.

---

# Solution

Using three identical $1\,\Omega$ resistors, we can connect them in different series and parallel combinations.

---

## 1. All Resistors in Series

For resistors in series:

$$
R_{\text{eq}} = 1 + 1 + 1
$$

$$
R_{\text{eq}} = 3\,\Omega
$$

---

## 2. All Resistors in Parallel

For resistors in parallel:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{1} + \frac{1}{1} + \frac{1}{1}
$$

$$
\frac{1}{R_{\text{eq}}} = 3
$$

$$
R_{\text{eq}} = \frac{1}{3}\,\Omega
$$

---

## 3. Two in Series, Then Parallel with One

First combine two resistors in series:

$$
R = 1 + 1 = 2\,\Omega
$$

Now place this in parallel with the third resistor:

$$
\frac{1}{R_{\text{eq}}}
=
\frac{1}{2} + \frac{1}{1}
$$

$$
\frac{1}{R_{\text{eq}}}
=
\frac{3}{2}
$$

$$
R_{\text{eq}} = \frac{2}{3}\,\Omega
$$

---

## 4. Two in Parallel, Then Series with One

First combine two resistors in parallel:

$$
\frac{1}{R}
=
\frac{1}{1} + \frac{1}{1}
$$

$$
\frac{1}{R} = 2
$$

$$
R = \frac{1}{2}\,\Omega
$$

Now place this in series with the third resistor:

$$
R_{\text{eq}} = \frac{1}{2} + 1
$$

$$
R_{\text{eq}} = \frac{3}{2}\,\Omega
$$

---

# Final Answer

The unique equivalent resistances possible are:

$$
\boxed{
\frac{1}{3}\,\Omega,\;
\frac{2}{3}\,\Omega,\;
\frac{3}{2}\,\Omega,\;
3\,\Omega
}
$$