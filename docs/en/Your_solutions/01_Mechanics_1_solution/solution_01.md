## 1. Projectile Motion

A projectile is fired from the ground with an initial velocity of $100\ \text{m/s}$ at an angle of $37^\circ$ above the horizontal. Assume no air resistance.

- Derive the differential equations of motion in the horizontal and vertical directions.
- Determine the time of flight.
- Determine the maximum height.
- Determine the range.

### Prepared presentation solution

#### Model and assumptions
- Motion takes place in two dimensions: horizontal $x$ and vertical $y$.
- Air resistance is neglected.
- The only force acting on the projectile after launch is gravity.
- Therefore, horizontal acceleration is zero and vertical acceleration is constant and equal to $-g$.

#### Differential equations of motion

In the horizontal direction:

$$
m\ddot{x} = 0 \quad \Rightarrow \quad \ddot{x} = 0
$$

In the vertical direction:

$$
m\ddot{y} = -mg \quad \Rightarrow \quad \ddot{y} = -g
$$

With the initial conditions:

$$
x(0)=0, \qquad y(0)=0
$$

$$
\dot{x}(0)=v_0\cos\theta, \qquad \dot{y}(0)=v_0\sin\theta
$$

where:

$$
v_0 = 100\ \text{m/s}, \qquad \theta = 37^\circ
$$

#### Position as a function of time

Integrating the horizontal equation:

$$
x(t)=v_0\cos\theta \, t
$$

Integrating the vertical equation:

$$
y(t)=v_0\sin\theta \, t - \frac{1}{2}gt^2
$$

These are the equations of projectile motion.

#### Time of flight

The projectile returns to the ground when $y(T)=0$:

$$
v_0\sin\theta \, T - \frac{1}{2}gT^2 = 0
$$

Factor out $T$:

$$
T\left(v_0\sin\theta - \frac{1}{2}gT\right)=0
$$

Ignoring the trivial solution $T=0$, we obtain:

$$
T=\frac{2v_0\sin\theta}{g}
$$

Substituting the numerical values:

$$
T=\frac{2\cdot 100 \cdot \sin 37^\circ}{9.81}\approx 12.27\ \text{s}
$$

#### Maximum height

The maximum height occurs when the vertical velocity is zero:

$$
\dot{y}(t)=v_0\sin\theta - gt
$$

Set $\dot{y}(t)=0$:

$$
t_H=\frac{v_0\sin\theta}{g}
$$

Now substitute this into $y(t)$:

$$
H_{\max}=\frac{v_0^2\sin^2\theta}{2g}
$$

Numerically:

$$
H_{\max}=\frac{100^2\sin^2 37^\circ}{2\cdot 9.81}\approx 181.0\ \text{m}
$$

#### Range

The range is the horizontal distance traveled during the full time of flight:

$$
R=x(T)=v_0\cos\theta \cdot T
$$

Substitute the expression for $T$:

$$
R=v_0\cos\theta \cdot \frac{2v_0\sin\theta}{g}
$$

Using the identity $2\sin\theta\cos\theta=\sin 2\theta$:

$$
R=\frac{v_0^2\sin(2\theta)}{g}
$$

Numerically:

$$
R=\frac{100^2\sin 74^\circ}{9.81}\approx 979.9\ \text{m}
$$

#### Final answers

$$
\boxed{T \approx 12.27\ \text{s}}
$$

$$
\boxed{H_{\max} \approx 181.0\ \text{m}}
$$

$$
\boxed{R \approx 979.9\ \text{m}}
$$

#### Interpretation
- The horizontal motion is uniform because there is no horizontal force.
- The vertical motion is uniformly accelerated because gravity acts downward with constant acceleration.
- The trajectory is a parabola.
