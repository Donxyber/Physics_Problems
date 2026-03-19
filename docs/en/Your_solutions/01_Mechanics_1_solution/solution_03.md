## 3. Path Intersection

Alice is moving along a path described by $A(t) = (2+t,\, 8-3t)$ and Bob is moving along a path $B(t) = (2t-1,\, 2t+2)$. Determine if their paths intersect. If yes, determine when and where they will collide. If not, determine the minimum distance between them and when it occurs.

### Prepared presentation solution

#### Given paths

Alice moves along:

$$
A(t)=(2+t,\ 8-3t)
$$

Bob moves along:

$$
B(t)=(2t-1,\ 2t+2)
$$

We must determine:
- whether they collide,
- if not, whether their paths intersect geometrically,
- and the minimum distance between them.

#### Step 1: Check whether they collide at the same time

For a collision, both coordinates must be equal for the same value of $t$:

$$
2+t=2t-1
$$

$$
8-3t=2t+2
$$

From the first equation:

$$
t=3
$$

From the second equation:

$$
6=5t
\Rightarrow
t=\frac{6}{5}
$$

These values are not equal, so there is no single time $t$ for which both coordinates match.

#### Conclusion about collision

They do **not** collide.

#### Step 2: Check whether the paths intersect geometrically

Now allow different parameters $t_A$ and $t_B$:

$$
2+t_A=2t_B-1
$$

$$
8-3t_A=2t_B+2
$$

From the first equation:

$$
t_A=2t_B-3
$$

Substitute into the second:

$$
8-3(2t_B-3)=2t_B+2
$$

$$
8-6t_B+9=2t_B+2
$$

$$
15=8t_B
\Rightarrow
t_B=\frac{15}{8}
$$

Then:

$$
t_A=2\cdot \frac{15}{8}-3=\frac{3}{4}
$$

Substitute into Alice’s path:

$$
A\left(\frac{3}{4}\right)=\left(2+\frac{3}{4},\ 8-3\cdot\frac{3}{4}\right)
=\left(\frac{11}{4},\ \frac{23}{4}\right)
$$

#### Geometric intersection point

The two paths intersect geometrically at:

$$
\left(\frac{11}{4},\ \frac{23}{4}\right)
$$

#### Step 3: Minimum distance between them at the same time

Distance squared:

$$
D^2(t)=\left[(2+t)-(2t-1)\right]^2+\left[(8-3t)-(2t+2)\right]^2
$$

Simplify:

$$
D^2(t)=(3-t)^2+(6-5t)^2
$$

$$
D^2(t)=26t^2-66t+45
$$

To minimize distance, differentiate:

$$
\frac{d}{dt}D^2(t)=52t-66
$$

Set equal to zero:

$$
52t-66=0
\Rightarrow
t=\frac{33}{26}
$$

Now compute the minimum distance:

$$
D_{\min}^2=26\left(\frac{33}{26}\right)^2-66\left(\frac{33}{26}\right)+45
=\frac{81}{26}
$$

Thus:

$$
D_{\min}=\frac{9}{\sqrt{26}}\approx 1.765
$$

#### Final answer
- The paths intersect geometrically.
- They do **not** collide at the same time.
- The geometric intersection point is:

$$
\boxed{\left(\frac{11}{4},\ \frac{23}{4}\right)}
$$

- The minimum distance is:

$$
\boxed{D_{\min}=\frac{9}{\sqrt{26}}\approx 1.765}
$$

- It occurs at:

$$
\boxed{t=\frac{33}{26}\approx 1.269}
$$

#### Interpretation
This problem distinguishes between:
- two trajectories crossing in space,
- and two objects arriving at the same point at the same time.

Those are not the same thing.

#### Oral defense note
If asked whether “the paths intersect” means collision, answer: no. A collision requires both the same point and the same time. Here, the geometric paths intersect, but Alice and Bob reach that point at different times.

