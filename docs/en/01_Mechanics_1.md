# Section 1: Mechanics I

## 1. Projectile Motion

A projectile is fired from the ground with an initial velocity of $100  \text{ m/s}$ at an angle of $37^\circ$ above the horizontal. Assume no air resistance.

* Derive the differential equations of motion in the horizontal and vertical directions.

* Determine the time of flight.

* Determine the maximum height.

* Determine the range.


### Prepared presentation solution

#### Model and assumptions
- Motion takes place in two dimensions: horizontal \(x\) and vertical \(y\).
- Air resistance is neglected.
- The only force acting on the projectile after launch is gravity.
- Therefore, horizontal acceleration is zero and vertical acceleration is constant and equal to \(-g\).

#### Differential equations of motion
In the horizontal direction:
\[
m\ddot{x} = 0 \quad \Rightarrow \quad \ddot{x} = 0
\]

In the vertical direction:
\[
m\ddot{y} = -mg \quad \Rightarrow \quad \ddot{y} = -g
\]

With the initial conditions:
\[
x(0)=0, \qquad y(0)=0
\]
\[
\dot{x}(0)=v_0\cos\theta, \qquad \dot{y}(0)=v_0\sin\theta
\]

where:
\[
v_0 = 100\ \text{m/s}, \qquad \theta = 37^\circ
\]

#### Position as a function of time
Integrating the horizontal equation:
\[
x(t)=v_0\cos\theta \, t
\]

Integrating the vertical equation:
\[
y(t)=v_0\sin\theta \, t - \frac{1}{2}gt^2
\]

These are the equations of projectile motion.

#### Time of flight
The projectile returns to the ground when \(y(T)=0\):
\[
v_0\sin\theta \, T - \frac{1}{2}gT^2 = 0
\]

Factor out \(T\):
\[
T\left(v_0\sin\theta - \frac{1}{2}gT\right)=0
\]

Ignoring the trivial solution \(T=0\), we obtain:
\[
T=\frac{2v_0\sin\theta}{g}
\]

Substituting the numerical values:
\[
T=\frac{2\cdot 100 \cdot \sin 37^\circ}{9.81}\approx 12.27\ \text{s}
\]

#### Maximum height
The maximum height occurs when the vertical velocity is zero:
\[
\dot{y}(t)=v_0\sin\theta - gt
\]

Set \(\dot{y}(t)=0\):
\[
t_H=\frac{v_0\sin\theta}{g}
\]

Now substitute this into \(y(t)\):
\[
H_{\max}=\frac{v_0^2\sin^2\theta}{2g}
\]

Numerically:
\[
H_{\max}=\frac{100^2\sin^2 37^\circ}{2\cdot 9.81}\approx 181.0\ \text{m}
\]

#### Range
The range is the horizontal distance traveled during the full time of flight:
\[
R=x(T)=v_0\cos\theta \cdot T
\]

Substitute the expression for \(T\):
\[
R=v_0\cos\theta \cdot \frac{2v_0\sin\theta}{g}
\]

Using the identity \(2\sin\theta\cos\theta=\sin 2\theta\):
\[
R=\frac{v_0^2\sin(2\theta)}{g}
\]

Numerically:
\[
R=\frac{100^2\sin 74^\circ}{9.81}\approx 979.9\ \text{m}
\]

#### Final answers
\[
\boxed{T \approx 12.27\ \text{s}}
\]
\[
\boxed{H_{\max} \approx 181.0\ \text{m}}
\]
\[
\boxed{R \approx 979.9\ \text{m}}
\]

#### Interpretation
- The horizontal motion is uniform because there is no horizontal force.
- The vertical motion is uniformly accelerated because gravity acts downward with constant acceleration.
- The trajectory is a parabola.

#### Oral defense note
If asked why the horizontal acceleration is zero, explain that no horizontal force acts on the projectile once it leaves the launcher.
If asked why the vertical acceleration is negative, explain that the positive \(y\)-direction is upward, while gravity acts downward.

## 2. Range Optimization

For projectile motion, show analytically that the maximum range $R(\theta)=\frac{v_0^2 \sin(2\theta)}{g}
$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

## 3. Path Intersection

Alice is moving along a path described by $A(t) = (2+t, 8-3t)$ and Bob is moving along a path $B(t) = (2t-1, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they will collide. If not, determine the minimum distance between them and when it occurs.

## 4. Vector Calculus

The position of an object is given by $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.

## 5. Relative Velocity

A river flows east at $2 \text{m/s}$. A boat that can travel at $5 \text{m/s}$ in still water wants to go directly north across the river. In what direction (angle) should it head? How long will it take to cross the river if it's 200 meters wide?

## 6. Variable Velocity

An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

## 7. Elimination of time and interpretation of acceleration

The path equation is given in parametric form:

$$
x(t)=2t^2, \qquad y(t)=3t^3
$$

* Eliminate the parameter $t$.
* Draw the trajectory.
* Calculate $\vec v(t)$, $|\vec v(t)|$, $\vec a(t)$ and $|\vec a(t)|$.
* Is the acceleration constant?


## 8. Circular Motion

Calculate the centripetal acceleration of a person standing on the Earth's equator. The Earth's radius is approximately 6378 km.

## 9. Momentum Comparison

Which has greater momentum: a 2-gram fly flying at $10$ m/s or a 60-gram tennis ball moving at $1$ m/s?


## 10. Kinematics

Point M moves according to the equation:

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

where $a, b, \omega$ are positive constants.

a) Find the equation of the point's trajectory,

b) Compute the path length of the point from time $t=0$ to $t=t_0$,

c) Draw the trajectory of this point using Python or interactive HTML. Discuss special cases.
