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


### Prepared presentation solution

#### Goal
We want to show analytically that for projectile motion, the maximum range for a given initial speed is obtained at a launch angle of \(45^\circ\).

#### Starting formula
For projectile motion without air resistance, the range is:
\[
R=\frac{v_0^2\sin(2\theta)}{g}
\]

where:
- \(v_0\) is the initial velocity,
- \(\theta\) is the launch angle,
- \(g\) is the gravitational acceleration.

#### Optimization
For fixed \(v_0\) and \(g\), the only variable is:
\[
\sin(2\theta)
\]

The sine function satisfies:
\[
-1 \leq \sin(2\theta) \leq 1
\]

Therefore, the maximum possible value of the range is obtained when:
\[
\sin(2\theta)=1
\]

This occurs when:
\[
2\theta=90^\circ
\]

Hence:
\[
\theta=45^\circ
\]

#### Maximum range
Substituting \(\sin(2\theta)=1\) into the range formula:
\[
R_{\max}=\frac{v_0^2}{g}
\]

#### Final answer
\[
\boxed{\theta=45^\circ}
\]
\[
\boxed{R_{\max}=\frac{v_0^2}{g}}
\]

#### Interpretation
The range depends on both the horizontal and vertical components of the initial velocity.  
At \(45^\circ\), these components are balanced in the way that maximizes the horizontal distance traveled.

#### Oral defense note
If asked why \(45^\circ\) is optimal, explain that the range is proportional to \(\sin(2\theta)\), and sine reaches its maximum value of 1 at \(90^\circ\), so \(2\theta=90^\circ\), hence \(\theta=45^\circ\).


## 3. Path Intersection

Alice is moving along a path described by $A(t) = (2+t, 8-3t)$ and Bob is moving along a path $B(t) = (2t-1, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they will collide. If not, determine the minimum distance between them and when it occurs.


### Prepared presentation solution

#### Given paths
Alice moves along:
\[
A(t)=(2+t,\ 8-3t)
\]

Bob moves along:
\[
B(t)=(2t-1,\ 2t+2)
\]

We must determine:
- whether they collide,
- if not, whether their paths intersect geometrically,
- and the minimum distance between them.

#### Step 1: Check whether they collide at the same time
For a collision, both coordinates must be equal for the same value of \(t\):

\[
2+t=2t-1
\]
\[
8-3t=2t+2
\]

From the first equation:
\[
t=3
\]

From the second equation:
\[
6=5t
\Rightarrow
t=\frac{6}{5}
\]

These values are not equal, so there is no single time \(t\) for which both coordinates match.

#### Conclusion about collision
They do **not** collide.

#### Step 2: Check whether the paths intersect geometrically
Now allow different parameters \(t_A\) and \(t_B\):

\[
2+t_A=2t_B-1
\]
\[
8-3t_A=2t_B+2
\]

From the first equation:
\[
t_A=2t_B-3
\]

Substitute into the second:
\[
8-3(2t_B-3)=2t_B+2
\]
\[
8-6t_B+9=2t_B+2
\]
\[
15=8t_B
\Rightarrow
t_B=\frac{15}{8}
\]

Then:
\[
t_A=2\cdot \frac{15}{8}-3=\frac{3}{4}
\]

Substitute into Alice’s path:
\[
A\left(\frac{3}{4}\right)=\left(2+\frac{3}{4},\ 8-3\cdot\frac{3}{4}\right)
=\left(\frac{11}{4},\ \frac{23}{4}\right)
\]

#### Geometric intersection point
The two paths intersect geometrically at:
\[
\left(\frac{11}{4},\ \frac{23}{4}\right)
\]

#### Step 3: Minimum distance between them at the same time
Distance squared:
\[
D^2(t)=\left[(2+t)-(2t-1)\right]^2+\left[(8-3t)-(2t+2)\right]^2
\]

Simplify:
\[
D^2(t)=(3-t)^2+(6-5t)^2
\]
\[
D^2(t)=26t^2-66t+45
\]

To minimize distance, differentiate:
\[
\frac{d}{dt}D^2(t)=52t-66
\]

Set equal to zero:
\[
52t-66=0
\Rightarrow
t=\frac{33}{26}
\]

Now compute the minimum distance:
\[
D_{\min}^2=26\left(\frac{33}{26}\right)^2-66\left(\frac{33}{26}\right)+45
=\frac{81}{26}
\]

Thus:
\[
D_{\min}=\frac{9}{\sqrt{26}}\approx 1.765
\]

#### Final answer
- The paths intersect geometrically.
- They do **not** collide at the same time.
- The geometric intersection point is:
\[
\boxed{\left(\frac{11}{4},\ \frac{23}{4}\right)}
\]
- The minimum distance is:
\[
\boxed{D_{\min}=\frac{9}{\sqrt{26}}\approx 1.765}
\]
- It occurs at:
\[
\boxed{t=\frac{33}{26}\approx 1.269}
\]

#### Interpretation
This problem distinguishes between:
- two trajectories crossing in space,
- and two objects arriving at the same point at the same time.

Those are not the same thing.

#### Oral defense note
If asked whether “the paths intersect” means collision, answer: no. A collision requires both the same point and the same time. Here, the geometric paths intersect, but Alice and Bob reach that point at different times.


## 4. Vector Calculus

The position of an object is given by $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.


### Prepared presentation solution

#### Given position vector
\[
\vec r(t)=(3t^2)\hat i+(5t-8t^2)\hat j
\]

We must find the velocity and acceleration vectors.

#### Velocity vector
Velocity is the derivative of position:
\[
\vec v(t)=\frac{d\vec r}{dt}
\]

Differentiate each component:
\[
\frac{d}{dt}(3t^2)=6t
\]
\[
\frac{d}{dt}(5t-8t^2)=5-16t
\]

Therefore:
\[
\vec v(t)=6t\,\hat i+(5-16t)\,\hat j
\]

#### Acceleration vector
Acceleration is the derivative of velocity:
\[
\vec a(t)=\frac{d\vec v}{dt}
\]

Differentiate again:
\[
\frac{d}{dt}(6t)=6
\]
\[
\frac{d}{dt}(5-16t)=-16
\]

So:
\[
\vec a(t)=6\,\hat i-16\,\hat j
\]

#### Final answer
\[
\boxed{\vec v(t)=6t\,\hat i+(5-16t)\,\hat j}
\]
\[
\boxed{\vec a(t)=6\,\hat i-16\,\hat j}
\]

#### Interpretation
The acceleration is constant because both components of the acceleration vector are constant numbers.

#### Oral defense note
If asked why velocity is obtained by differentiation, explain that velocity is the rate of change of position with respect to time, and acceleration is the rate of change of velocity.


## 5. Relative Velocity

A river flows east at $2 \text{m/s}$. A boat that can travel at $5 \text{m/s}$ in still water wants to go directly north across the river. In what direction (angle) should it head? How long will it take to cross the river if it's 200 meters wide?


### Prepared presentation solution

#### Given
- The river flows east at:
\[
2\ \text{m/s}
\]
- The boat's speed in still water is:
\[
5\ \text{m/s}
\]
- The river is:
\[
200\ \text{m}
\]
wide.

The boat wants to travel directly north across the river.

#### Step 1: Choose the direction of the boat
Let the boat head at an angle \(\alpha\) west of north.

Its velocity relative to the water has magnitude:
\[
5\ \text{m/s}
\]

To go directly north, the westward component of the boat's velocity must exactly cancel the eastward river flow.

So:
\[
5\sin\alpha=2
\]

Hence:
\[
\sin\alpha=\frac{2}{5}
\]

Therefore:
\[
\alpha=\arcsin\left(\frac{2}{5}\right)\approx 23.58^\circ
\]

#### Direction
The boat must head:
\[
\boxed{23.58^\circ\ \text{west of north}}
\]

#### Step 2: Find the northward velocity
The northward component is:
\[
v_N=5\cos\alpha
\]

Using:
\[
\cos\alpha=\sqrt{1-\sin^2\alpha}
=\sqrt{1-\left(\frac{2}{5}\right)^2}
=\sqrt{\frac{21}{25}}
=\frac{\sqrt{21}}{5}
\]

So:
\[
v_N=5\cdot \frac{\sqrt{21}}{5}=\sqrt{21}\approx 4.58\ \text{m/s}
\]

#### Step 3: Crossing time
Time is distance divided by northward speed:
\[
t=\frac{200}{\sqrt{21}}\approx 43.6\ \text{s}
\]

#### Final answer
\[
\boxed{\text{Direction: }23.58^\circ\ \text{west of north}}
\]
\[
\boxed{t\approx 43.6\ \text{s}}
\]

#### Interpretation
The boat does not point directly north.  
It must aim slightly upstream so that the river's eastward current is canceled.

#### Oral defense note
If asked why the boat must aim west of north, explain that the river pushes it east, so the boat must generate a westward component to compensate.


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
