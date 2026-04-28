Here is the fully corrected **Unit 2** content in English Markdown, incorporating all the fixes discussed.

---

# 📐 UNIT 2: Exponential and Logarithmic Functions — Extremely Detailed Edition (Corrected)

> **AP Exam Weighting:** $27$–$40\%$  
> **Suggested Class Periods:** $30$–$45$  
> **Core Topics:** Exponential and logarithmic functions, inverse relationships, modeling, and applications

---

## 🔢 TOPIC 2.1 — Change in Arithmetic and Geometric Sequences

### 📌 Core Concept

A **sequence** is a function from the natural numbers (usually starting at $0$ or $1$) to the real numbers, so its graph consists of **discrete points**, not a continuous curve.

> **Note:** This document uses the $0$‑th term as the starting term ($a_0$). If your textbook starts with the $1$‑st term, the formulas become $a_n = a_1 + (n-1)d$ (arithmetic) or $g_n = g_1 \cdot r^{\,n-1}$ (geometric). Both forms are equivalent.

---

### ➕ Arithmetic Sequence

**Definition:** The difference between consecutive terms is constant (the **common difference** $d$). This represents a **constant rate of change**.

**General term:**

$$a_n = a_0 + d \cdot n$$

where $a_0$ is the initial term (0‑th term) and $d$ is the common difference.

Using a known $k$‑th term:

$$a_n = a_k + d(n - k)$$

**Example:** $3, 7, 11, 15, 19, \dots$

- Common difference $d = 4$
- $a_0 = 3$
- General term: $a_n = 3 + 4n$
- 10th term: $a_{10} = 3 + 4(10) = 43$

---

### ✖️ Geometric Sequence

**Definition:** The ratio between consecutive terms is constant (the **common ratio** $r$). This represents a **constant proportional change**.

**General term:**

$$g_n = g_0 \cdot r^n$$

where $g_0$ is the initial term and $r$ is the common ratio.

Using a known $k$‑th term:

$$g_n = g_k \cdot r^{\,n-k}$$

**Example:** $2, 6, 18, 54, 162, \dots$

- Common ratio $r = 3$
- $g_0 = 2$
- General term: $g_n = 2 \cdot 3^n$
- 5th term: $g_5 = 2 \cdot 3^5 = 2 \cdot 243 = 486$

---

### 📊 Key Comparison

| Feature | Arithmetic Sequence | Geometric Sequence |
|:-------:|:-------------------:|:-------------------:|
| Change pattern | Addition (add $d$) | Multiplication (multiply by $r$) |
| Growth pattern | Same amount added each step | The added amount grows each step |
| Formula structure | $a_0 + d \cdot n$ | $g_0 \cdot r^n$ |

> 🔹 An **increasing arithmetic sequence** adds the same amount each step, while an **increasing geometric sequence** adds larger and larger amounts each step.

---

## 📈 TOPIC 2.2 — Change in Linear and Exponential Functions

### 📌 Core Concept

Arithmetic and geometric sequences can be **extended to all real numbers**, giving linear and exponential functions.

---

### 📏 Linear Function ← Arithmetic Sequence

Extend $a_n = a_0 + d \cdot n$ to all real $x$:

$$f(x) = mx + b$$

or point‑slope form:

$$f(x) = y_i + m(x - x_i)$$

Here $m$ (slope) corresponds to the common difference $d$, and $b$ (intercept) corresponds to the initial value $a_0$.

---

### 📈 Exponential Function ← Geometric Sequence

Extend $g_n = g_0 \cdot r^n$ to all real $x$:

$$f(x) = a \cdot b^x$$

or based on a known point:

$$f(x) = y_i \cdot r^{(x - x_i)}$$

Here $b$ (base) corresponds to the common ratio $r$, and $a$ (initial value) corresponds to $g_0$.

---

### 🔄 Linear vs. Exponential: Key Difference

**Linear function:** Over equal‑length input intervals, the output changes by a **constant amount** (addition).

**Exponential function:** Over equal‑length input intervals, the output changes by a **constant factor** (multiplication).

> Linear functions are based on **addition**, exponential functions on **multiplication**.

**Side‑by‑side example:**

| $x$ | $f(x) = 3x + 2$ (linear) | $g(x) = 2 \cdot 3^x$ (exponential) |
|:---:|:------------------------:|:----------------------------------:|
| $0$ | $2$ | $2$ |
| $1$ | $5$ ($+3$) | $6$ ($\times 3$) |
| $2$ | $8$ ($+3$) | $18$ ($\times 3$) |
| $3$ | $11$ ($+3$) | $54$ ($\times 3$) |

---

## 🚀 TOPIC 2.3 — Exponential Functions

### 📌 General Form

$$f(x) = a \cdot b^x$$

where:
- $a$ = initial value ($a \neq 0$)
- $b$ = base ($b > 0$, $b \neq 1$)
- Domain: all real numbers $\mathbb{R}$

> **Note about the sign of $a$:** The discussion below (increasing/decreasing, concavity, limits) assumes $a > 0$, which is the most common case in AP modeling.  
> If $a < 0$, the graph is reflected across the $x$‑axis:
> - Increasing becomes decreasing, and vice versa.
> - Concave up becomes concave down, and vice versa.
> - The signs of limits also flip ($\infty$ becomes $-\infty$, etc.).

---

### 🌱 Exponential Growth vs. Decay (when $a > 0$)

| Condition | Type | Graph features |
|:---------:|:----:|:--------------:|
| $a > 0$, $b > 1$ | **Exponential growth** | Increasing, concave up |
| $a > 0$, $0 < b < 1$ | **Exponential decay** | Decreasing, concave up |

---

### 📊 Key Features

1. **Constant factor property:** Over equal‑length input intervals, outputs change by a constant factor.
2. **Monotonicity:** An exponential function is either always increasing or always decreasing (when $a>0$).
3. **Concavity:** Always concave up (when $a>0$); no inflection points.
4. **No extrema:** Except on a closed interval, there are no local maxima/minima.
5. **End behavior (when $a > 0$):**

$$\lim_{x \to \infty} a b^x = \begin{cases} \infty & (b > 1) \\ 0 & (0 < b < 1) \end{cases}$$

$$\lim_{x \to -\infty} a b^x = \begin{cases} 0 & (b > 1) \\ \infty & (0 < b < 1) \end{cases}$$

**Example:** $f(x) = 5 \cdot 2^x$

- Initial value $a = 5$, base $b = 2$ ($>1$, growth)
- $f(0) = 5$, $f(1) = 10$, $f(2) = 20$, $f(3) = 40$
- Each increase of $1$ in $x$ doubles the output
- $\lim_{x \to -\infty} f(x) = 0$ (horizontal asymptote $y = 0$)

---

## 🔧 TOPIC 2.4 — Exponential Function Manipulation

### 📌 Properties of Exponents

#### 1️⃣ Product Property

$$b^m \cdot b^n = b^{m+n}$$

**Graphical meaning:** A **horizontal shift** of an exponential function is equivalent to a **vertical stretch**:

$$b^{x+k} = b^k \cdot b^x = a \cdot b^x \quad \text{where } a = b^k$$

So $f(x) = b^{x+k}$ and $f(x) = (b^k) \cdot b^x$ are the same function.

#### 2️⃣ Power Property

$$(b^m)^n = b^{mn}$$

**Graphical meaning:** A **horizontal dilation** of an exponential function is equivalent to **changing the base**:

$$b^{cx} = (b^c)^x$$

Thus $f(x) = b^{cx}$ is the same as an exponential function with base $b^c$.

#### 3️⃣ Negative Exponent Property

$$b^{-n} = \frac{1}{b^n}$$

#### 4️⃣ Fractional Exponent Property

$$b^{1/k} = \sqrt[k]{b}$$

---

**Example:** Rewrite $f(x) = 2^{x+3}$ in the form $f(x) = a \cdot 2^x$.

$$2^{x+3} = 2^3 \cdot 2^x = 8 \cdot 2^x$$

So $a = 8$; a horizontal shift left by $3$ units is equivalent to a vertical stretch by a factor of $8$.

**Example:** Rewrite $f(x) = 3^{2x}$ in the form $f(x) = (b)^x$.

$$3^{2x} = (3^2)^x = 9^x$$

So $b = 9$.

---

## 🌍 TOPIC 2.5 — Exponential Function Context and Data Modeling

### 📌 Modeling with Exponentials

Use an exponential model when a phenomenon changes by a **constant factor** over equal time intervals.

$$f(x) = a \cdot b^x$$

---

### 🔑 How to Build an Exponential Model

1. **From initial value and growth factor:** given $a$ and $b$
2. **From two points:** solve a system of equations
3. **Using regression:** exponential regression on a calculator
4. **Via transformations:** apply transformations to $f(x) = a \cdot b^x$

---

### 🌐 The Natural Base $e$

$$e \approx 2.71828\ldots$$

The natural base $e$ is extremely important in calculus and is often used to model continuous growth/decay:

$$f(x) = a \cdot e^{kx}$$

where $k$ is the continuous growth rate ($k>0$ for growth, $k<0$ for decay).

---

### 📖 Percentage Change and Growth Factor

For $f(x) = a \cdot b^x$, the base $b$ is called the **growth factor**:

$$b = 1 + r$$

where $r$ is the **percentage rate of change** per unit input (expressed as a decimal).

- **$r > 0$** : exponential growth ($b > 1$)
- **$r < 0$** : exponential decay ($0 < b < 1$, because $1+r$ is still positive)

**Example:** A population grows by $5\%$ per year → $r = 0.05$, $b = 1.05$, model: $P(t) = P_0 \cdot (1.05)^t$.  
If it decays by $5\%$ per year → $r = -0.05$, $b = 0.95$, model: $P(t) = P_0 \cdot (0.95)^t$.

---

### 🔄 Equivalent Forms in Context

If $d$ represents days, $f(d) = 2^d$ means **doubling every day**. An equivalent form:

$$f(d) = (2^7)^{d/7} = 128^{d/7}$$

means **becoming 128 times larger every week**.

---

## 📊 TOPIC 2.6 — Competing Function Model Validation

### 📌 Comparing and Validating Models

When a data set shows a **slightly changing rate of change**, you can fit linear, quadratic, or exponential models.

**How to choose:**
- Context clues
- Residual plot analysis

---

### 📉 Residual Analysis

$$\text{Residual} = \text{Actual value} - \text{Predicted value}$$

**Criterion:** If the residual plot shows **no obvious pattern** (random scatter), the model is appropriate.

- Pattern present → model is not appropriate
- Random scatter → model is appropriate

---

### 📋 Quick Decision Guide

- **Linear:** Output changes by a constant amount over equal input intervals.
- **Exponential:** Output changes by a constant factor over equal input intervals.
- **Quadratic:** The rate of change itself changes linearly.

---

## 🔗 TOPIC 2.7 — Composition of Functions

### 📌 Definition of Composition

If $f$ and $g$ are functions, the composition $f \circ g$ is defined by:

$$(f \circ g)(x) = f(g(x))$$

First apply $g$ to $x$, then apply $f$ to the result.

**Domain of $f \circ g$:** All $x$ such that $g(x)$ is in the domain of $f$.

---

### ⚠️ Important Properties

**Composition is not commutative:**

$$f(g(x)) \neq g(f(x)) \quad \text{(in general)}$$

**Identity function:** $f(x) = x$ composes trivially:

$$g(f(x)) = f(g(x)) = g(x)$$

---

### 🔄 Algebraic Composition

If $f$ and $g$ have formulas, substitute $g(x)$ into every $x$ in $f$:

**Example:** $f(x) = x^2 + 1$, $g(x) = 3x$

$$f(g(x)) = f(3x) = (3x)^2 + 1 = 9x^2 + 1$$

$$g(f(x)) = g(x^2 + 1) = 3(x^2 + 1) = 3x^2 + 3$$

Here $f(g(x)) \neq g(f(x))$.

---

### ✂️ Decomposing a Function

A complex function can be written as a composition of simpler functions.

**Example:** $h(x) = \sqrt{2^x + 1}$

Let $f(x) = \sqrt{x}$, $g(x) = x + 1$, $k(x) = 2^x$

Then $h(x) = f(g(k(x)))$.

---

### 📐 Transformations as Compositions

- Horizontal/vertical shifts: compose with $g(x) = x + k$
- Horizontal/vertical dilations: compose with $g(x) = kx$

---

## 🔄 TOPIC 2.8 — Inverse Functions

### 📌 Definition of Inverse

A function $f$ is **invertible** on a given domain if each output corresponds to exactly one input (i.e., it is one‑to‑one; passes the horizontal line test).

$$f^{-1}(b) = a \quad \text{if and only if} \quad f(a) = b$$

The inverse function $f^{-1}$ maps outputs back to inputs. If $f$ contains the ordered pair $(a, b)$, then $f^{-1}$ contains $(b, a)$.

---

### 🔑 Key Properties

**Composition property:** A function and its inverse compose to the identity:

$$f(f^{-1}(x)) = f^{-1}(f(x)) = x$$

**Domain and range swap:**
- Domain of $f$ = Range of $f^{-1}$
- Range of $f$ = Domain of $f^{-1}$

---

### 📊 Three Ways to Find an Inverse

| Method | Operation |
|:------:|:---------:|
| **Numerical** | Reverse input‑output pairs: $(a, b) \to (b, a)$ |
| **Graphical** | Reflect across $y = x$ (the identity line) |
| **Algebraic** | Swap $x$ and $y$, then solve for $y$ |

**Example (algebraic):** Find the inverse of $f(x) = 2x + 3$.

1. Write $y = 2x + 3$
2. Swap $x$ and $y$: $x = 2y + 3$
3. Solve for $y$: $x - 3 = 2y \implies y = \frac{x - 3}{2}$
4. So $f^{-1}(x) = \frac{x - 3}{2}$

Check: $f(f^{-1}(x)) = 2\left(\frac{x-3}{2}\right) + 3 = x - 3 + 3 = x$ ✓

---

### ⚠️ Notes

- You can make a function invertible by restricting its domain (e.g., $f(x)=x^2$ with $x\ge 0$).
- Contextual restrictions may also affect the applicability of the inverse.

---

## 🔢 TOPIC 2.9 — Logarithmic Expressions

### 📌 Definition of Logarithm

$$\log_b c = a \quad \iff \quad b^a = c$$

Read as "$\log$ base $b$ of $c$ equals $a$", meaning: the exponent $a$ to which the base $b$ must be raised to get $c$.

Here:
- $b$ = base ($b > 0$, $b \neq 1$)
- $c$ = argument (must satisfy $\mathbf{c > 0}$, otherwise the logarithm is undefined)
- $a$ = logarithm value

---

### 📋 Common Logarithms

$$\log x = \log_{10} x \quad \text{(base 10 is omitted when written)}$$

$$\ln x = \log_e x \quad \text{(natural logarithm, base $e$)}$$

---

### 📊 Logarithmic Scale

On a logarithmic scale, each unit represents a **multiplicative change** in the base.

For a base‑10 logarithmic scale:
$$\ldots, 0, 1, 2, 3, \ldots \quad \text{corresponds to} \quad 10^0, 10^1, 10^2, 10^3, \ldots$$
i.e., $1, 10, 100, 1000, \dots$

**Example:** $\log_{10} 1000 = 3$ because $10^3 = 1000$

**Example:** $\log_2 32 = 5$ because $2^5 = 32$

**Example:** $\log_3 \frac{1}{9} = -2$ because $3^{-2} = \frac{1}{9}$

---

## 🔄 TOPIC 2.10 — Inverses of Exponential Functions

### 📌 Logarithmic Function = Inverse of Exponential

The exponential function $f(x) = b^x$ and the logarithmic function $g(x) = \log_b x$ are inverses of each other:

$$f(g(x)) = b^{\log_b x} = x$$
$$g(f(x)) = \log_b(b^x) = x$$

---

### 📐 General Form of a Logarithmic Function

$$f(x) = a \cdot \log_b x$$

where $b > 0$, $b \neq 1$, $a \neq 0$.

---

### 🔄 Inverse Relationship in Changes

| Exponential $y = b^x$ | Logarithmic $y = \log_b x$ |
|:---------------------:|:--------------------------:|
| Equal input addition → output multiplied by $b$ | Input multiplied by $b$ → output increases by $1$ |
| Input **addition** → output **multiplication** | Input **multiplication** → output **addition** |

---

### 📊 Graphical Relationship

The graphs of $g(x) = b^x$ and $f(x) = \log_b x$ are symmetric about the line $y = x$:

- If $(s, t)$ lies on the exponential graph, then $(t, s)$ lies on the logarithmic graph.

---

## 📊 TOPIC 2.11 — Logarithmic Functions

### 📌 Key Features

$$f(x) = a \cdot \log_b x$$

> **Note about the sign of $a$:** The discussion below assumes $a > 0$ (common in modeling).  
> If $a < 0$, the graph is reflected across the $x$‑axis: monotonicity and concavity reverse (increasing becomes decreasing, and concavity flips).

| Feature | Description (when $a > 0$, $b > 1$) |
|:-------:|:-----------------------------------:|
| **Domain** | $x > 0$ (positive reals) |
| **Range** | all real numbers $\mathbb{R}$ |
| **Monotonicity** | Always increasing ($b>1$) or always decreasing ($0<b<1$) |
| **Concavity** | Always concave down ($b>1$) or concave up ($0<b<1$) |
| **Extrema** | None (except on a closed interval) |
| **Inflection points** | None |

---

### 📐 End Behavior and Asymptotes (when $a > 0$)

Logarithmic functions have a **vertical asymptote** at $x = 0$:

$$\lim_{x \to 0^+} \log_b x = \begin{cases} -\infty & (b > 1) \\ \infty & (0 < b < 1) \end{cases}$$

$$\lim_{x \to \infty} \log_b x = \begin{cases} \infty & (b > 1) \\ -\infty & (0 < b < 1) \end{cases}$$

---

### 🔄 How to Recognize a Logarithmic Function

If the additive transformation $g(x) = f(x + k)$ causes the input to change proportionally over equal output intervals, then $f$ is logarithmic.

---

## 🛠️ TOPIC 2.12 — Logarithmic Function Manipulation

### 📌 Three Core Properties of Logarithms

#### 1️⃣ Product Property (Product becomes Sum)

$$\log_b(xy) = \log_b x + \log_b y$$

**Graphical meaning:** A **horizontal dilation** of a logarithmic function is equivalent to a **vertical shift**:

$$\log_b(kx) = \log_b k + \log_b x = a + \log_b x \quad \text{where } a = \log_b k$$

#### 2️⃣ Power Property (Exponent becomes Factor)

$$\log_b(x^n) = n \cdot \log_b x$$

**Graphical meaning:** Raising the input to a power is equivalent to a **vertical stretch**:

$$\log_b(x^k) = k \cdot \log_b x$$

#### 3️⃣ Change of Base Formula

$$\log_b x = \frac{\log_a x}{\log_a b}$$

where $a > 0$, $a \neq 1$.

**Meaning:** All logarithmic functions are **vertical stretches** of each other.

---

### 🌐 Natural Logarithm

$$\ln x = \log_e x$$

$\ln x$ is the logarithm with base $e$.

---

**Example (Product Property):** $\log_2(8 \cdot 4) = \log_2 8 + \log_2 4 = 3 + 2 = 5$

Check: $8 \cdot 4 = 32$, $\log_2 32 = 5$ ✓

**Example (Power Property):** $\log_3(9^4) = 4 \cdot \log_3 9 = 4 \cdot 2 = 8$

Check: $9^4 = 6561$, $\log_3 6561 = 8$ (because $3^8 = 6561$) ✓

**Example (Change of Base):** $\log_2 5 = \frac{\log_{10} 5}{\log_{10} 2} \approx \frac{0.6990}{0.3010} \approx 2.322$

---

## 🎯 TOPIC 2.13 — Exponential and Logarithmic Equations and Inequalities

### 📌 Strategy for Solving Equations

Use properties of exponents, logarithms, and the **inverse relationship** between exponentials and logs:

$$b^{\log_b x} = x \quad \text{and} \quad \log_b(b^x) = x$$

---

### 🔑 Common Methods

**Method 1: Take a logarithm** — for exponential equations

$$a^x = b \implies \ln(a^x) = \ln b \implies x \ln a = \ln b \implies x = \frac{\ln b}{\ln a}$$

**Method 2: Exponentiate** — for logarithmic equations

$$\log_b x = c \implies x = b^c$$

---

### ⚠️ Check for Extraneous Solutions

After solving, always check that the solution satisfies the domain restrictions of the original equation (argument $>0$, base $>0$ and $\neq 1$).

---

**Example 1 (exponential equation):** Solve $3^{x+1} = 27$

$$3^{x+1} = 27 = 3^3 \implies x + 1 = 3 \implies x = 2$$

**Example 2 (exponential – take log):** Solve $2^x = 10$

$$2^x = 10 \implies \ln(2^x) = \ln 10 \implies x \ln 2 = \ln 10 \implies x = \frac{\ln 10}{\ln 2} \approx 3.322$$

**Example 3 (logarithmic equation):** Solve $\log_2(x + 1) = 3$

$$\log_2(x + 1) = 3 \implies x + 1 = 2^3 = 8 \implies x = 7$$

Check: $\log_2(7 + 1) = \log_2 8 = 3$ ✓

---

### 📐 Solving Inequalities

The key is to use the **monotonicity** of exponential and logarithmic functions, while respecting domain restrictions.

#### 🔹 Exponential Inequalities

**Steps:**
1. Express both sides with the same base, or take a logarithm.
2. Determine whether the base $b$ is $>1$ or $0<b<1$.
   - If $b > 1$ (increasing), the inequality sign stays the same.
   - If $0 < b < 1$ (decreasing), the inequality sign reverses.

**Example 4 (exponential inequality, $b>1$):** Solve $2^x > 5$

Since $2 > 1$, the function is increasing. Take $\log_2$ of both sides (or $\ln$):

$$2^x > 5 \implies \log_2(2^x) > \log_2 5 \implies x > \log_2 5$$

or $x > \frac{\ln 5}{\ln 2} \approx 2.322$.

**Example 5 (exponential inequality, $0<b<1$):** Solve $\left(\frac{1}{2}\right)^x \geq 8$

Base $b = 0.5 < 1$, so the function is decreasing. Taking $\log_{0.5}$ reverses the inequality:

$$\left(\frac{1}{2}\right)^x \geq 8 \implies \log_{0.5}\left(\left(\frac{1}{2}\right)^x\right) \leq \log_{0.5} 8 \implies x \leq \log_{0.5} 8$$

Compute $\log_{0.5} 8 = \frac{\ln 8}{\ln 0.5} = \frac{\ln 8}{-\ln 2} = -3$, so $x \leq -3$.

#### 🔹 Logarithmic Inequalities

**Steps:**
1. Determine the domain (argument $>0$).
2. Write both sides as logarithms with the same base, using the monotonicity of the log function.
3. Remove the logarithm, respecting the inequality direction based on whether $b>1$ or $0<b<1$.
4. Intersect with the domain.

**Example 6 (log inequality, $b>1$):** Solve $\log_2(x - 1) < 3$

Domain: $x - 1 > 0 \implies x > 1$.  
Base $2 > 1$, so $\log_2$ is increasing; the inequality direction stays:

$$\log_2(x - 1) < 3 \implies x - 1 < 2^3 = 8 \implies x < 9$$

Intersect with domain $x > 1$: $1 < x < 9$.

**Example 7 (log inequality, $0<b<1$):** Solve $\log_{0.5}(x + 2) \geq -1$

Domain: $x + 2 > 0 \implies x > -2$.  
Base $0.5 < 1$, so $\log_{0.5}$ is decreasing; the inequality reverses when we exponentiate:

$$\log_{0.5}(x + 2) \geq -1 \implies x + 2 \leq (0.5)^{-1} = 2 \implies x \leq 0$$

Intersect with domain $x > -2$: $-2 < x \leq 0$.

---

### 📐 Inverse of Transformed Forms

Inverse of a transformed exponential:

$$y = a \cdot b^{(x-h)} + k \quad \longrightarrow \quad y = h + \log_b\left(\frac{x - k}{a}\right) \quad \text{(requires $a>0$, $x>k$)}$$

Inverse of a transformed logarithm:

$$y = a \cdot \log_b(x - h) + k \quad \longrightarrow \quad y = h + b^{(x-k)/a}$$

---

## 🌍 TOPIC 2.14 — Logarithmic Function Context and Data Modeling

### 📌 Applications of Logarithmic Models

As inverses of exponential functions, logarithms model situations where the **input changes proportionally** and the **output changes by equal amounts**.

**Real‑world applications:**
- Sound intensity (decibels)
- Earthquake magnitude (Richter scale)
- pH (acidity)
- Human working memory

---

### 📊 How to Build a Logarithmic Model

1. **From proportionality and zero point**
2. **From two points:** solve a system of equations
3. **Via transformations:** apply transformations to $f(x) = a \cdot \log_b x$
4. **Using regression:** logarithmic regression on a calculator

---

### 🔑 Importance of Natural Logarithms in Modeling

$$\ln x = \log_e x$$

Natural logarithms are widely used in scientific modeling and often simplify calculations.

---

## 📉 TOPIC 2.15 — Semi-log Plots

### 📌 What is a Semi‑log Plot?

In a semi‑log plot, **one axis (usually the $y$‑axis) uses a logarithmic scale**.

**Core idea:** If data are exponential, they will appear **linear** on a semi‑log plot.

---

### 🎯 Using Semi‑log Plots to Identify Exponential Models

When the $y$‑axis is logarithmically scaled, if the points lie approximately on a straight line, then an exponential model $y = a \cdot b^x$ is appropriate.

**Advantage:** Semi‑log plots reveal exponential behavior without needing to add a constant to $y$ values.

---

### 🔄 Linearization

For an exponential model $y = a \cdot b^x$, take a logarithm with any base $n$ ($n > 0$, $n \neq 1$):

$$\log_n y = \log_n(a \cdot b^x) = \log_n a + x \cdot \log_n b$$

Let $Y = \log_n y$. Then:

$$Y = (\log_n b) \cdot x + \log_n a$$

This is a **linear function** of $x$:
- Slope $m = \log_n b$
- Intercept $b_{\text{lin}} = \log_n a$

> **Note:** Any convenient base $n$ (e.g., $n=10$ or $n=e$) works. Changing $n$ changes the slope and intercept but does not affect the fact that the relationship is linear.

---

**Example:** Data points $(1, 5), (2, 10), (3, 20), (4, 40)$

Take $\log_{10}$:

| $x$ | $y$ | $\log_{10} y$ |
|:---:|:---:|:-------------:|
| $1$ | $5$ | $0.6990$ |
| $2$ | $10$ | $1.0000$ |
| $3$ | $20$ | $1.3010$ |
| $4$ | $40$ | $1.6021$ |

$\log_{10} y$ increases by roughly $0.301$ each step → exponential model.

Slope $= \log_{10} 2 \approx 0.3010$, intercept $= \log_{10} 2.5 \approx 0.3979$

Linearized form: $\log_{10} y = 0.3010x + 0.3979$

Thus $y = 10^{0.3010x + 0.3979} = 10^{0.3979} \cdot (10^{0.3010})^x \approx 2.5 \cdot 2^x$.

---

## 📋 UNIT 2 Core Formula Quick Reference

| Category | Formula |
|:--------:|:-------:|
| **Arithmetic sequence** | $a_n = a_0 + d \cdot n$ (starting at term $0$) |
| **Geometric sequence** | $g_n = g_0 \cdot r^n$ |
| **Linear function** | $f(x) = mx + b$ |
| **Exponential function** | $f(x) = a \cdot b^x$ |
| **Logarithm definition** | $\log_b c = a \iff b^a = c$ (argument $c>0$) |
| **Logarithmic function** | $f(x) = a \cdot \log_b x$ |
| **Product property (exponents)** | $b^m \cdot b^n = b^{m+n}$ |
| **Power property (exponents)** | $(b^m)^n = b^{mn}$ |
| **Product property (logs)** | $\log_b(xy) = \log_b x + \log_b y$ |
| **Power property (logs)** | $\log_b(x^n) = n \cdot \log_b x$ |
| **Change of base** | $\log_b x = \frac{\log_a x}{\log_a b}$ |
| **Exponential‑log inverse** | $b^{\log_b x} = x$, $\log_b(b^x) = x$ |
| **Semi‑log linearization** | $\log_n y = (\log_n b) \cdot x + \log_n a$ |
| **Natural base** | $e \approx 2.718$, $\ln x = \log_e x$ |
