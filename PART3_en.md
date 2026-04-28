Here is the fully corrected **Unit 3** content in English Markdown, incorporating all fixes (including trigonometric inequalities, phase shift handling, atan2 for polar coordinates, etc.).

---

# 📐 UNIT 3: Trigonometric and Polar Functions

> **AP Exam Weighting:** $30$–$35\%$  
> **Recommended Class Periods:** $35$–$50$  
> **Total Topics:** $15$ (3.1 through 3.15)

---

## 🔹 3.1 — Periodic Phenomena

### Core Concept

A **periodic function** repeats its output values over equal‑length input intervals. If there exists a smallest positive number $k$ such that for all $x$:

$$
f(x + k) = f(x)
$$

then $k$ is the **minimum positive period**.

**Key properties:**
- All features of a periodic function (intervals of increase/decrease, concavity, rate of change) repeat exactly in each period.
- Knowing the graph over one full period allows you to draw the entire graph via translations.
- The period can be estimated by the horizontal distance between consecutive maxima (or consecutive minima).

### Example

> **Example 1:** Tide data shows high tide at $t=0$ and the next high tide at $t=12$ hours. Estimate the period.

$$
\text{Period} = 12 \text{ hours}
$$

---

## 🔹 3.2 — Sine, Cosine, and Tangent

### Unit Circle Definition

For an angle $\theta$ in standard position:
- **Vertex** at the origin
- **Initial side** along the positive $x$-axis
- **Terminal ray** is the other side

> **Positive angle** = counter‑clockwise rotation; **Negative angle** = clockwise rotation.

Angles that are coterminal differ by integer multiples of $2\pi$, with $k \in \mathbb{Z}$:

$$
\theta + 2\pi k \quad (k \in \mathbb{Z})
$$

**Radian measure:** angle (radians) = arc length / radius. On the unit circle (radius $=1$), radians = arc length.

### Trigonometric Definitions

For the intersection point $P$ on the unit circle:

$$
\sin\theta = y\text{-coordinate of } P
$$

$$
\cos\theta = x\text{-coordinate of } P
$$

$$
\tan\theta = \frac{\sin\theta}{\cos\theta} = \text{slope of terminal ray (when } \cos\theta \neq 0\text{)}
$$

### Example

> **Example 2:** Find $\sin\frac{\pi}{6}$, $\cos\frac{\pi}{6}$, and $\tan\frac{\pi}{6}$.

On the unit circle, $\theta = \frac{\pi}{6}$ corresponds to $P\left(\frac{\sqrt{3}}{2}, \frac{1}{2}\right)$

$$
\sin\frac{\pi}{6} = \frac{1}{2},\quad \cos\frac{\pi}{6} = \frac{\sqrt{3}}{2},\quad \tan\frac{\pi}{6} = \frac{1/2}{\sqrt{3}/2} = \frac{1}{\sqrt{3}} = \frac{\sqrt{3}}{3}
$$

---

## 🔹 3.3 — Sine and Cosine Function Values

### Coordinates on a Circle

Given a circle of radius $r$ and an angle $\theta$ in standard position, the intersection point $P$ of the terminal ray with the circle is:

$$
P = (r\cos\theta,\; r\sin\theta)
$$

### Exact Values for Special Angles

Use the isosceles right triangle ($45^\circ = \frac{\pi}{4}$) and the equilateral triangle ($30^\circ = \frac{\pi}{6}$, $60^\circ = \frac{\pi}{3}$), together with quadrant signs.

| $\theta$ | $\sin\theta$ | $\cos\theta$ | $\tan\theta$ |
|:--------:|:------------:|:------------:|:------------:|
| $0$ | $0$ | $1$ | $0$ |
| $\frac{\pi}{6}$ | $\frac{1}{2}$ | $\frac{\sqrt{3}}{2}$ | $\frac{\sqrt{3}}{3}$ |
| $\frac{\pi}{4}$ | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{2}}{2}$ | $1$ |
| $\frac{\pi}{3}$ | $\frac{\sqrt{3}}{2}$ | $\frac{1}{2}$ | $\sqrt{3}$ |
| $\frac{\pi}{2}$ | $1$ | $0$ | undefined (vertical asymptote) |

> **Example 3:** Find $\sin\frac{5\pi}{4}$.

$\frac{5\pi}{4}$ has its terminal side in the third quadrant, reference angle $\frac{\pi}{4}$. In QIII, $\sin$ is negative.

$$
\sin\frac{5\pi}{4} = -\sin\frac{\pi}{4} = -\frac{\sqrt{2}}{2}
$$

---

## 🔹 3.4 — Sine and Cosine Function Graphs

### Sine function $f(\theta) = \sin\theta$

- **Domain:** $\mathbb{R}$ (all real numbers)
- **Range:** $[-1, 1]$
- Gives the $y$-coordinate (vertical displacement) of point $P$ on the unit circle
- As $\theta$ increases, $\sin\theta$ oscillates between $-1$ and $1$

### Cosine function $g(\theta) = \cos\theta$

- **Domain:** $\mathbb{R}$ (all real numbers)
- **Range:** $[-1, 1]$
- Gives the $x$-coordinate (horizontal displacement) of point $P$ on the unit circle
- As $\theta$ increases, $\cos\theta$ oscillates between $-1$ and $1$

### Graph Symmetry

- $y = \sin\theta$: **odd function**, symmetric about the origin ($\sin(-\theta) = -\sin\theta$)
- $y = \cos\theta$: **even function**, symmetric about the $y$-axis ($\cos(-\theta) = \cos\theta$)
- Both have period $2\pi$

---

## 🔹 3.5 — Sinusoidal Functions

### Definition

A **sinusoidal function** is any function obtained by applying additive and multiplicative transformations to $f(\theta) = \sin\theta$. Both sine and cosine are sinusoidal, and they can be converted via a phase shift:

$$
\cos\theta = \sin\left(\theta + \frac{\pi}{2}\right)
$$

### Key Features

**Period** and **frequency** are reciprocals:

$$
\text{Period} = 2\pi,\qquad \text{Frequency} = \frac{1}{2\pi}
$$

**Amplitude** is half the difference between maximum and minimum:

$$
\text{Amplitude} = \frac{\text{max} - \text{min}}{2}
$$

For $f(\theta) = \sin\theta$ and $g(\theta) = \cos\theta$, amplitude $=1$.

**Midline** is the average of maximum and minimum:

$$
\text{Midline: } y = \frac{\text{max} + \text{min}}{2}
$$

For $y = \sin\theta$ and $y = \cos\theta$, midline is $y = 0$.

**Symmetry:**
- $y = \sin\theta$: **odd** ($\sin(-\theta) = -\sin\theta$)
- $y = \cos\theta$: **even** ($\cos(-\theta) = \cos\theta$)

---

## 🔹 3.6 — Sinusoidal Function Transformations

### General Form (Standard Notation)

The most common standard form is:

$$
f(\theta) = a\sin(b\theta - c) + d
$$

$$
g(\theta) = a\cos(b\theta - c) + d
$$

where $a, b, c, d$ are real numbers, $a \neq 0$, $b \neq 0$.

### Role of Each Parameter

| Parameter | Transformation | Effect |
|:---------:|:--------------|:-------|
| $a$ | Vertical stretch/compression | **Amplitude** $= |a|$; if $a < 0$, reflect over $x$-axis |
| $b$ | Horizontal stretch/compression | **Period** $= \dfrac{2\pi}{|b|}$ |
| $c$ | Horizontal shift | **Phase shift** $= \dfrac{c}{b}$ (right if $\dfrac{c}{b} > 0$) |
| $d$ | Vertical shift | **Midline** $y = d$ |

### Complete Formula Summary

$$
\text{Amplitude} = |a|,\quad \text{Period} = \frac{2\pi}{|b|},\quad \text{Phase shift} = \frac{c}{b},\quad \text{Midline: } y = d
$$

> **Note:** If you encounter the form $f(\theta) = a\sin\bigl(b(\theta + c)\bigr) + d$, then the phase shift is $-c$. This document uses $f(\theta) = a\sin(b\theta - c) + d$, which makes the phase shift directly $c/b$.

### Example

> **Example 4:** Find the amplitude, period, phase shift, and midline of $f(x) = 3\sin(2x - \pi) + 1$.

$$
a = 3,\; b = 2,\; c = \pi,\; d = 1
$$

$$
\text{Amplitude} = |3| = 3,\quad \text{Period} = \frac{2\pi}{2} = \pi,\quad \text{Phase shift} = \frac{\pi}{2} \text{ (right)},\quad \text{Midline: } y = 1
$$

---

## 🔹 3.7 — Sinusoidal Function Context and Data Modeling

### Modeling Steps

1. **Determine the period:** horizontal distance between consecutive maxima (or minima)
2. **Compute amplitude and vertical shift:**

   $$
   \text{Amplitude} = \frac{\text{max} - \text{min}}{2},\qquad \text{Vertical shift} = \frac{\text{max} + \text{min}}{2}
   $$

3. **Find the phase shift:** compare actual data points to a standard sine/cosine curve
4. **Use technology:** sinusoidal regression on a calculator
5. **Predict:** interpolate and extrapolate only within the context‑appropriate domain

> **Example 5:** The highest temperature in a year is $30^\circ\text{C}$ (July), the lowest is $10^\circ\text{C}$ (January), period 12 months. Build a sinusoidal model.

$$
\text{Amplitude} = \frac{30-10}{2} = 10,\quad \text{Midline} = \frac{30+10}{2} = 20,\quad b = \frac{2\pi}{12} = \frac{\pi}{6}
$$

Assume July corresponds to $t=6$ (starting from January). Use a cosine model:

$$
T(t) = 10\cos\left(\frac{\pi}{6}(t - 6)\right) + 20
$$

---

## 🔹 3.8 — The Tangent Function

### Definition

$\tan\theta$ represents the slope of the terminal ray:

$$
\tan\theta = \frac{\sin\theta}{\cos\theta},\quad \cos\theta \neq 0
$$

### Key Features

- **Period:** $\pi$ (slope repeats every half‑circle)
- **Vertical asymptotes:** where $\cos\theta = 0$, i.e., $\theta = \frac{\pi}{2} + k\pi,\; k\in\mathbb{Z}$
- Between consecutive asymptotes: $\tan$ increases from $-\infty$ to $+\infty$, the graph changes from concave down to concave up
- **Domain:** $\theta \neq \frac{\pi}{2} + k\pi,\; k\in\mathbb{Z}$

### Transformed Form

$$
f(\theta) = a\tan(b\theta - c) + d
$$

- Vertical stretch factor $|a|$; if $a < 0$, reflect over $x$-axis, and the function **decreases** on each period
- **Period** $= \dfrac{\pi}{|b|}$
- **Phase shift** $= \dfrac{c}{b}$
- Vertical shift $d$ (the inflection line becomes $y = d$)

---

## 🔹 3.9 — Inverse Trigonometric Functions

### Definition

Inverse trigonometric functions swap the input and output of the corresponding trig functions:
- **Input:** a number (from the range of the original trig function)
- **Output:** an angle

### Common Notation

$$
\arcsin x = \sin^{-1} x,\quad \arccos x = \cos^{-1} x,\quad \arctan x = \tan^{-1} x
$$

### Domain Restrictions (to make them invertible)

| Function | Domain (input) | Range (output) |
|:--------:|:--------------:|:---------------:|
| $\sin^{-1} x$ | $[-1, 1]$ | $\left[-\dfrac{\pi}{2},\; \dfrac{\pi}{2}\right]$ |
| $\cos^{-1} x$ | $[-1, 1]$ | $[0,\; \pi]$ |
| $\tan^{-1} x$ | $\mathbb{R}$ | $\left(-\dfrac{\pi}{2},\; \dfrac{\pi}{2}\right)$ |

> **Note:** $\arctan x$ has **horizontal asymptotes** $y = \dfrac{\pi}{2}$ and $y = -\dfrac{\pi}{2}$: as $x \to +\infty$, $\arctan x \to \dfrac{\pi}{2}$; as $x \to -\infty$, $\arctan x \to -\dfrac{\pi}{2}$.

### Example

> **Example 6:** Find $\sin^{-1}\left(\frac{1}{2}\right)$.

Because $\sin\frac{\pi}{6} = \frac{1}{2}$ and $\frac{\pi}{6} \in \left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$:

$$
\sin^{-1}\left(\frac{1}{2}\right) = \frac{\pi}{6}
$$

---

## 🔹 3.10 — Trigonometric Equations and Inequalities

### Solving Trigonometric Equations

1. Use inverse trig functions to find a **principal solution**
2. Because trig functions are **periodic**, there are usually infinitely many solutions
3. If the problem restricts the domain (e.g., $[0, 2\pi)$), find all solutions within that interval
4. Remember that the inverse function gives only **one** value; you must find additional solutions using quadrant analysis

> **Example 7a:** Solve $\sin\theta = \frac{\sqrt{2}}{2}$ on $[0, 2\pi)$.

Principal solution: $\theta = \frac{\pi}{4}$. Since sine is also positive in QII, another solution is $\pi - \frac{\pi}{4} = \frac{3\pi}{4}$.

$$
\theta = \frac{\pi}{4},\; \frac{3\pi}{4}
$$

> **Example 7b:** Solve $\cos\theta = -\frac{1}{2}$ on $[0, 2\pi)$.

Principal value (from $\cos^{-1}$): $\frac{2\pi}{3}$. Cosine is also negative in QIII, so $2\pi - \frac{2\pi}{3} = \frac{4\pi}{3}$.

$$
\theta = \frac{2\pi}{3},\; \frac{4\pi}{3}
$$

### Solving Trigonometric Inequalities

Use the **unit circle** or **function graphs**.

> **Example 7c:** Solve $\sin\theta > \frac{1}{2}$ on $[0, 2\pi)$.

**Steps:**
1. Find equality solutions: $\sin\theta = \frac{1}{2}$ gives $\theta = \frac{\pi}{6}$ and $\frac{5\pi}{6}$.
2. On the unit circle, $\sin\theta > \frac{1}{2}$ corresponds to $y$-coordinate $> \frac{1}{2}$.
3. On $[0, 2\pi)$, the solution is $\left(\frac{\pi}{6},\; \frac{5\pi}{6}\right)$.
4. For all real numbers, add periodicity: $\left(\frac{\pi}{6} + 2\pi k,\; \frac{5\pi}{6} + 2\pi k\right),\; k \in \mathbb{Z}$.

> **Example 7d:** Solve $\cos\theta \le -\frac{1}{2}$ on $[0, 2\pi)$.

1. Equality: $\cos\theta = -\frac{1}{2}$ at $\theta = \frac{2\pi}{3}$ and $\frac{4\pi}{3}$.
2. $\cos\theta \le -\frac{1}{2}$ means $x$-coordinate $\le -\frac{1}{2}$.
3. Solution on $[0, 2\pi)$: $\left[\frac{2\pi}{3},\; \frac{4\pi}{3}\right]$.

### Important Principles

- For inequalities, first find the solution set on one fundamental period (e.g., $[0, 2\pi)$ or $[0, \pi)$ for tangent), then extend using periodicity.
- For $\tan$ inequalities, work on $(-\pi/2, \pi/2)$ and then add $k\pi$.

---

## 🔹 3.11 — The Secant, Cosecant, and Cotangent Functions

### Definitions

**Secant:**

$$
\sec\theta = \frac{1}{\cos\theta},\quad \cos\theta \neq 0
$$

**Cosecant:**

$$
\csc\theta = \frac{1}{\sin\theta},\quad \sin\theta \neq 0
$$

**Cotangent:**

$$
\cot\theta = \frac{1}{\tan\theta} = \frac{\cos\theta}{\sin\theta},\quad \sin\theta \neq 0
$$

### Key Features

| Function | Domain restrictions | Vertical asymptotes | Range | Period |
|:--------:|:-------------------:|:-------------------:|:-----:|:------:|
| $\sec\theta$ | $\cos\theta \neq 0$ | $\theta = \frac{\pi}{2} + k\pi$ | $(-\infty, -1] \cup [1, \infty)$ | $2\pi$ |
| $\csc\theta$ | $\sin\theta \neq 0$ | $\theta = k\pi$ | $(-\infty, -1] \cup [1, \infty)$ | $2\pi$ |
| $\cot\theta$ | $\sin\theta \neq 0$ | $\theta = k\pi$ | $\mathbb{R}$ (decreasing between asymptotes) | $\pi$ |

> **Note:** $\sec\theta$ and $\csc\theta$ never take values in $(-1, 1)$; their graphs are U‑shaped curves obtained by taking reciprocals of the cosine and sine graphs.

---

## 🔹 3.12 — Equivalent Representations of Trigonometric Functions

### Pythagorean Identities

From the unit circle (Pythagorean theorem):

$$
\sin^2\theta + \cos^2\theta = 1
$$

**Common variations:**

$$
\tan^2\theta + 1 = \sec^2\theta \quad\Longrightarrow\quad \tan^2\theta = \sec^2\theta - 1
$$

$$
\cot^2\theta + 1 = \csc^2\theta \quad\Longrightarrow\quad \cot^2\theta = \csc^2\theta - 1
$$

### Sum Identities

**Sine sum:**

$$
\sin(\alpha + \beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta
$$

**Cosine sum:**

$$
\cos(\alpha + \beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta
$$

### Difference Identities

$$
\sin(\alpha - \beta) = \sin\alpha\cos\beta - \cos\alpha\sin\beta
$$

$$
\cos(\alpha - \beta) = \cos\alpha\cos\beta + \sin\alpha\sin\beta
$$

### Double‑Angle Identities

Set $\alpha = \beta = \theta$:

$$
\sin(2\theta) = 2\sin\theta\cos\theta
$$

$$
\cos(2\theta) = \cos^2\theta - \sin^2\theta = 1 - 2\sin^2\theta = 2\cos^2\theta - 1
$$

### Example

> **Example 8:** Use a sum identity to find $\sin\frac{7\pi}{12}$.

$$
\frac{7\pi}{12} = \frac{\pi}{3} + \frac{\pi}{4}
$$

$$
\sin\frac{7\pi}{12} = \sin\left(\frac{\pi}{3} + \frac{\pi}{4}\right) = \sin\frac{\pi}{3}\cos\frac{\pi}{4} + \cos\frac{\pi}{3}\sin\frac{\pi}{4}
$$

$$
= \frac{\sqrt{3}}{2} \cdot \frac{\sqrt{2}}{2} + \frac{1}{2} \cdot \frac{\sqrt{2}}{2} = \frac{\sqrt{6} + \sqrt{2}}{4}
$$

---

## 🔹 3.13 — Trigonometry and Polar Coordinates

### Polar Coordinate System

A point is represented by an ordered pair $(r, \theta)$:
- $r$ = distance from the origin (radius, usually $r \ge 0$)
- $\theta$ = angle from the positive $x$-axis to the ray through the point

The same point can have multiple polar representations (e.g., $(r, \theta)$ and $(-r, \theta + \pi)$).

### Conversion Between Polar and Rectangular Coordinates

**Polar → Rectangular:**

$$
\begin{cases}
x = r\cos\theta \\[4pt]
y = r\sin\theta
\end{cases}
$$

**Rectangular → Polar:**

$$
\begin{cases}
r = \sqrt{x^2 + y^2} \\[6pt]
\theta =
\begin{cases}
\arctan\dfrac{y}{x}, & x > 0 \\[8pt]
\arctan\dfrac{y}{x} + \pi, & x < 0 \\[8pt]
\dfrac{\pi}{2}, & x = 0,\; y > 0 \\[8pt]
-\dfrac{\pi}{2}\;\left(\text{or } \dfrac{3\pi}{2}\right), & x = 0,\; y < 0
\end{cases}
\end{cases}
$$

> The piecewise definition for $\theta$ is equivalent to the $\operatorname{atan2}(y, x)$ function.

### Complex Numbers in Polar Form

A complex number $a + bi$ in polar form (modulus‑argument form):

$$
a + bi = r(\cos\theta + i\sin\theta),\quad \text{where } r = \sqrt{a^2 + b^2},\; \theta = \operatorname{atan2}(b, a)
$$

### Example

> **Example 9:** Convert $(x, y) = (1, \sqrt{3})$ to polar coordinates.

$$
r = \sqrt{1^2 + (\sqrt{3})^2} = \sqrt{4} = 2
$$

$$
\theta = \arctan\frac{\sqrt{3}}{1} = \frac{\pi}{3}\quad (\text{since } x > 0)
$$

Polar coordinates: $\left(2,\; \dfrac{\pi}{3}\right)$.

---

## 🔹 3.14 — Polar Function Graphs

### Polar Function $r = f(\theta)$

A polar function maps an input angle $\theta$ to an output radius $r$.

- **Input:** angle $\theta$
- **Output:** radius $r$

### Graph Features

- Changing the input rotates the ray from the positive $x$-axis.
- Changing the output changes the distance from the origin.
- Restricting the domain of $\theta$ yields only part of the curve.

### Common Polar Curves

| Type | Example form | Graph description |
|:----:|:-------------|:------------------|
| **Circle** | $r = a$ | Circle of radius $|a|$ centered at the origin |
| **Rose** | $r = a\sin(n\theta)$ or $r = a\cos(n\theta)$ | $n$ petals if $n$ is odd, $2n$ petals if $n$ is even |
| **Cardioid** | $r = a(1 \pm \sin\theta)$ or $r = a(1 \pm \cos\theta)$ | Heart‑shaped |
| **Line** | $\theta = \alpha$ | Ray from the origin at angle $\alpha$ |

---

## 🔹 3.15 — Rates of Change in Polar Functions

### Analyzing Distance from the Origin

For $r = f(\theta)$:

| Sign of $f(\theta)$ | Monotonicity | Distance from origin |
|:-------------------:|:------------:|:--------------------:|
| $> 0$ | Increasing | **Increasing** |
| $< 0$ | Decreasing | **Increasing** |
| $> 0$ | Decreasing | **Decreasing** |
| $< 0$ | Increasing | **Decreasing** |

If $f$ changes from increasing to decreasing (or vice versa) on an interval, there is an **extremum** (closest or farthest point from the origin).

### Average Rate of Change

The **average rate of change** of $r$ with respect to $\theta$ on $[\theta_1, \theta_2]$ is:

$$
\frac{\Delta r}{\Delta \theta} = \frac{f(\theta_2) - f(\theta_1)}{\theta_2 - \theta_1}
$$

- **Geometric meaning:** The average amount $r$ changes per radian increase in $\theta$ (units: radius per radian)
- Can be used to estimate values of $r$ within the interval.

### Example

> **Example 10:** For the polar function $r = 2 + 3\sin\theta$, find the average rate of change of $r$ as $\theta$ goes from $0$ to $\dfrac{\pi}{2}$.

$$
f(0) = 2 + 3\sin(0) = 2,\qquad f\left(\frac{\pi}{2}\right) = 2 + 3\sin\left(\frac{\pi}{2}\right) = 2 + 3 = 5
$$

$$
\text{Average rate of change} = \frac{5 - 2}{\frac{\pi}{2} - 0} = \frac{3}{\frac{\pi}{2}} = \frac{6}{\pi} \approx 1.91
$$

This means that over this interval, for each additional radian, the radius increases by about $1.91$ units on average.

---

## 📋 Unit 3 Core Formula Quick Reference

### Basic Definitions

$$
\sin\theta = y,\quad \cos\theta = x,\quad \tan\theta = \frac{y}{x} = \frac{\sin\theta}{\cos\theta}
$$

### Sinusoidal Function (Standard Form)

$$
f(\theta) = a\sin(b\theta - c) + d \quad\text{or}\quad f(\theta) = a\cos(b\theta - c) + d
$$

$$
\text{Amplitude} = |a|,\quad \text{Period} = \frac{2\pi}{|b|},\quad \text{Phase shift} = \frac{c}{b},\quad \text{Midline } y = d
$$

### Tangent Function

$$
\tan\theta = \frac{\sin\theta}{\cos\theta},\quad \text{Period} = \pi
$$

$$
f(\theta) = a\tan(b\theta - c) + d,\quad \text{Period} = \frac{\pi}{|b|}
$$

### Reciprocal Trigonometric Functions

$$
\sec\theta = \frac{1}{\cos\theta},\quad \csc\theta = \frac{1}{\sin\theta},\quad \cot\theta = \frac{\cos\theta}{\sin\theta}
$$

### Pythagorean Identities

$$
\sin^2\theta + \cos^2\theta = 1,\quad \tan^2\theta + 1 = \sec^2\theta,\quad \cot^2\theta + 1 = \csc^2\theta
$$

### Sum / Difference / Double‑Angle Identities

$$
\sin(\alpha \pm \beta) = \sin\alpha\cos\beta \pm \cos\alpha\sin\beta
$$

$$
\cos(\alpha \pm \beta) = \cos\alpha\cos\beta \mp \sin\alpha\sin\beta
$$

$$
\sin(2\theta) = 2\sin\theta\cos\theta,\quad \cos(2\theta) = \cos^2\theta - \sin^2\theta
$$

### Polar ↔ Rectangular Conversion

$$
\begin{cases}
x = r\cos\theta \\[2pt]
y = r\sin\theta
\end{cases}
\qquad
\begin{cases}
r = \sqrt{x^2 + y^2} \\[2pt]
\theta = \operatorname{atan2}(y, x)
\end{cases}
$$

### Average Rate of Change (Polar Function)

$$
\frac{\Delta r}{\Delta \theta} = \frac{f(\theta_2) - f(\theta_1)}{\theta_2 - \theta_1}
$$

---

> **Summary:** Unit 3 starts with **periodic phenomena**, introduces trigonometric functions via the **unit circle**, explores **sinusoidal function transformations and modeling**, then extends to **tangent**, **reciprocal functions**, **trigonometric identities**, **inverse functions**, and **trigonometric equations & inequalities**. Finally, it moves into the **polar coordinate system**, bridging rectangular and polar representations. Mastering this unit covers approximately $30$–$35\%$ of the AP Precalculus exam. 🎯
