# 📦 UNIT 4: Functions Involving Parameters, Vectors, and Matrices

> **⚠️ Important Note**: Unit 4 consists of **Additional Topics Available to Schools**, and is **NOT assessed on the AP Exam**. Schools may decide whether to teach it based on local requirements.

---

## 🔷 4.1 — Parametric Functions

### Core Concept

A **parametric function** maps an input (the parameter $t$) to an output ordered pair:

$$f(t) = (x(t),\; y(t))$$

- $x(t)$ and $y(t)$ are two **independent** functions of $t$
- $t$ is the parameter (often representing time)
- The graph is **traced out** by all points $(x(t), y(t))$ in order of increasing $t$ (not connected by straight line segments, but a curve formed by the set of points)

### Generating a Numerical Table

Given parameter values $t_i$ within the domain, a numerical table can be generated:

$$(x_i, y_i) = (x(t_i),\; y(t_i))$$

### Domain and Graph

$$\text{domain}(f) = \{t \in \mathbb{R} \mid t \text{ is meaningful}\}$$

- The domain is often restricted, resulting in start and end points on the graph
- The graph of a parametric function **may fail the vertical line test**, yet it is still a function (because each $t$ uniquely determines an $(x,y)$ pair)

### 📌 Example

> **Example**: Given $f(t) = (t^2,\; t+1)$, $t \in [0, 3]$
>
> | $t$ | $(x(t), y(t))$ |
> |:---:|:--------------:|
> | $0$ | $(0, 1)$ |
> | $1$ | $(1, 2)$ |
> | $2$ | $(4, 3)$ |
> | $3$ | $(9, 4)$ |
>
> These points trace out a parabolic arc in order of increasing $t$.

---

## 🔷 4.2 — Parametric Functions Modeling Planar Motion

### Core Concept

Parametric functions can be used to model the **motion of a particle in the plane**:

$$f(t) = (x(t),\; y(t))$$

- The graph represents the **position** of the particle at time $t$
- $x(t)$: horizontal position component; $y(t)$: vertical position component

### Key Features

| Feature | Method |
|---------|--------|
| Horizontal extrema | Max/min values of $x(t)$ |
| Vertical extrema | Max/min values of $y(t)$ |
| $x$-intercept(s) | Solve $y(t)=0$ for $t$, then substitute into $x(t)$ to get the $x$-coordinate |
| $y$-intercept(s) | Solve $x(t)=0$ for $t$, then substitute into $y(t)$ to get the $y$-coordinate |

### 📌 Example

> **Example**: $f(t) = (\cos t,\; \sin t)$, $t \in [0, 2\pi]$
>
> - $x(t)$ max $= 1$ (at $t=0$), min $= -1$ (at $t=\pi$)
> - $y(t)$ max $= 1$ (at $t=\frac{\pi}{2}$), min $= -1$ (at $t=\frac{3\pi}{2}$)
> - $x$-intercept: $y(t)=0 \Rightarrow \sin t = 0 \Rightarrow t=0,\pi,2\pi$, giving points $(1,0)$ and $(-1,0)$
> - $y$-intercept: $x(t)=0 \Rightarrow \cos t = 0 \Rightarrow t=\frac{\pi}{2},\frac{3\pi}{2}$, giving points $(0,1)$ and $(0,-1)$

---

## 🔷 4.3 — Parametric Functions and Rates of Change

### Direction of Motion Analysis

As the parameter $t$ increases, the direction of the particle's motion is determined by the monotonicity of $x(t)$ and $y(t)$:

$$
\begin{aligned}
x(t) \text{ increases as } t \text{ increases} &\Rightarrow \text{moving right} \\
x(t) \text{ decreases as } t \text{ increases} &\Rightarrow \text{moving left} \\
y(t) \text{ increases as } t \text{ increases} &\Rightarrow \text{moving up} \\
y(t) \text{ decreases as } t \text{ increases} &\Rightarrow \text{moving down}
\end{aligned}
$$

### Average Rate of Change

On the interval $[t_1, t_2]$:

$$\text{AROC}_x = \frac{x(t_2) - x(t_1)}{t_2 - t_1}$$

$$\text{AROC}_y = \frac{y(t_2) - y(t_1)}{t_2 - t_1}$$

**Slope of the curve** (when $\text{AROC}_x \neq 0$):

$$\text{slope} = \frac{y(t_2) - y(t_1)}{x(t_2) - x(t_1)} = \frac{\text{AROC}_y}{\text{AROC}_x}$$

### Different Parametrizations of the Same Curve

The same planar curve can be traversed in different directions and at different speeds using different parametric functions.

### 📌 Example

> **Example**: $f(t) = (t,\; t^2)$, $t \in [0, 2]$
>
> On $[0, 2]$: $x(t)$ increases from $0$ to $2$ (moving right), $y(t)$ increases from $0$ to $4$ (moving up), so the particle moves up and to the right.
>
> Average rates of change: $\text{AROC}_x = \frac{2-0}{2-0}=1$, $\text{AROC}_y = \frac{4-0}{2-0}=2$
>
> Curve slope $= \frac{2}{1}=2$

---

## 🔷 4.4 — Parametrically Defined Circles and Lines

### Unit Circle (Counterclockwise)

Starting at $(1,0)$, one full counterclockwise revolution around the origin:

$$(x(t),\; y(t)) = (\cos t,\; \sin t), \quad 0 \leq t \leq 2\pi$$

### Arbitrary Circle/Ellipse (After Transformations)

Transformations can produce circles or ellipses with any center and radii:

$$(x(t),\; y(t)) = (h + a\cos t,\; k + b\sin t)$$

- $(h, k)$: center
- $a > 0$: horizontal semi-axis length; $b > 0$: vertical semi-axis length
- If $a = b$, it is a circle; if $a \neq b$, it is an ellipse

### Parametrization of a Line Segment

The line segment from $(x_1, y_1)$ to $(x_2, y_2)$:

$$(x(t),\; y(t)) = (x_1 + \Delta x \cdot t,\; y_1 + \Delta y \cdot t), \quad t \in [0,1]$$

where $\Delta x = x_2 - x_1$, $\Delta y = y_2 - y_1$.

More generally:

$$(x(t),\; y(t)) = (x_1 + v_x t,\; y_1 + v_y t)$$

where $v_x$ and $v_y$ are the rates of change of $x$ and $y$ with respect to $t$.

### 📌 Example

> **Example**: Write the parametric equation of a circle centered at $(2, -1)$ with radius $3$.
>
> $$(x(t), y(t)) = (2 + 3\cos t,\; -1 + 3\sin t), \quad 0 \leq t \leq 2\pi$$
>
> **Example**: Parametrize the line segment from $(1,2)$ to $(5,6)$.
>
> $$(x(t), y(t)) = (1 + 4t,\; 2 + 4t), \quad 0 \leq t \leq 1$$

---

## 🔷 4.5 — Implicitly Defined Functions

### Core Concept

An equation involving two variables can implicitly define one or more functions:

$$F(x, y) = 0$$

### Solving for Explicit Form

Solving the equation for one of the variables yields an explicit function:

$$y = f(x) \quad \text{or} \quad x = g(y)$$

The graph of the solved function is part of or all of the graph of the original equation.

### Covariation Analysis

For nearby ordered pairs on the graph of an implicitly defined function (when the change in $x$ is small):

$$ \frac{\Delta y}{\Delta x} > 0 \Rightarrow x \text{ and } y \text{ both increase or both decrease} $$

$$ \frac{\Delta y}{\Delta x} < 0 \Rightarrow \text{as } x \text{ increases, } y \text{ decreases (or vice versa)} $$

$$ \frac{\Delta y}{\Delta x} = 0 \Rightarrow \text{horizontal interval} $$

$$ \frac{\Delta x}{\Delta y} = 0 \Rightarrow \text{vertical interval} $$

### 📌 Example

> **Example**: $x^2 + y^2 = 25$
>
> Solving for $y$: $y = \pm\sqrt{25 - x^2}$, domain $x \in [-5, 5]$
>
> This defines **two** functions (the upper and lower semicircles).
>
> Near the point $(3,4)$: as $x$ increases, $y$ decreases ($\frac{\Delta y}{\Delta x} < 0$).

---

## 🔷 4.6 — Conic Sections

### Parabola

Vertex at $(h, k)$, $a \neq 0$:

**Opening up/down**:

$$y - k = a(x - h)^2$$

- $a > 0$: opens upward
- $a < 0$: opens downward

**Opening left/right**:

$$x - h = a(y - k)^2$$

- $a > 0$: opens to the right
- $a < 0$: opens to the left

### Ellipse

Center at $(h, k)$, horizontal radius $a > 0$, vertical radius $b > 0$:

$$\frac{(x - h)^2}{a^2} + \frac{(y - k)^2}{b^2} = 1$$

- When $a = b$, the ellipse degenerates into a **circle**
- $a$: horizontal semi-axis length; $b$: vertical semi-axis length

### Hyperbola

Center at $(h, k)$, $a > 0$, $b > 0$:

**Opening left and right**:

$$\frac{(x - h)^2}{a^2} - \frac{(y - k)^2}{b^2} = 1$$

- $a$: length of the transverse semi-axis (distance from center to vertex)
- $b$: length of the conjugate semi-axis

*Asymptotes*: $y - k = \pm\frac{b}{a}(x - h)$

**Opening up and down**:

$$\frac{(y - k)^2}{a^2} - \frac{(x - h)^2}{b^2} = 1$$

- $a$: length of the transverse semi-axis (distance from center to vertex)
- $b$: length of the conjugate semi-axis

*Asymptotes*: $y - k = \pm\frac{a}{b}(x - h)$

### 📌 Example

> **Example**: Identify the graph of $\frac{(x-1)^2}{4} + \frac{(y+2)^2}{9} = 1$.
>
> This is an ellipse, center $(1,-2)$, $a=2$ (horizontal radius), $b=3$ (vertical radius).
>
> **Example**: What is $y - 3 = 2(x + 1)^2$?
>
> This is a parabola, vertex $(-1, 3)$, opening upward.

---

## 🔷 4.7 — Parametrization of Implicitly Defined Functions

### Core Idea

A parametrization $(x(t), y(t))$ satisfies an implicit equation: substituting $x(t)$ and $y(t)$ into the equation holds true for every value of $t$ in the domain.

### Parametrization of Explicit Functions

If $y = f(x)$, it can be parametrized as:

$$(x(t), y(t)) = (t,\; f(t))$$

If $f$ is invertible, its inverse can be parametrized as:

$$(x(t), y(t)) = (f(t),\; t)$$

### Parametrization of Conic Sections

**Ellipse** (center $(h,k)$, radii $a>0, b>0$):

$$(x(t), y(t)) = (h + a\cos t,\; k + b\sin t), \quad 0 \leq t \leq 2\pi$$

**Hyperbola** (opening left and right, center $(h,k)$, $a>0, b>0$):

$$(x(t), y(t)) = (h + a\sec t,\; k + b\tan t), \quad 0 \leq t \leq 2\pi,\; t \neq \frac{\pi}{2}, \frac{3\pi}{2}$$

> ⚠️ Note: $\sec t$ and $\tan t$ are undefined at $t = \frac{\pi}{2}$ and $t = \frac{3\pi}{2}$; these points must be excluded.

**Hyperbola** (opening up and down, center $(h,k)$, $a>0, b>0$):

$$(x(t), y(t)) = (h + a\tan t,\; k + b\sec t), \quad 0 \leq t \leq 2\pi,\; t \neq \frac{\pi}{2}, \frac{3\pi}{2}$$

### 📌 Example

> **Example**: Parametrize $y = x^2$, $x \in [-2, 2]$
>
> $$(x(t), y(t)) = (t,\; t^2), \quad -2 \leq t \leq 2$$
>
> **Example**: Parametrize $\frac{x^2}{9} + \frac{y^2}{4} = 1$
>
> $$(x(t), y(t)) = (3\cos t,\; 2\sin t), \quad 0 \leq t \leq 2\pi$$

---

## 🔷 4.8 — Vectors

### Vector Definition

A vector is a **directed line segment**. In the plane:

$$\overrightarrow{P_1P_2} = \langle a, b \rangle$$

where $a = x_2 - x_1$, $b = y_2 - y_1$.

- **Tail**: $P_1$; **Head**: $P_2$
- **Zero vector**: $\langle 0, 0 \rangle$

### Magnitude

$$|\vec{v}| = \sqrt{a^2 + b^2}$$

### Scalar Multiplication

$$k \cdot \langle a, b \rangle = \langle ka, kb \rangle$$

The resulting vector is parallel to the original vector.

### Vector Addition

$$\langle a_1, b_1 \rangle + \langle a_2, b_2 \rangle = \langle a_1 + a_2, \; b_1 + b_2 \rangle$$

Graphically: the triangle rule (head-to-tail).

### Dot Product

$$\langle a_1, b_1 \rangle \cdot \langle a_2, b_2 \rangle = a_1a_2 + b_1b_2$$

**Geometric Interpretation**:

$$\vec{u} \cdot \vec{v} = |\vec{u}|\,|\vec{v}|\cos\theta$$

where $\theta \in [0, \pi]$ is the angle between the two vectors.

**Perpendicularity Condition**: If the dot product of two nonzero vectors is zero, then $\vec{u} \perp \vec{v}$.

### Unit Vector

A vector with magnitude $1$. The unit vector in the same direction as $\vec{v}$:

$$\hat{v} = \frac{\vec{v}}{|\vec{v}|}$$

### Basis Vector Representation

$$\langle a, b \rangle = a\hat{i} + b\hat{j}$$

where $\hat{i} = \langle 1, 0 \rangle$, $\hat{j} = \langle 0, 1 \rangle$.

### Law of Sines and Law of Cosines

Triangles formed by vector addition can be solved using the **Law of Sines** and the **Law of Cosines**.

### 📌 Example

> **Example**: $\vec{u} = \langle 3, 4 \rangle$, $\vec{v} = \langle 1, -2 \rangle$
>
> $|\vec{u}| = \sqrt{3^2 + 4^2} = 5$
>
> $|\vec{v}| = \sqrt{1^2 + (-2)^2} = \sqrt{5}$
>
> $\vec{u} + \vec{v} = \langle 4, 2 \rangle$
>
> $\vec{u} \cdot \vec{v} = 3(1) + 4(-2) = 3 - 8 = -5$
>
> $\cos\theta = \frac{-5}{5 \cdot \sqrt{5}} = -\frac{1}{\sqrt{5}}$, so $\theta > 90^\circ$

---

## 🔷 4.9 — Vector-Valued Functions

> 💡 This section involves the concept of rates of change. The rigorous definition of the **velocity vector** requires derivatives from calculus; here we introduce its meaning intuitively.

### Position Vector

The position of a particle can be expressed as a vector-valued function:

$$\vec{p}(t) = x(t)\hat{i} + y(t)\hat{j} \quad \text{or} \quad \vec{p}(t) = \langle x(t), y(t) \rangle$$

The magnitude of the position vector gives the **distance** of the particle from the origin:

$$|\vec{p}(t)| = \sqrt{[x(t)]^2 + [y(t)]^2}$$

### Velocity Vector

The velocity vector describes how position changes over time (a rigorous definition requires calculus; here we provide an intuitive understanding):

$$\vec{v}(t) \text{'s components reflect how fast and in which direction position changes}$$

- If $x(t)$ increases as $t$ increases $\Rightarrow$ moving right
- If $x(t)$ decreases as $t$ increases $\Rightarrow$ moving left
- If $y(t)$ increases as $t$ increases $\Rightarrow$ moving up
- If $y(t)$ decreases as $t$ increases $\Rightarrow$ moving down

The **magnitude** of the velocity vector gives the particle's **speed**:

$$\text{speed} = |\vec{v}(t)| = \sqrt{(\text{horizontal rate of change})^2 + (\text{vertical rate of change})^2}$$

### 📌 Example

> **Example**: $\vec{p}(t) = \langle 3\cos t, 2\sin t \rangle$
>
> At $t = \frac{\pi}{2}$: position $\vec{p}(\frac{\pi}{2}) = \langle 0, 2 \rangle$, distance from origin $= 2$
>
> At $t = 0$: $x(t)=3\cos t$ starts decreasing from $3$ (trending left), $y(t)=2\sin t$ starts increasing from $0$ (trending up)

---

## 🔷 4.10 — Matrices

### Matrix Definition

An $n \times m$ matrix is an array with $n$ rows and $m$ columns.

$$A_{n \times m} = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1m} \\ a_{21} & a_{22} & \cdots & a_{2m} \\ \vdots & \vdots & \ddots & \vdots \\ a_{n1} & a_{n2} & \cdots & a_{nm} \end{bmatrix}$$

### Matrix Multiplication

**Condition**: The number of columns in the first matrix must equal the number of rows in the second matrix.

If $A$ is $n \times p$ and $B$ is $p \times m$, then the product $C = AB$ is an $n \times m$ matrix.

$$c_{ij} = \sum_{k=1}^{p} a_{ik} \cdot b_{kj}$$

That is, $c_{ij}$ is the dot product of the $i$-th row of $A$ and the $j$-th column of $B$.

### 📌 Example

> **Example**: $A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$, $B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}$
>
> $$AB = \begin{bmatrix} 1(5)+2(7) & 1(6)+2(8) \\ 3(5)+4(7) & 3(6)+4(8) \end{bmatrix} = \begin{bmatrix} 19 & 22 \\ 43 & 50 \end{bmatrix}$$

---

## 🔷 4.11 — The Inverse and Determinant of a Matrix

### Identity Matrix

$I$ is a square matrix with $1$s on the diagonal (from top-left to bottom-right) and $0$s everywhere else:

$$I_{2\times 2} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$$

Properties: $A \cdot I = A$, $I \cdot A = A$

### Inverse Matrix

If $A^{-1}$ is the inverse of $A$, then:

$$A \cdot A^{-1} = A^{-1} \cdot A = I$$

### Inverse of a $2 \times 2$ Matrix

If $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ and $\det(A) \neq 0$:

$$A^{-1} = \frac{1}{\det(A)} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

### Determinant

For $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$:

$$\det(A) = ad - bc$$

### Geometric Interpretation of the Determinant

If the two columns (or two rows) of a $2 \times 2$ matrix are vectors in $\mathbb{R}^2$ originating from the origin, then:

$$|\det(A)| = \text{area of the parallelogram spanned by the two vectors}$$

$\det(A) = 0 \iff$ the two vectors are **parallel** (collinear, area = $0$).

### Condition for Invertibility

$$A \text{ is invertible} \iff \det(A) \neq 0$$

### 📌 Example

> **Example**: $A = \begin{bmatrix} 2 & 3 \\ 1 & 4 \end{bmatrix}$
>
> $\det(A) = 2(4) - 3(1) = 8 - 3 = 5 \neq 0$, so it is invertible.
>
> $$A^{-1} = \frac{1}{5} \begin{bmatrix} 4 & -3 \\ -1 & 2 \end{bmatrix} = \begin{bmatrix} \frac{4}{5} & -\frac{3}{5} \\ -\frac{1}{5} & \frac{2}{5} \end{bmatrix}$$

---

## 🔷 4.12 — Linear Transformations and Matrices

### Definition of a Linear Transformation

A linear transformation $L: \mathbb{R}^2 \to \mathbb{R}^2$ maps an input vector to an output vector such that each component of the output is a sum of constant multiples of the input components:

$$L\left(\begin{bmatrix} x \\ y \end{bmatrix}\right) = \begin{bmatrix} a_{11}x + a_{12}y \\ a_{21}x + a_{22}y \end{bmatrix}$$

### Zero Vector Property

$$L(\vec{0}) = \vec{0}$$

### Correspondence Between Linear Transformations and Matrices

Every linear transformation $L: \mathbb{R}^2 \to \mathbb{R}^2$ corresponds to a unique $2 \times 2$ matrix $A$:

$$L(\vec{v}) = A\vec{v}$$

Conversely, every $2 \times 2$ matrix $A$ defines a linear transformation.

### Batch Transformation

If $A$ is a $2 \times 2$ transformation matrix and $V$ is a $2 \times n$ matrix of input vectors (i.e., $n$ input vectors arranged in $2$ rows), then $AV$ is a $2 \times n$ matrix of output vectors.

### 📌 Example

> **Example**: $A = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix}$, $\vec{v} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}$
>
> $$L(\vec{v}) = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix} \begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} 2 \\ 6 \end{bmatrix}$$
>
> This represents a horizontal stretch by a factor of $2$ and a vertical stretch by a factor of $3$.

---

## 🔷 4.13 — Matrices as Functions

### Association Between Transformations and Matrices

The linear transformation $(x, y) \mapsto (a_{11}x + a_{12}y, \; a_{21}x + a_{22}y)$ is associated with the matrix:

$$\begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}$$

### Rotation Matrix

The transformation that rotates a vector counterclockwise by an angle $\theta$:

$$R_\theta = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}$$

### Mapping of Unit Vectors

The mapping of the unit vectors $\hat{i} = \langle 1, 0 \rangle$ and $\hat{j} = \langle 0, 1 \rangle$ under a linear transformation provides key information for determining the associated matrix.

### Determinant and Area Scaling

$$|\det(A)| = \text{the factor by which the transformation scales areas}$$

### Composition of Transformations

The composition of two linear transformations is itself a linear transformation. The matrix associated with the composition is the **product** of the matrices associated with each individual transformation:

$$L_2 \circ L_1 \quad \text{corresponds to matrix} \quad A_2 A_1$$

### Inverse Transformation

If $L(\vec{v}) = A\vec{v}$, then the inverse transformation is:

$$L^{-1}(\vec{v}) = A^{-1}\vec{v}$$

satisfying $L^{-1}(L(\vec{v})) = \vec{v}$.

### 📌 Example

> **Example**: The rotation matrix for $90^\circ$:
>
> $$R_{90^\circ} = \begin{bmatrix} \cos 90^\circ & -\sin 90^\circ \\ \sin 90^\circ & \cos 90^\circ \end{bmatrix} = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}$$
>
> Applied to $\vec{v} = \langle 2, 3 \rangle$:
>
> $$\begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 2 \\ 3 \end{bmatrix} = \begin{bmatrix} -3 \\ 2 \end{bmatrix}$$
>
> That is, the point $(2,3)$ rotated $90^\circ$ counterclockwise reaches $(-3,2)$.

---

## 🔷 4.14 — Matrices Modeling Contexts

### State Transition Model

A contextual scenario provides transition rates (percent changes) between states. A transition matrix can be constructed based on these rates to model how states change over discrete intervals.

### Predicting Future States

Let $M$ be the transition matrix and $\vec{s}_0$ the initial state vector. Then:

$$\vec{s}_1 = M\vec{s}_0$$

$$\vec{s}_n = M^n \vec{s}_0$$

### Steady State

After many transitions, the state distribution no longer changes:

$$M\vec{s} = \vec{s}$$

That is, $\vec{s}$ remains unchanged after one transition.

### Predicting Past States

Using the **inverse** of the transition matrix:

$$\vec{s}_{-1} = M^{-1}\vec{s}_0$$

$$\vec{s}_{-n} = M^{-n}\vec{s}_0$$

### 📌 Example

> **Example**: In a certain city, each year $10\%$ of residents move from the city center to the suburbs, and $5\%$ of residents move from the suburbs to the city center.
>
> Transition matrix (row/column 1 = city center, row/column 2 = suburbs):
>
> $$M = \begin{bmatrix} 0.90 & 0.05 \\ 0.10 & 0.95 \end{bmatrix}$$
>
> Initial state: $\vec{s}_0 = \begin{bmatrix} 1000 \\ 500 \end{bmatrix}$ (1000 in city center, 500 in suburbs)
>
> After one year:
>
> $$\vec{s}_1 = \begin{bmatrix} 0.90 & 0.05 \\ 0.10 & 0.95 \end{bmatrix} \begin{bmatrix} 1000 \\ 500 \end{bmatrix} = \begin{bmatrix} 900 + 25 \\ 100 + 475 \end{bmatrix} = \begin{bmatrix} 925 \\ 575 \end{bmatrix}$$
>
> Solving for the steady state: $M\vec{s} = \vec{s}$
>
> $$
> \begin{cases}
> 0.9s_1 + 0.05s_2 = s_1 \\
> 0.1s_1 + 0.95s_2 = s_2
> \end{cases}
> \Rightarrow
> \begin{cases}
> -0.1s_1 + 0.05s_2 = 0 \\
> 0.1s_1 - 0.05s_2 = 0
> \end{cases}
> $$
>
> Both equations are equivalent, giving $s_2 = 2s_1$. So the steady-state ratio is $s_1 : s_2 = 1 : 2$.
>
> Total population is $1500$, so at steady state: city center $= 500$, suburbs $= 1000$ ($\frac{1}{3}$ city center : $\frac{2}{3}$ suburbs).

---

## 📊 Unit 4 Quick Summary

| Topic | Name | Core Concept | Periods |
|:-----:|------|:------------:|:-------:|
| **4.1** | Parametric Functions | $f(t) = (x(t), y(t))$ | 2 |
| **4.2** | Parametric Functions Modeling Planar Motion | Position, extrema, intercepts | 2 |
| **4.3** | Parametric Functions and Rates of Change | Direction analysis, AROC, slope | 2 |
| **4.4** | Parametrically Defined Circles and Lines | Unit circle, arbitrary circle, line segment param. | 2 |
| **4.5** | Implicitly Defined Functions | $F(x,y)=0$, covariation analysis | 2 |
| **4.6** | Conic Sections | Parabola, ellipse, hyperbola equations | 3 |
| **4.7** | Parametrization of Implicitly Defined Functions | Parametrizing conic sections | 2 |
| **4.8** | Vectors | Magnitude, addition, dot product, unit vectors | 3 |
| **4.9** | Vector-Valued Functions | Position vector, velocity vector, speed | 1 |
| **4.10** | Matrices | Definition, matrix multiplication | 2 |
| **4.11** | The Inverse and Determinant of a Matrix | $\det(A)$, $A^{-1}$, geometric meaning | 2 |
| **4.12** | Linear Transformations and Matrices | $L(\vec{v}) = A\vec{v}$ | 1 |
| **4.13** | Matrices as Functions | Rotation, composition, inverse transformation | 3 |
| **4.14** | Matrices Modeling Contexts | Transition matrices, steady state | 3 |
| | **Total** | | **28 periods** |

---

> 🎯 Although **Unit 4** is not assessed on the AP Exam, it serves as a crucial bridge to **college-level linear algebra** and **multivariable calculus**! Mastering the foundations of parametrization, vectors, and matrices will lay a solid groundwork for future studies.
