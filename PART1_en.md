## ⚠️ Unit 1 Common Mistakes (Self‑Study Pitfalls)
- 这份笔记由 LG-leo 整理和维护。如果你觉得这份笔记对你有帮助，欢迎在 GitHub 上关注我或给我一个 ⭐，这能帮助我持续产出更多免费的学习资源。
- 我的其他课程笔记：https://github.com/LG-leo?tab=repositories
- This note is maintained by LG-leo. If you find it helpful, feel free to follow me or leave a ⭐ on GitHub. It helps me keep producing more free study resources. Check out my other notes: https://github.com/LG-leo?tab=repositories
---

### 🚫 Pitfall 1: Confusing Holes with Vertical Asymptotes

This is the most classic and easily confused issue with rational functions.

#### ✅ Correct Rule

The key is whether the common factor between the numerator and denominator **cancels completely**.

| Condition | Result | Reason |
|:---------:|:------:|:------:|
| Denominator has a zero at $a$, numerator does **not** have a zero at $a$ | Vertical asymptote $x = a$ | Denominator $\to 0$, numerator $\to$ nonzero, function $\to \pm\infty$ |
| Both numerator and denominator have a zero at $a$, and **multiplicity in numerator $\ge$ multiplicity in denominator** | Hole at $x = a$ | Common factor cancels; denominator no longer zero |
| Both have a zero at $a$, but **multiplicity in numerator $<$ multiplicity in denominator** | Vertical asymptote $x = a$ | After cancellation, denominator still has a zero |

#### 📌 One‑sentence reminder

> **"Cancel completely → hole; cannot cancel completely → asymptote"**

#### 💥 Comparative Examples

**Example A (Hole):**
$$
r(x) = \frac{x^2 - 4}{x - 2}
$$

Simplify:
$$
r(x) = \frac{(x-2)(x+2)}{x-2} = x + 2,\; x \neq 2
$$

At $x = 2$ there is a **hole** at $(2, 4)$.

**Example B (Vertical Asymptote):**
$$
r(x) = \frac{x + 2}{x - 2}
$$

Numerator at $x = 2$: $2+2=4\neq 0$, nothing cancels. $x = 2$ is a **vertical asymptote**.

**Example C (Tricky – numerator multiplicity < denominator multiplicity):**
$$
r(x) = \frac{x-1}{(x-1)^2} = \frac{1}{x-1},\; x \neq 1
$$

One $(x-1)$ cancels but denominator still has a zero → $x = 1$ is still a **vertical asymptote**, not a hole!

---

### 🚫 Pitfall 2: Mixing Up End Behavior of Polynomials vs Rational Functions

The way you analyze end behavior is **completely different** for these two function types.

#### ✅ Polynomial End Behavior: Look Only at the Leading Term

$$
p(x) = a_n x^n + a_{n-1} x^{n-1} + \cdots + a_0 \;\approx\; a_n x^n \quad \text{as } |x| \to \infty
$$

Only two things matter: degree $n$ (even/odd) + leading coefficient $a_n$ (positive/negative)

| $n$ | $a_n > 0$ | $a_n < 0$ |
|:---:|:---------:|:---------:|
| **Even** | both ends $\to +\infty$ | both ends $\to -\infty$ |
| **Odd** | left $\to -\infty$, right $\to +\infty$ | left $\to +\infty$, right $\to -\infty$ |

#### ✅ Rational Function End Behavior: Compare Degrees of Numerator and Denominator

$$
r(x) = \frac{p(x)}{q(x)}, \quad \deg(p)=m,\; \deg(q)=n
$$

| Condition | End Behavior |
|:---------:|:-------------:|
| $m < n$ | Horizontal asymptote $y = 0$ |
| $m = n$ | Horizontal asymptote $y = \dfrac{a_m}{b_n}$ (ratio of leading coefficients) |
| $m > n$ | **No** horizontal asymptote; may have slant asymptote (if $m = n+1$) or polynomial‑like end behavior |

#### 💥 Typical Mistake

**Wrong approach:** See a rational function and treat it like a polynomial.

**Right approach:** First ask – "Is this a polynomial or a rational function?"

> Polynomial → **leading term only**  
> Rational function → **compare degrees**

#### Side‑by‑side Examples

| Function | Type | Analysis |
|:--------:|:----:|:---------:|
| $f(x) = -3x^4 + 2x^2$ | ✅ Polynomial | $n=4$ even, $a_n=-3<0$ → both ends $\to -\infty$ |
| $f(x) = \dfrac{-3x^4 + 2x^2}{x^2 + 1}$ | ✅ Rational | $m=4, n=2, m>n$ → no HA, end behavior like $-3x^2$ |
| $f(x) = \dfrac{-3x^4 + 2x^2}{2x^4 - 5}$ | ✅ Rational | $m=n=4$ → HA $y = \dfrac{-3}{2}$ |
| $f(x) = \dfrac{2x}{x^2+1}$ | ✅ Rational | $m=1 < n=2$ → HA $y = 0$ |

---

### 🚫 Pitfall 3: Incorrectly Identifying Even / Odd Functions

#### ✅ The Reliable Method

Use the definitions directly (most reliable):

| Type | Definition | Symmetry |
|:----:|:----------:|:--------:|
| **Even** | $f(-x) = f(x)$ | Symmetric about the $y$-axis |
| **Odd** | $f(-x) = -f(x)$ | Symmetric about the origin |

#### 💥 Common Misconceptions

**Misconception 1: Look only at the highest‑degree term.**

No! Consider $p(x) = x^3 + x^2$.  
Check:
$$
p(-x) = (-x)^3 + (-x)^2 = -x^3 + x^2
$$
This is neither $p(x)$ nor $-p(x)$ → **neither even nor odd**.

> ✅ **Correct rule:** A polynomial is **even** iff **every term has an even degree**; it is **odd** iff **every term has an odd degree**. Mixed degrees → neither.

**Misconception 2: $f(0)=0$ implies odd.**

Counterexample: $f(x) = x^2$, $f(0)=0$ but it is **even**!

> ✅ **Correct rule:** An odd function **must** satisfy $f(0)=0$ (if $0$ is in the domain), but $f(0)=0$ does **not** guarantee oddness.

**Misconception 3: Even functions cannot have odd‑degree terms, odd functions cannot have even‑degree terms.**

True for non‑zero coefficients, but zero coefficients cause no harm.

Example: $f(x) = x^4 + 0x^3 + 2x^2 + 0x + 1$ – all **non‑zero** exponents are even → even function ✅

#### 📌 Quick Reference Table

| Function | Substitute $-x$ | $f(-x)=f(x)$? | $f(-x)=-f(x)$? | Conclusion |
|:--------:|:---------------:|:-------------:|:--------------:|:----------:|
| $f(x)=x^2$ | $(-x)^2=x^2$ | ✅ | ❌ | **Even** |
| $f(x)=x^3$ | $(-x)^3=-x^3$ | ❌ | ✅ | **Odd** |
| $f(x)=x^3+x$ | $(-x)^3+(-x) = -x^3-x = -(x^3+x)$ | ❌ | ✅ | **Odd** |
| $f(x)=x^2+x$ | $(-x)^2+(-x)=x^2-x$ | ❌ | ❌ | **Neither** |
| $f(x)=5$ (constant) | $5$ | ✅ | ❌ | **Even** (degree 0 is even) |
| $f(x)=0$ | $0$ | ✅ | ✅ | **Both even and odd** |

---

### 📝 Ultimate One‑Line Summary of the Three Pitfalls

| # | Pitfall | One‑Sentence Reminder |
|:-:|:-------:|:---------------------:|
| 1 | **Hole vs Vertical Asymptote** | "Cancel completely → hole; cannot cancel completely → asymptote" |
| 2 | **Polynomial vs Rational End Behavior** | Polynomial → **leading term**; Rational → **compare degrees** |
| 3 | **Even / Odd Function** | Substituting $-x$ is the safest method – don't just look at the highest power. |
