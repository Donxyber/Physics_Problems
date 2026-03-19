## 2. Range Optimization

For projectile motion, show analytically that the maximum range $R(\theta)=\frac{v_0^2\sin(2\theta)}{g}$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

### Prepared presentation solution

#### Goal
We want to show analytically that for projectile motion, the maximum range for a given initial speed is obtained at a launch angle of $45^\circ$.

#### Starting formula

For projectile motion without air resistance, the range is:

$$
R=\frac{v_0^2\sin(2\theta)}{g}
$$

where:
- $v_0$ is the initial velocity,
- $\theta$ is the launch angle,
- $g$ is the gravitational acceleration.

#### Optimization

For fixed $v_0$ and $g$, the only variable is:

$$
\sin(2\theta)
$$

The sine function satisfies:

$$
-1 \leq \sin(2\theta) \leq 1
$$

Therefore, the maximum possible value of the range is obtained when:

$$
\sin(2\theta)=1
$$

This occurs when:

$$
2\theta=90^\circ
$$

Hence:

$$
\theta=45^\circ
$$

#### Maximum range

Substituting $\sin(2\theta)=1$ into the range formula:

$$
R_{\max}=\frac{v_0^2}{g}
$$

#### Final answer

$$
\boxed{\theta=45^\circ}
$$

$$
\boxed{R_{\max}=\frac{v_0^2}{g}}
$$

#### Interpretation
The range depends on both the horizontal and vertical components of the initial velocity.  
At $45^\circ$, these components are balanced in the way that maximizes the horizontal distance traveled.

#### Oral defense note
If asked why $45^\circ$ is optimal, explain that the range is proportional to $\sin(2\theta)$, and sine reaches its maximum value of 1 at $90^\circ$, so $2\theta=90^\circ$, hence $\theta=45^\circ$.

