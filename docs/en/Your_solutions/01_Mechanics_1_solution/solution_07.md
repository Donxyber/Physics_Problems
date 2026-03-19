## 7. Elimination of Time and Interpretation of Acceleration

The path equation is given in parametric form:

$$
x(t)=2t^2, \qquad y(t)=3t^3
$$

- Eliminate the parameter $t$.
- Draw the trajectory.
- Calculate $\vec v(t)$, $|\vec v(t)|$, $\vec a(t)$, and $|\vec a(t)|$.
- Is the acceleration constant?

### Prepared presentation solution

#### Given parametric equations

$$
x(t)=2t^2,\qquad y(t)=3t^3
$$

We must:
- eliminate the parameter $t$,
- describe the trajectory,
- calculate $\vec v$, $|\vec v|$, $\vec a$, and $|\vec a|$,
- determine whether the acceleration is constant.

#### Step 1: Eliminate the parameter

From:

$$
x=2t^2
$$

we obtain:

$$
t^2=\frac{x}{2}
$$

Now square the equation for $y$:

$$
y^2=(3t^3)^2=9t^6
$$

But:

$$
t^6=(t^2)^3
$$

So:

$$
y^2=9\left(\frac{x}{2}\right)^3
$$

Hence the trajectory is:

$$
\boxed{y^2=\frac{9}{8}x^3}
$$

#### Step 2: Describe the trajectory

This is a semicubical parabola.

If $t\ge 0$, then $x\ge 0$ and $y\ge 0$, so the motion follows the upper-right branch.

#### Step 3: Velocity vector

Velocity is:

$$
\vec v(t)=\left(\frac{dx}{dt},\frac{dy}{dt}\right)
$$

Differentiate:

$$
\frac{dx}{dt}=4t,\qquad \frac{dy}{dt}=9t^2
$$

Therefore:

$$
\boxed{\vec v(t)=(4t,\ 9t^2)}
$$

#### Step 4: Speed

$$
|\vec v(t)|=\sqrt{(4t)^2+(9t^2)^2}
$$

So:

$$
|\vec v(t)|=\sqrt{16t^2+81t^4}
$$

This can also be written as:

$$
\boxed{|\vec v(t)|=|t|\sqrt{16+81t^2}}
$$

If $t\ge 0$, then:

$$
|\vec v(t)|=t\sqrt{16+81t^2}
$$

#### Step 5: Acceleration vector

Acceleration is:

$$
\vec a(t)=\left(\frac{d^2x}{dt^2},\frac{d^2y}{dt^2}\right)
$$

Differentiate again:

$$
\frac{d^2x}{dt^2}=4,\qquad \frac{d^2y}{dt^2}=18t
$$

Thus:

$$
\boxed{\vec a(t)=(4,\ 18t)}
$$

#### Step 6: Magnitude of acceleration

$$
|\vec a(t)|=\sqrt{4^2+(18t)^2}
$$

So:

$$
\boxed{|\vec a(t)|=\sqrt{16+324t^2}}
$$

#### Step 7: Is the acceleration constant?

No.

Although the $x$-component is constant, the $y$-component is:

$$
18t
$$

which depends on time.

Therefore the acceleration vector changes with time.

#### Final answer

$$
\boxed{y^2=\frac{9}{8}x^3}
$$

$$
\boxed{\vec v(t)=(4t,\ 9t^2)}
$$

$$
\boxed{|\vec v(t)|=\sqrt{16t^2+81t^4}}
$$

$$
\boxed{\vec a(t)=(4,\ 18t)}
$$

$$
\boxed{|\vec a(t)|=\sqrt{16+324t^2}}
$$

Acceleration is **not constant**.

#### Interpretation
The particle does not move with uniform acceleration because one component of the acceleration depends on time.

#### Oral defense note
If asked whether constant magnitude means constant acceleration, answer carefully: acceleration is a vector. Here the vector itself changes with time, so the acceleration is not constant.

