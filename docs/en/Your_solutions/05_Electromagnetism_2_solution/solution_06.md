## 6. EM Wave Analysis — Solution

Given:
$$
E_y(x,t) = 100 \sin(10^7 x - \omega t)
$$

---

## 1. Direction of Propagation

A wave of the form:
$$
\sin(kx - \omega t)
$$
propagates in the **+x direction**.

---

## 2. Wave Number and Wavelength

Wave number:
$$
k = 10^7 \,\text{rad/m}
$$

Relation:
$$
k = \frac{2\pi}{\lambda}
$$

So:
$$
\lambda = \frac{2\pi}{k}
= \frac{2\pi}{10^7}
$$

$$
\lambda \approx 6.28 \times 10^{-7}\,\text{m}
$$

---

## 3. Angular Frequency

For EM waves:
$$
c = \frac{\omega}{k}
\Rightarrow \omega = ck
$$

Using $c = 3 \times 10^8\,\text{m/s}$:

$$
\omega = (3 \times 10^8)(10^7)
= 3 \times 10^{15}\,\text{rad/s}
$$

---

## 4. Magnetic Field Component

For electromagnetic waves:
$$
B = \frac{E}{c}
$$

Amplitude:
$$
B_0 = \frac{100}{3 \times 10^8}
\approx 3.33 \times 10^{-7}\,\text{T}
$$

Since $\vec E$ is along $\hat y$ and propagation is along $\hat x$,  
$\vec B$ is along $\hat z$.

---

## Final Magnetic Field

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15} t)
$$

---

## Final Answers

- Direction: $\boxed{+\hat x}$
- Wavelength: $\boxed{6.28 \times 10^{-7}\,\text{m}}$
- Angular frequency: $\boxed{3 \times 10^{15}\,\text{rad/s}}$
- Magnetic field:
$$
\boxed{
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15} t)
}
$$