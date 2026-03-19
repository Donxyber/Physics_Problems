## 4. Vector Calculus

The position of an object is given by $\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$. Find the object's velocity and acceleration vectors as a function of time.

### Prepared presentation solution

#### Given position vector

$$
\vec r(t)=(3t^2)\hat i+(5t-8t^2)\hat j
$$

We must find the velocity and acceleration vectors.

#### Velocity vector

Velocity is the derivative of position:

$$
\vec v(t)=\frac{d\vec r}{dt}
$$

Differentiate each component:

$$
\frac{d}{dt}(3t^2)=6t
$$

$$
\frac{d}{dt}(5t-8t^2)=5-16t
$$

Therefore:

$$
\vec v(t)=6t\,\hat i+(5-16t)\,\hat j
$$

#### Acceleration vector

Acceleration is the derivative of velocity:

$$
\vec a(t)=\frac{d\vec v}{dt}
$$

Differentiate again:

$$
\frac{d}{dt}(6t)=6
$$

$$
\frac{d}{dt}(5-16t)=-16
$$

So:

$$
\vec a(t)=6\,\hat i-16\,\hat j
$$

#### Final answer

$$
\boxed{\vec v(t)=6t\,\hat i+(5-16t)\,\hat j}
$$

$$
\boxed{\vec a(t)=6\,\hat i-16\,\hat j}
$$

#### Interpretation
The acceleration is constant because both components of the acceleration vector are constant numbers.

#### Oral defense note
If asked why velocity is obtained by differentiation, explain that velocity is the rate of change of position with respect to time, and acceleration is the rate of change of velocity.

