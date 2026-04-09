# Section 2: Mechanics II

## 1. Gravitational Dependence

A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's?

What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?

### Prepared presentation solution

For a simple pendulum,
\[
T = 2\pi \sqrt{\frac{L}{g}}.
\]

#### Period on the Moon
If the pendulum length is unchanged, then
\[
T \propto \frac{1}{\sqrt{g}}.
\]
Since
\[
g_{\text{Moon}}=\frac{g_{\text{Earth}}}{6},
\]
we get
\[
T_{\text{Moon}} = T_{\text{Earth}}\sqrt{\frac{g_{\text{Earth}}}{g_{\text{Moon}}}}
= 4\sqrt{6}.
\]
Numerically,
\[
T_{\text{Moon}} \approx 4 \cdot 2.449 = 9.80\ \text{s}.
\]

#### Length for a 1-second pendulum on Earth
From
\[
T = 2\pi \sqrt{\frac{L}{g}},
\]
solve for \(L\):
\[
L = g\left(\frac{T}{2\pi}\right)^2.
\]
For \(T=1\ \text{s}\) and \(g=9.81\ \text{m/s}^2\),
\[
L = 9.81\left(\frac{1}{2\pi}\right)^2 \approx 0.248\ \text{m}.
\]

#### Final answers
- Period on the Moon:
\[
\boxed{T_{\text{Moon}} \approx 9.80\ \text{s}}
\]
- Required length for \(T=1\ \text{s}\) on Earth:
\[
\boxed{L \approx 0.248\ \text{m}}
\]

---

## 2. Harmonic Motion

A 10 kg mass is attached to a spring and oscillates according to the equation
\[
x(t) = 0.2 \cos(10\pi t)
\]
(in meters). What is the spring constant \(k\)? What is the total mechanical energy of the system?

### Prepared presentation solution

The standard form of simple harmonic motion is
\[
x(t)=A\cos(\omega t+\phi).
\]
By comparison:
- Amplitude:
\[
A=0.2\ \text{m}
\]
- Angular frequency:
\[
\omega=10\pi\ \text{rad/s}
\]
- Mass:
\[
m=10\ \text{kg}
\]

#### Spring constant
For a spring-mass system,
\[
\omega=\sqrt{\frac{k}{m}}.
\]
Hence,
\[
k=m\omega^2=10(10\pi)^2=1000\pi^2\ \text{N/m}.
\]
Numerically,
\[
k \approx 9869.6\ \text{N/m}.
\]

#### Total mechanical energy
For SHM,
\[
E=\frac{1}{2}kA^2.
\]
Thus,
\[
E=\frac{1}{2}(1000\pi^2)(0.2)^2
=20\pi^2\ \text{J}.
\]
Numerically,
\[
E \approx 197.4\ \text{J}.
\]

#### Final answers
\[
\boxed{k=1000\pi^2\ \text{N/m}\approx 9869.6\ \text{N/m}}
\]
\[
\boxed{E=20\pi^2\ \text{J}\approx 197.4\ \text{J}}
\]

---

## 3. Conservation of Energy

A pendulum with a length of 1.0 meter is released from an initial angle of \(15^\circ\). What is the speed of the pendulum bob at the bottom of its swing?

### Prepared presentation solution

Use conservation of mechanical energy.

The bob drops by a vertical height
\[
h=L(1-\cos\theta).
\]
With \(L=1.0\ \text{m}\) and \(\theta=15^\circ\),
\[
h=1(1-\cos 15^\circ).
\]

Potential energy at release becomes kinetic energy at the bottom:
\[
mgh=\frac{1}{2}mv^2.
\]
Mass cancels:
\[
v=\sqrt{2gh}.
\]
Substitute:
\[
v=\sqrt{2gL(1-\cos 15^\circ)}.
\]
Using \(g=9.81\ \text{m/s}^2\),
\[
v=\sqrt{2(9.81)(1)(1-\cos 15^\circ)} \approx 0.90\ \text{m/s}.
\]

#### Final answer
\[
\boxed{v \approx 0.90\ \text{m/s}}
\]

---

## 4. Energy & Momentum

A 0.5 kg block slides down a frictionless track from a height of 3.0 m. At the bottom, it collides and sticks to a 1.5 kg block, which is initially at rest. What is the speed of the combined mass just after the collision?

### Prepared presentation solution

#### Step 1: Speed before the collision
Since the track is frictionless, mechanical energy is conserved:
\[
mgh=\frac{1}{2}mv^2.
\]
Thus,
\[
v=\sqrt{2gh}=\sqrt{2(9.81)(3.0)}\approx 7.67\ \text{m/s}.
\]

#### Step 2: Use momentum conservation for the sticking collision
Let:
- \(m_1=0.5\ \text{kg}\),
- \(m_2=1.5\ \text{kg}\),
- \(v_1=7.67\ \text{m/s}\),
- \(v_2=0\).

Since the blocks stick together,
\[
m_1v_1+m_2v_2=(m_1+m_2)v_f.
\]
So,
\[
v_f=\frac{m_1v_1}{m_1+m_2}
=\frac{0.5\cdot 7.67}{2.0}
\approx 1.92\ \text{m/s}.
\]

#### Final answer
\[
\boxed{v_f \approx 1.92\ \text{m/s}}
\]

---

## 5. Inelastic Collision

A 70 kg runner moving at \(3 \text{ m/s}\) jumps onto a 140 kg stationary cart. What is the final speed of the cart with the runner? Is kinetic energy conserved in this collision? Explain.

### Prepared presentation solution

This is a perfectly inelastic collision, so momentum is conserved.

#### Final speed
Initial momentum:
\[
p_i = (70)(3) + (140)(0) = 210\ \text{kg m/s}.
\]
Total mass after collision:
\[
m_{\text{total}}=70+140=210\ \text{kg}.
\]
Therefore,
\[
v_f=\frac{210}{210}=1.0\ \text{m/s}.
\]

#### Is kinetic energy conserved?
Initial kinetic energy:
\[
K_i=\frac{1}{2}(70)(3^2)=315\ \text{J}.
\]
Final kinetic energy:
\[
K_f=\frac{1}{2}(210)(1^2)=105\ \text{J}.
\]

Since
\[
K_f \ne K_i,
\]
kinetic energy is **not** conserved.

The missing kinetic energy is transformed into internal energy such as deformation, heat, and sound.

#### Final answers
\[
\boxed{v_f=1.0\ \text{m/s}}
\]
Kinetic energy is **not conserved**.

---

## 6. Energy Dissipation

A tennis ball is dropped from a height of \(2.0\) m. After each bounce, it loses 30% of its mechanical energy. To what height does it rise after the second bounce?

### Prepared presentation solution

The ball retains \(70\%\) of its mechanical energy after each bounce.

Since potential energy at the top is \(mgh\), height is proportional to mechanical energy.

#### After the first bounce
\[
h_1=0.7\times 2.0=1.4\ \text{m}.
\]

#### After the second bounce
\[
h_2=0.7\times 1.4=0.98\ \text{m}.
\]

#### Final answer
\[
\boxed{h_2=0.98\ \text{m}}
\]

---

## 7. Dynamics with Friction

A 5 kg block is placed on a 10 kg block. A horizontal force of 45 N is applied to the 10 kg block, and the 5 kg block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is 0.2. Find the acceleration of the 10 kg block.

### Prepared presentation solution

The 10 kg block moves to the right. Since the 5 kg block is tied to the wall, the lower block slides beneath it. Therefore there are two friction forces opposing the motion of the 10 kg block:

1. Friction from the upper 5 kg block
2. Friction from the ground

Take \(g=9.81\ \text{m/s}^2\).

#### Friction between the two blocks
Normal force from the top block:
\[
N_1 = 5g = 49.05\ \text{N}.
\]
Kinetic friction:
\[
f_1 = \mu N_1 = 0.2(49.05)=9.81\ \text{N}.
\]

#### Friction between the lower block and the ground
The ground supports both masses:
\[
N_2 = (10+5)g = 15g = 147.15\ \text{N}.
\]
So,
\[
f_2 = \mu N_2 = 0.2(147.15)=29.43\ \text{N}.
\]

#### Net force on the 10 kg block
\[
F_{\text{net}}=45 - 9.81 - 29.43 = 5.76\ \text{N}.
\]

#### Acceleration
Only the 10 kg block accelerates, so
\[
a=\frac{F_{\text{net}}}{10}=\frac{5.76}{10}=0.576\ \text{m/s}^2.
\]

#### Final answer
\[
\boxed{a \approx 0.576\ \text{m/s}^2}
\]

---

## 8. Work of a variable force

Given a one-dimensional force:
\[
F(x)=-kx
\]

* Write down the equation of motion and solve it.
* Calculate the work done during the displacement from \(0\) to \(x_0\).
* Interpret the result as potential energy.
* Verify the relationship \(F = -\frac{dU}{dx}\).
* Draw the graph of \(F(x)\) and \(U(x)\).

### Prepared presentation solution

#### Equation of motion
From Newton's second law:
\[
m\ddot x = -kx.
\]
Rearrange:
\[
\ddot x + \frac{k}{m}x=0.
\]
Define
\[
\omega=\sqrt{\frac{k}{m}}.
\]
The general solution is
\[
x(t)=A\cos(\omega t)+B\sin(\omega t),
\]
or equivalently
\[
x(t)=C\cos(\omega t+\phi).
\]

#### Work done from \(0\) to \(x_0\)
The work done by the force is
\[
W=\int_0^{x_0}F(x)\,dx = \int_0^{x_0}(-kx)\,dx.
\]
Hence,
\[
W=-k\left[\frac{x^2}{2}\right]_0^{x_0}
=-\frac{1}{2}kx_0^2.
\]

#### Interpretation as potential energy
For a conservative force,
\[
W = -\Delta U.
\]
If we set \(U(0)=0\), then
\[
U(x)=\frac{1}{2}kx^2.
\]

#### Verify \(F=-\frac{dU}{dx}\)
Differentiate:
\[
\frac{dU}{dx}=\frac{d}{dx}\left(\frac{1}{2}kx^2\right)=kx.
\]
Therefore,
\[
-\frac{dU}{dx}=-kx=F(x).
\]
Verified.

#### Graphs
- \(F(x)=-kx\): straight line through the origin with negative slope.
- \(U(x)=\frac{1}{2}kx^2\): upward-opening parabola with minimum at \(x=0\).

#### Final results
\[
\boxed{m\ddot x + kx = 0}
\]
\[
\boxed{x(t)=A\cos(\omega t)+B\sin(\omega t),\quad \omega=\sqrt{\frac{k}{m}}}
\]
\[
\boxed{W_{0\to x_0}=-\frac{1}{2}kx_0^2}
\]
\[
\boxed{U(x)=\frac{1}{2}kx^2}
\]

---

## 9. Vertical throw with drag

We have the equation of motion:
\[
m\frac{dv}{dt} = -mg - kv
\]
with initial conditions \(v(0)=v_0\), \(x(0)=10\).

* Solve the equation by analytical methods.
* Determine the maximum height.
* Compare with the case without drag.
* Perform a numerical simulation using HTML or Python.

### Prepared presentation solution

#### Step 1: Solve for velocity
Rewrite the equation:
\[
\frac{dv}{dt}+\frac{k}{m}v=-g.
\]
This is a first-order linear differential equation.

Its solution is
\[
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}.
\]

#### Step 2: Solve for position
Since
\[
\frac{dx}{dt}=v(t),
\]
integrate:
\[
x(t)=10+\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-kt/m}\right)-\frac{mg}{k}t.
\]

#### Step 3: Maximum height
At maximum height,
\[
v(t_{\max})=0.
\]
So,
\[
\left(v_0+\frac{mg}{k}\right)e^{-kt_{\max}/m}-\frac{mg}{k}=0.
\]
Thus,
\[
e^{-kt_{\max}/m}=\frac{mg}{kv_0+mg},
\]
and
\[
t_{\max}=\frac{m}{k}\ln\left(1+\frac{kv_0}{mg}\right).
\]

Then,
\[
x_{\max}=x(t_{\max}).
\]

#### Step 4: Comparison with no drag
Without drag, the equation becomes
\[
m\frac{dv}{dt}=-mg.
\]
Then
\[
v(t)=v_0-gt,
\]
\[
x(t)=10+v_0t-\frac{1}{2}gt^2,
\]
and the maximum height is
\[
x_{\max,\text{no drag}} = 10+\frac{v_0^2}{2g}.
\]

With drag:
- the upward velocity decreases faster,
- the time to reach the top is shorter,
- the maximum height is lower.

#### Python numerical simulation
```python
import numpy as np
import matplotlib.pyplot as plt

m = 1.0
g = 9.81
k = 0.3
v0 = 20.0
x0 = 10.0

t = np.linspace(0, 5, 500)
v = (v0 + m*g/k) * np.exp(-k*t/m) - m*g/k
x = x0 + (m/k)*(v0 + m*g/k)*(1 - np.exp(-k*t/m)) - (m*g/k)*t

plt.plot(t, x)
plt.xlabel("t [s]")
plt.ylabel("x(t) [m]")
plt.title("Vertical motion with linear drag")
plt.grid(True)
plt.show()
