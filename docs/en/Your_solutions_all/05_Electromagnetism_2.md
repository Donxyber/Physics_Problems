# Section 5: Electromagnetism II

## 1. Gauss's Law

A point charge of $+2\ \text{C}$ is located at the origin. Calculate the electric flux through a spherical surface of radius $1\ \text{m}$ centered at the origin.

### Prepared presentation solution

By Gauss's law,

$$
\Phi_E = \frac{Q_{\text{enc}}}{\varepsilon_0}
$$

Here,

$$
Q_{\text{enc}} = 2\ \text{C}
$$

and

$$
\varepsilon_0 = 8.854\times 10^{-12}\ \text{F/m}
$$

So,

$$
\Phi_E = \frac{2}{8.854\times 10^{-12}}
\approx 2.26\times 10^{11}\ \text{N m}^2/\text{C}
$$

#### Final answer

$$
\Phi_E \approx 2.26\times 10^{11}\ \text{N m}^2/\text{C}
$$

The flux is **outward**, since the charge is positive.

---

## 2. Ampere's Law

Two long, parallel wires are $10\ \text{cm}$ apart and carry currents of $5\ \text{A}$ in opposite directions. Calculate the magnitude and direction of the magnetic field at a point midway between the wires.

### Prepared presentation solution

The midpoint is at a distance

$$
r=\frac{10\ \text{cm}}{2}=5\ \text{cm}=0.05\ \text{m}
$$

from each wire.

For one long straight wire,

$$
B=\frac{\mu_0 I}{2\pi r}
$$

with

$$
\mu_0 = 4\pi\times 10^{-7}\ \text{T m/A}
$$

So the field from one wire is

$$
B_1=\frac{(4\pi\times 10^{-7})(5)}{2\pi(0.05)}
=2\times 10^{-5}\ \text{T}
$$

Since the currents are in opposite directions, the magnetic fields at the midpoint point in the **same direction**, so they add:

$$
B_{\text{net}}=2B_1=4\times 10^{-5}\ \text{T}
$$

#### Direction

Using the right-hand rule, the magnetic field at the midpoint is perpendicular to the plane containing the two wires. Its exact sense depends on which wire carries current upward and which downward. For one standard orientation, the field is **into the page**.

#### Final answer

$$
B_{\text{net}}=4.0\times 10^{-5}\ \text{T}
$$

Direction: **into the page** for the standard orientation from the right-hand rule.

---

## 3. Biot-Savart Law

A small segment of a line wire of length $0.1\ \text{m}$ carries a current of $3\ \text{A}$. The segment is located at a distance of $0.2\ \text{m}$ from a point $P$. Calculate the magnetic field at point $P$ due to this current segment (assume the segment is perpendicular to the line connecting it to point $P$).

### Prepared presentation solution

For a small current element, the Biot-Savart law gives

$$
dB=\frac{\mu_0}{4\pi}\frac{I\,dl\,\sin\theta}{r^2}
$$

Since the segment is perpendicular to the line joining it to point $P$,

$$
\theta=90^\circ,\qquad \sin\theta=1
$$

Substitute:

$$
dB=\frac{10^{-7}(3)(0.1)}{(0.2)^2}
$$

$$
dB=\frac{3\times 10^{-8}}{0.04}=7.5\times 10^{-7}\ \text{T}
$$

#### Final answer

$$
B \approx 7.5\times 10^{-7}\ \text{T}
$$

Direction: given by the **right-hand rule** around the current element.

---

## 4. Magnetic Torque

A rectangular loop of wire with dimensions $10\ \text{cm}$ by $5\ \text{cm}$ carries a current of $2\ \text{A}$. A uniform magnetic field of $B = 0.3\ \text{T}$ is applied parallel to the plane of the loop. What is the magnitude of the magnetic torque on the loop?

### Prepared presentation solution

The torque on a current loop is

$$
\tau = N I A B \sin\theta
$$

For a single loop,

$$
N=1
$$

The area is

$$
A=(0.10)(0.05)=0.005\ \text{m}^2
$$

If the magnetic field is parallel to the plane of the loop, then it is perpendicular to the loop's area vector, so

$$
\theta=90^\circ,\qquad \sin\theta=1
$$

Thus,

$$
\tau=(1)(2)(0.005)(0.3)=0.003\ \text{N m}
$$

#### Final answer

$$
\tau = 3.0\times 10^{-3}\ \text{N m}
$$

---

## 5. Energy Stored by charge in a capacitor

We have a parallel-plate capacitor with the following parameters:

- $S = 0.02\,\mathrm{m^2}$
- $d = 5\,\mathrm{mm} = 0.005\,\mathrm{m}$
- $U = 500\,\mathrm{V}$

1. Calculate the capacitance $C$ of the capacitor.
2. Calculate the energy stored in the capacitor.
3. Calculate the electric field intensity $E$ between the plates.
4. Calculate the force of attraction $F$ between the plates.

### Prepared presentation solution

#### 1. Capacitance

For a parallel-plate capacitor,

$$
C=\varepsilon_0\frac{S}{d}
$$

Substitute:

$$
C=8.854\times 10^{-12}\cdot \frac{0.02}{0.005}
=8.854\times 10^{-12}\cdot 4
$$

$$
C=3.54\times 10^{-11}\ \text{F}
$$

#### 2. Energy stored

To avoid confusion with the voltage symbol $U$, let the stored energy be denoted by $W$.

$$
W=\frac{1}{2}CU^2
$$

So,

$$
W=\frac{1}{2}(3.54\times 10^{-11})(500)^2
$$

$$
W\approx 4.43\times 10^{-6}\ \text{J}
$$

#### 3. Electric field intensity

For a uniform field between the plates,

$$
E=\frac{U}{d}=\frac{500}{0.005}=1.0\times 10^5\ \text{V/m}
$$

#### 4. Force of attraction

Use the energy-density form of pressure:

$$
p=\frac{1}{2}\varepsilon_0 E^2
$$

Then

$$
F=pS=\frac{1}{2}\varepsilon_0 E^2 S
$$

Substitute:

$$
F=\frac{1}{2}(8.854\times 10^{-12})(1.0\times 10^5)^2(0.02)
$$

$$
F\approx 8.85\times 10^{-4}\ \text{N}
$$

#### Final answers

$$
C=3.54\times 10^{-11}\ \text{F}
$$

$$
W\approx 4.43\times 10^{-6}\ \text{J}
$$

$$
E=1.0\times 10^5\ \text{V/m}
$$

$$
F\approx 8.85\times 10^{-4}\ \text{N}
$$

---

## 6. EM Wave Analysis

An electromagnetic wave has its electric field component described by

$$
E_y(x,t) = 100 \sin(10^7 x - \omega t)\ \text{V/m}
$$

What is the direction of propagation? What is the wavelength $\lambda$? What is the angular frequency $\omega$? What is the equation for the magnetic field component?

### Prepared presentation solution

The standard form of a wave traveling in the positive $x$ direction is

$$
\sin(kx-\omega t)
$$

So this wave propagates in the **positive $x$ direction**.

From the equation,

$$
k=10^7\ \text{rad/m}
$$

#### Wavelength

$$
\lambda=\frac{2\pi}{k}=\frac{2\pi}{10^7}
\approx 6.28\times 10^{-7}\ \text{m}
$$

So,

$$
\lambda \approx 628\ \text{nm}
$$

#### Angular frequency

For an EM wave in vacuum,

$$
\omega=ck
$$

with

$$
c=3.0\times 10^8\ \text{m/s}
$$

Thus,

$$
\omega=(3.0\times 10^8)(10^7)=3.0\times 10^{15}\ \text{rad/s}
$$

#### Magnetic field component

For an electromagnetic wave,

$$
B_0=\frac{E_0}{c}=\frac{100}{3.0\times 10^8}
=3.33\times 10^{-7}\ \text{T}
$$

If the electric field is in the $y$ direction and the wave propagates in the $+x$ direction, then the magnetic field must point in the $z$ direction so that

$$
\vec E \times \vec B
$$

points along $+x$.

Therefore,

$$
B_z(x,t)=3.33\times 10^{-7}\sin(10^7x-\omega t)\ \text{T}
$$

#### Final answers

- Direction of propagation: **positive $x$ direction**
- Wavelength:

$$
\lambda \approx 6.28\times 10^{-7}\ \text{m} = 628\ \text{nm}
$$

- Angular frequency:

$$
\omega = 3.0\times 10^{15}\ \text{rad/s}
$$

- Magnetic field:

$$
B_z(x,t)=3.33\times 10^{-7}\sin(10^7x-\omega t)\ \text{T}
$$

---

## 7. Wavelength and Frequency

The human eye is most sensitive to light with a wavelength of about $550\ \text{nm}$. What color does this correspond to in the visible spectrum? What is the frequency of this light?

### Prepared presentation solution

A wavelength of

$$
550\ \text{nm}=5.50\times 10^{-7}\ \text{m}
$$

corresponds approximately to **green light**.

The frequency is

$$
f=\frac{c}{\lambda}
$$

So,

$$
f=\frac{3.0\times 10^8}{5.50\times 10^{-7}}
\approx 5.45\times 10^{14}\ \text{Hz}
$$

#### Final answers

- Color: **green**
- Frequency:

$$
f\approx 5.45\times 10^{14}\ \text{Hz}
$$

---

## 8. EM Spectrum

List the following types of electromagnetic radiation in order of increasing wavelength: Infrared, Ultraviolet, Microwaves, X-rays, Radio waves, Gamma rays.

### Prepared presentation solution

From **shortest wavelength** to **longest wavelength**:

1. Gamma rays
2. X-rays
3. Ultraviolet
4. Infrared
5. Microwaves
6. Radio waves

#### Final answer

$$
\text{Gamma rays} < \text{X-rays} < \text{Ultraviolet} < \text{Infrared} < \text{Microwaves} < \text{Radio waves}
$$

---

## 9. Refraction (Snell's Law)

A light ray travels from air ($n=1.00$) into glass ($n=1.50$). If the angle of incidence is $30^\circ$, what is the angle of refraction?

### Prepared presentation solution

Use Snell's law:

$$
n_1\sin\theta_1=n_2\sin\theta_2
$$

Substitute:

$$
1.00\sin 30^\circ = 1.50\sin\theta_2
$$

Since

$$
\sin 30^\circ = 0.5
$$

we get

$$
0.5 = 1.5\sin\theta_2
$$

Thus,

$$
\sin\theta_2 = \frac{0.5}{1.5}=\frac{1}{3}
$$

So,

$$
\theta_2=\sin^{-1}\left(\frac{1}{3}\right)\approx 19.5^\circ
$$

#### Final answer

$$
\theta_2 \approx 19.5^\circ
$$

The ray bends **toward the normal**, because it enters a medium with higher refractive index.

---

## 10. Speed of Light in Media

What is the speed of light in a diamond, which has an index of refraction $n = 2.42$?

### Prepared presentation solution

The speed of light in a medium is

$$
v=\frac{c}{n}
$$

Substitute:

$$
v=\frac{3.0\times 10^8}{2.42}
\approx 1.24\times 10^8\ \text{m/s}
$$

#### Final answer

$$
v \approx 1.24\times 10^8\ \text{m/s}
$$
