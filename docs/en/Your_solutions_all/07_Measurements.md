# Section 7: Measurements

## 1. Propagation of Error I

The radius of a sphere is measured to be $r = (6.20 \pm 0.05)\text{ cm}$. Calculate the volume of the sphere and its associated uncertainty.

### Prepared presentation solution

The volume of a sphere is

$$
V=\frac{4}{3}\pi r^3
$$

Substitute $r=6.20\ \text{cm}$:

$$
V=\frac{4}{3}\pi (6.20)^3 \approx 998.31\ \text{cm}^3
$$

For a power law, the relative uncertainty is

$$
\frac{\Delta V}{V}=3\frac{\Delta r}{r}
$$

So,

$$
\frac{\Delta V}{V}=3\cdot \frac{0.05}{6.20}\approx 0.0242
$$

Thus,

$$
\Delta V = 0.0242 \times 998.31 \approx 24.15\ \text{cm}^3
$$

### Final answer

$$
V=(998.3 \pm 24.2)\ \text{cm}^3
$$

---

## 2. Propagation of Error II

The length and width of a rectangular plate are measured to be $L = (15.3 \pm 0.1)\text{ cm}$ and $W = (8.4 \pm 0.1)\text{ cm}$. Calculate the area of the plate and its uncertainty.

### Prepared presentation solution

The area is

$$
A=LW
$$

So,

$$
A=15.3\times 8.4 = 128.52\ \text{cm}^2
$$

For multiplication, relative uncertainties add:

$$
\frac{\Delta A}{A}=\frac{\Delta L}{L}+\frac{\Delta W}{W}
$$

Thus,

$$
\frac{\Delta A}{A}=\frac{0.1}{15.3}+\frac{0.1}{8.4}\approx 0.01844
$$

Therefore,

$$
\Delta A = 0.01844\times 128.52 \approx 2.37\ \text{cm}^2
$$

### Final answer

$$
A=(128.5 \pm 2.4)\ \text{cm}^2
$$

---

## 3. Propagation of Error III

The resistance $R$ is calculated using Ohm's Law, $R = V/I$. If the voltage is measured as $V = (10.0 \pm 0.2)\text{ V}$ and the current as $I = (2.00 \pm 0.05)\text{ A}$, what is the calculated resistance and its uncertainty?

### Prepared presentation solution

The resistance is

$$
R=\frac{V}{I}
$$

So,

$$
R=\frac{10.0}{2.00}=5.00\ \Omega
$$

For division, relative uncertainties add:

$$
\frac{\Delta R}{R}=\frac{\Delta V}{V}+\frac{\Delta I}{I}
$$

Thus,

$$
\frac{\Delta R}{R}=\frac{0.2}{10.0}+\frac{0.05}{2.00}=0.02+0.025=0.045
$$

Therefore,

$$
\Delta R = 0.045\times 5.00 = 0.225\ \Omega
$$

### Final answer

$$
R=(5.00 \pm 0.23)\ \Omega
$$

---

## 4. Relative Uncertainty

A car's speedometer has a 5% uncertainty. If it reads 60 km/h, what is the range of the car's actual speed?

### Prepared presentation solution

Absolute uncertainty:

$$
\Delta v = 0.05\times 60 = 3\ \text{km/h}
$$

So the actual speed lies between

$$
60-3=57\ \text{km/h}
$$

and

$$
60+3=63\ \text{km/h}
$$

### Final answer

$$
57\ \text{km/h} \le v \le 63\ \text{km/h}
$$

---

## 5. Percentage Calculation

A measurement of time is recorded as $t = 5.45 \pm 0.22$ seconds. What is the percentage uncertainty of this measurement?

### Prepared presentation solution

Percentage uncertainty is

$$
\frac{\Delta t}{t}\times 100\%
$$

So,

$$
\frac{0.22}{5.45}\times 100\% \approx 4.04\%
$$

### Final answer

$$
\text{Percentage uncertainty} \approx 4.0\%
$$

---

## 6. Instrument Precision

A digital thermometer reads $25.4^\circ\text{C}$. Assuming the uncertainty is half the value of the last digit, what is the absolute uncertainty of this measurement?

### Prepared presentation solution

The last digit is in tenths of a degree:

$$
0.1^\circ\text{C}
$$

Half of that is

$$
0.05^\circ\text{C}
$$

### Final answer

$$
25.4 \pm 0.05^\circ\text{C}
$$

---

## 7. Standard Deviation

Eleven students received the following scores on a test: 88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89.

What is the mean

$$
\bar{x}=\frac{1}{N}\sum_{i=1}^{N}x_i
$$

and standard deviation

$$
\sigma=\sqrt{\frac{1}{N-1}\sum_{i=1}^{N}(x_i-\bar{x})^2}
$$

of these test scores? If the highest and lowest scores are removed, what are the new mean and standard deviation of the remaining scores?

### Prepared presentation solution

#### Original data

Data:

$$
88,\ 92,\ 79,\ 85,\ 95,\ 81,\ 86,\ 90,\ 83,\ 77,\ 89
$$

Number of scores:

$$
N=11
$$

Sum:

$$
\sum x_i = 945
$$

Mean:

$$
\bar{x}=\frac{945}{11}\approx 85.91
$$

Using

$$
\sigma=\sqrt{\frac{1}{N-1}\sum_{i=1}^{N}(x_i-\bar{x})^2}
$$

the sample standard deviation is

$$
\sigma \approx 5.58
$$

#### After removing highest and lowest

Remove 95 and 77.

Remaining scores:

$$
79,\ 81,\ 83,\ 85,\ 86,\ 88,\ 89,\ 90,\ 92
$$

New number of scores:

$$
N=9
$$

New sum:

$$
\sum x_i = 773
$$

New mean:

$$
\bar{x}=\frac{773}{9}\approx 85.89
$$

New sample standard deviation:

$$
\sigma \approx 4.31
$$

### Final answers

Original set:

$$
\bar{x}\approx 85.91,\qquad \sigma\approx 5.58
$$

Trimmed set:

$$
\bar{x}\approx 85.89,\qquad \sigma\approx 4.31
$$

---

## 8. Mass-Spring Measurements - html

Generate a simulator of a mass suspended on a spring in HTML with a timing function. Treating the mass as a given value with zero uncertainty, perform a series of 10 time measurements for 10 complete oscillations. Use the collected data to calculate the mean period, standard deviation. Calculate the value of the spring constant along with its measurement uncertainty.

### Live simulator

Open the live simulator here:

[Open Mass-Spring Simulator](mass_spring_measurements.html)

### What the simulator does

- Animates a mass on a spring
- Lets you start and stop timing manually
- Stores 10 measurements of the time for 10 oscillations
- Calculates:
  - mean time for 10 oscillations
  - mean period
  - standard deviation
  - spring constant using

$$
T=2\pi\sqrt{\frac{m}{k}}
$$

so

$$
k=\frac{4\pi^2 m}{T^2}
$$

If the mass is treated as exact, then the relative uncertainty in $k$ is

$$
\frac{\Delta k}{k}=2\frac{\Delta T}{T}
$$

---

## 9. Pendulum Measurements - html/real

Create a simple pendulum simulator in HTML equipped with a stopwatch for manual timing. Assuming the string length is an exact value, run the simulation and perform 10 measurements of the time taken for 10 complete oscillations. Based on the obtained results, manually calculate the mean period and standard deviation. Using this data, determine the value of the acceleration due to gravity and calculate the measurement uncertainty of this result.

### Live simulator

Open the live simulator here:

[Open Pendulum Simulator](pendulum_measurements.html)

### What the simulator does

- Animates a simple pendulum
- Lets you start and stop timing manually
- Stores 10 measurements of the time for 10 oscillations
- Calculates:
  - mean time for 10 oscillations
  - mean period
  - standard deviation
  - gravitational acceleration using

$$
T=2\pi\sqrt{\frac{L}{g}}
$$

so

$$
g=\frac{4\pi^2L}{T^2}
$$

If the string length is treated as exact, then the relative uncertainty in $g$ is

$$
\frac{\Delta g}{g}=2\frac{\Delta T}{T}
$$

### Optional real-life experiment

You may repeat the same procedure with a real pendulum:
- use a string and small mass
- measure the string length
- measure the time for 10 oscillations ten times
- compute the mean period and standard deviation
- then calculate $g$ and its uncertainty

---

## 10. Light Speed Measurement

Measure the speed of light using a microwave oven, a bar of chocolate (or slices of cheese), and a ruler. To this end, measure the distance between the melted spots on the chocolate to determine the wavelength of the microwaves. Use the frequency of the typical microwave oven, $f=2.45\ \text{GHz}$, to calculate the speed of light. How does your result compare to the accepted value of $c = 300\,000\,000\ \text{m/s}$? What is the percentage error of your measurement?

### Prepared presentation solution

In a microwave oven, the distance between two melted spots corresponds to half the wavelength:

$$
\frac{\lambda}{2}=d
$$

So,

$$
\lambda=2d
$$

The wave speed is

$$
c=f\lambda
$$

#### Example calculation

Suppose the distance between two melted spots is

$$
d=6.1\ \text{cm}=0.061\ \text{m}
$$

Then

$$
\lambda=2d=0.122\ \text{m}
$$

Using

$$
f=2.45\times 10^9\ \text{Hz}
$$

we get

$$
c=f\lambda=(2.45\times 10^9)(0.122)\approx 2.989\times 10^8\ \text{m/s}
$$

Compare with accepted value:

$$
c_0=3.00\times 10^8\ \text{m/s}
$$

Percentage error:

$$
\%\text{ error}=\frac{|c-c_0|}{c_0}\times 100\%
$$

$$
\%\text{ error}=\frac{|2.989\times 10^8-3.00\times 10^8|}{3.00\times 10^8}\times 100\%
\approx 0.37\%
$$

### Final answer for the example

$$
c\approx 2.99\times 10^8\ \text{m/s}
$$

$$
\%\text{ error}\approx 0.37\%
$$

Replace the example value of $d$ with your own measured spacing if you perform the experiment yourself.
