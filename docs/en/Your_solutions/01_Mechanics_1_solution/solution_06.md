## 6. Variable Velocity

An object's velocity is given by $v(t) = t^2 + 2t - 5$. If the object was at $x=4$ at $t=0$, what is its position and acceleration at time $t=3$?

### Prepared presentation solution

#### Given

The velocity is:

$$
v(t)=t^2+2t-5
$$

The initial condition is:

$$
x(0)=4
$$

We must find:
- the position at time $t=3$,
- the acceleration at time $t=3$.

#### Step 1: Find the position function

Velocity is the derivative of position:

$$
v(t)=\frac{dx}{dt}
$$

So:

$$
x(t)=\int (t^2+2t-5)\,dt
$$

Integrating:

$$
x(t)=\frac{t^3}{3}+t^2-5t+C
$$

Use the initial condition $x(0)=4$:

$$
4=C
$$

Therefore:

$$
x(t)=\frac{t^3}{3}+t^2-5t+4
$$

#### Step 2: Compute the position at $t=3$

$$
x(3)=\frac{27}{3}+9-15+4
$$

$$
x(3)=9+9-15+4=7
$$

#### Step 3: Find the acceleration

Acceleration is the derivative of velocity:

$$
a(t)=\frac{dv}{dt}
$$

Differentiate:

$$
a(t)=2t+2
$$

Now evaluate at $t=3$:

$$
a(3)=2\cdot 3+2=8
$$

#### Final answer

$$
\boxed{x(3)=7}
$$

$$
\boxed{a(3)=8}
$$

#### Interpretation
The position is obtained by integrating velocity, while acceleration is obtained by differentiating velocity.

#### Oral defense note
Why does integration give position? Velocity is the rate of change of position, so position is recovered by integrating velocity and using the initial condition.
