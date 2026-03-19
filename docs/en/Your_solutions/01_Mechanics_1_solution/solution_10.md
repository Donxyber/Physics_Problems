## 10. Kinematics

Point $M$ moves according to the equation:

$$
\vec{r}(t) = (a \cos(\omega t),\, b \sin(\omega t),\, bt)
$$

where $a$, $b$, $\omega$ are positive constants.

a) Find the equation of the point's trajectory.

b) Compute the path length of the point from time $t=0$ to $t=t_0$.

c) Draw the trajectory of this point using Python or interactive HTML. Discuss special cases.

### Prepared presentation solution

#### Given

The point moves according to:

$$
\vec r(t)=\big(a\cos(\omega t),\ b\sin(\omega t),\ bt\big)
$$

where $a$, $b$, and $\omega$ are positive constants.

We must:
- find the trajectory,
- compute the path length from $t=0$ to $t=t_0$,
- describe the curve and discuss special cases.

#### a) Equation of the trajectory

The coordinates are:

$$
x=a\cos(\omega t),\qquad y=b\sin(\omega t),\qquad z=bt
$$

From the first two equations:

$$
\left(\frac{x}{a}\right)^2+\left(\frac{y}{b}\right)^2=1
$$

So the projection onto the $xy$-plane is an ellipse.

Since:

$$
t=\frac{z}{b}
$$

we can substitute into the first two equations:

$$
x=a\cos\left(\frac{\omega z}{b}\right),\qquad
y=b\sin\left(\frac{\omega z}{b}\right)
$$

Thus the trajectory is an **elliptical helix**.

#### Final trajectory form

$$
\boxed{\left(\frac{x}{a}\right)^2+\left(\frac{y}{b}\right)^2=1}
$$

with

$$
\boxed{x=a\cos\left(\frac{\omega z}{b}\right),\qquad y=b\sin\left(\frac{\omega z}{b}\right)}
$$

#### b) Path length from $t=0$ to $t=t_0$

The velocity vector is:

$$
\vec r\,'(t)=\big(-a\omega\sin(\omega t),\ b\omega\cos(\omega t),\ b\big)
$$

Its magnitude is:

$$
|\vec r\,'(t)|=
\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}
$$

Therefore, the arc length is:

$$
s(t_0)=\int_0^{t_0}
\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}\,dt
$$

So:

$$
\boxed{
s(t_0)=\int_0^{t_0}
\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}\,dt
}
$$

In the general case, this integral is not elementary.

#### c) Interpretation and special cases

- The motion is helical because the point rotates in the $xy$-plane while rising linearly in $z$.
- The projection onto the $xy$-plane is an ellipse.
- Therefore the full trajectory is an elliptical helix.

##### Special case 1: $a=b$

If $a=b=R$, then:

$$
x=R\cos(\omega t),\qquad y=R\sin(\omega t)
$$

The projection becomes a circle, so the trajectory is a **circular helix**.

In this case:

$$
|\vec r\,'(t)|=\sqrt{R^2\omega^2+b^2}
$$

which is constant, and then:

$$
\boxed{s(t_0)=t_0\sqrt{R^2\omega^2+b^2}}
$$

##### Special case 2: $\omega\to 0$

The oscillatory motion becomes very slow, so the path approaches a nearly vertical straight line.

##### Special case 3: very small $b$ in the $z$-component

The vertical rise per unit time becomes small, so the helix becomes more compressed.

#### Example Python code for plotting

```python
import numpy as np
import matplotlib.pyplot as plt

a = 3
b = 2
omega = 1.5
t0 = 10

t = np.linspace(0, t0, 1000)
x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

fig = plt.figure(figsize=(8, 6))
ax = fig.add_subplot(111, projection='3d')
ax.plot(x, y, z)
ax.set_xlabel('x')
ax.set_ylabel('y')
ax.set_zlabel('z')
ax.set_title('Trajectory of M: elliptical helix')
plt.show()
