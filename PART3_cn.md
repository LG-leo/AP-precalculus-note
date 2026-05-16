# 📐 UNIT 3: Trigonometric and Polar Functions
- 这份笔记由 LG-leo 整理和维护。如果你觉得这份笔记对你有帮助，欢迎在 GitHub 上关注我或给我一个 ⭐，这能帮助我持续产出更多免费的学习资源。
- 我的其他课程笔记：https://github.com/LG-leo?tab=repositories
- This note is maintained by LG-leo. If you find it helpful, feel free to follow me or leave a ⭐ on GitHub. It helps me keep producing more free study resources. Check out my other notes: https://github.com/LG-leo?tab=repositories
> **AP Exam Weighting:** $30$–$35\%$  
> **Recommended Class Periods:** $35$–$50$  
> **Total Topics:** $15$（3.1 到 3.15）

---

## 🔹 3.1 — Periodic Phenomena 周期现象

### 核心概念

**周期函数（Periodic Function）** 是指输出值在等长输入区间上重复出现的函数。若存在最小正数 $k$ 使得对所有 $x$ 有：

$$
f(x + k) = f(x)
$$

则 $k$ 为最小正周期。

**关键性质：**
- 周期函数在一个周期内的所有特征（增减区间、凹凸性、变化率）会在每个周期中完全重复。
- 只需知道一个完整周期的图像，即可通过平移画出整个函数图像。
- 周期可通过观察连续最大值（或连续最小值）之间的水平距离来估计。

### 示例

> **例 1：** 某潮汐数据显示高潮在 $t=0$ 时出现，下一次高潮在 $t=12$ 小时后。估计周期。

$$
\text{周期} = 12 \text{ 小时}
$$

---

## 🔹 3.2 — Sine, Cosine, and Tangent 正弦、余弦、正切

### 单位圆定义

在标准位置的角 $\theta$：
- **顶点**在原点
- **起始边**在正 $x$-轴上
- **终边**（terminal ray）为另一条射线

> **正角** = 逆时针旋转；**负角** = 顺时针旋转。

终边相同的角相差整数倍的 $2\pi$，即 $k \in \mathbb{Z}$：

$$
\theta + 2\pi k \quad (k \in \mathbb{Z})
$$

**弧度制：** 角的弧度 = 弧长 / 半径。对于单位圆（半径 $= 1$），弧度 = 弧长。

### 三角函数定义

对于单位圆上的交点 $P$：

$$
\sin\theta = y\text{-坐标 of } P
$$

$$
\cos\theta = x\text{-坐标 of } P
$$

$$
\tan\theta = \frac{\sin\theta}{\cos\theta} = \text{终边的斜率（当 } \cos\theta \neq 0 \text{ 时）}
$$

### 示例

> **例 2：** 求 $\theta = \frac{\pi}{6}$ 的正弦、余弦和正切值。

在单位圆上，$\theta = \frac{\pi}{6}$ 对应点 $P\left(\frac{\sqrt{3}}{2}, \frac{1}{2}\right)$

$$
\sin\frac{\pi}{6} = \frac{1}{2}, \quad \cos\frac{\pi}{6} = \frac{\sqrt{3}}{2}, \quad \tan\frac{\pi}{6} = \frac{1/2}{\sqrt{3}/2} = \frac{1}{\sqrt{3}} = \frac{\sqrt{3}}{3}
$$

---

## 🔹 3.3 — Sine and Cosine Function Values 正弦与余弦函数值

### 圆上的坐标

给定半径为 $r$ 的圆和标准位置的角 $\theta$，终边与圆的交点 $P$ 坐标为：

$$
P = (r\cos\theta,\; r\sin\theta)
$$

### 特殊角的精确值

利用等腰直角三角形（$45^\circ = \frac{\pi}{4}$）和等边三角形（$30^\circ = \frac{\pi}{6}$，$60^\circ = \frac{\pi}{3}$），结合象限符号可得精确值。

| $\theta$ | $\sin\theta$ | $\cos\theta$ | $\tan\theta$ |
|:--------:|:------------:|:------------:|:------------:|
| $0$ | $0$ | $1$ | $0$ |
| $\frac{\pi}{6}$ | $\frac{1}{2}$ | $\frac{\sqrt{3}}{2}$ | $\frac{\sqrt{3}}{3}$ |
| $\frac{\pi}{4}$ | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{2}}{2}$ | $1$ |
| $\frac{\pi}{3}$ | $\frac{\sqrt{3}}{2}$ | $\frac{1}{2}$ | $\sqrt{3}$ |
| $\frac{\pi}{2}$ | $1$ | $0$ | 无定义（垂直渐近线） |

> **例 3：** 求 $\sin\frac{5\pi}{4}$ 的值。

$\frac{5\pi}{4}$ 的终边在第三象限，参考角为 $\frac{\pi}{4}$。在第三象限 $\sin$ 为负：

$$
\sin\frac{5\pi}{4} = -\sin\frac{\pi}{4} = -\frac{\sqrt{2}}{2}
$$

---

## 🔹 3.4 — Sine and Cosine Function Graphs 正弦与余弦函数图像

### 正弦函数 $f(\theta) = \sin\theta$

- **定义域：** $\mathbb{R}$（全体实数）
- **值域：** $[-1, 1]$
- 给出单位圆上点 $P$ 的 $y$-坐标（垂直位移）
- 随 $\theta$ 增加，$\sin\theta$ 在 $-1$ 与 $1$ 之间振荡

### 余弦函数 $g(\theta) = \cos\theta$

- **定义域：** $\mathbb{R}$（全体实数）
- **值域：** $[-1, 1]$
- 给出单位圆上点 $P$ 的 $x$-坐标（水平位移）
- 随 $\theta$ 增加，$\cos\theta$ 在 $-1$ 与 $1$ 之间振荡

### 图像对称性

- $y = \sin\theta$：**奇函数**，图像关于原点对称（$\sin(-\theta) = -\sin\theta$）
- $y = \cos\theta$：**偶函数**，图像关于 $y$-轴对称（$\cos(-\theta) = \cos\theta$）
- 两者周期均为 $2\pi$

---

## 🔹 3.5 — Sinusoidal Functions 正弦型函数

### 定义

**正弦型函数（Sinusoidal Function）** 是指通过加法和乘法变换从 $f(\theta) = \sin\theta$ 得到的任何函数。正弦和余弦都是正弦型函数，且二者可通过相位移动互相转化：

$$
\cos\theta = \sin\left(\theta + \frac{\pi}{2}\right)
$$

### 关键特征

**周期（Period）** 与 **频率（Frequency）** 互为倒数：

$$
\text{周期} = 2\pi, \quad \text{频率} = \frac{1}{2\pi}
$$

**振幅（Amplitude）** 是最大值与最小值之差的一半：

$$
\text{振幅} = \frac{\text{最大值} - \text{最小值}}{2}
$$

对 $f(\theta) = \sin\theta$ 和 $g(\theta) = \cos\theta$，振幅为 $1$。

**中线（Midline）** 是最大值与最小值的平均值：

$$
\text{中线： } y = \frac{\text{最大值} + \text{最小值}}{2}
$$

对 $y = \sin\theta$ 和 $y = \cos\theta$，中线为 $y = 0$。

**对称性：**
- $y = \sin\theta$：**奇函数**（原点对称，$\sin(-\theta) = -\sin\theta$）
- $y = \cos\theta$：**偶函数**（$y$-轴对称，$\cos(-\theta) = \cos\theta$）

---

## 🔹 3.6 — Sinusoidal Function Transformations 正弦型函数的变换

### 一般形式（标准写法）

正弦型函数最常用的标准形式为：

$$
f(\theta) = a\sin(b\theta - c) + d
$$

$$
g(\theta) = a\cos(b\theta - c) + d
$$

其中 $a, b, c, d$ 为实数，$a \neq 0$，$b \neq 0$。

### 各参数的作用

| 参数 | 变换类型 | 效果 |
|:----:|:---------|:-----|
| $a$ | 垂直拉伸/压缩 | **振幅** $= |a|$；若 $a < 0$，图像关于 $x$-轴翻转 |
| $b$ | 水平拉伸/压缩 | **周期** $= \dfrac{2\pi}{|b|}$ |
| $c$ | 水平平移 | **相位移动（phase shift）** $= \dfrac{c}{b}$（右移当 $\dfrac{c}{b} > 0$） |
| $d$ | 垂直平移 | **中线** $y = d$ |

### 完整公式

$$
\text{振幅} = |a|, \quad \text{周期} = \frac{2\pi}{|b|}, \quad \text{相位移动} = \frac{c}{b}, \quad \text{中线： } y = d
$$

> **注意：** 若使用另一种形式 $f(\theta) = a\sin\bigl(b(\theta + c)\bigr) + d$，则相位移动为 $-c$（即当 $c>0$ 时图像左移 $c$ 单位）。本讲义采用 $f(\theta) = a\sin(b\theta - c) + d$ 形式，使相位移动直接为 $c/b$，更便于理解。

### 示例

> **例 4：** 求函数 $f(x) = 3\sin(2x - \pi) + 1$ 的振幅、周期、相位移动和中线。

$$
a = 3,\quad b = 2,\quad c = \pi,\quad d = 1
$$

$$
\text{振幅} = |3| = 3,\quad \text{周期} = \frac{2\pi}{2} = \pi,\quad \text{相位移动} = \frac{c}{b} = \frac{\pi}{2}\text{（右移）},\quad \text{中线： } y = 1
$$

---

## 🔹 3.7 — Sinusoidal Function Context and Data Modeling 正弦型函数建模

### 建模步骤

1. **确定周期：** 相邻最大值（或相邻最小值）之间的水平距离
2. **计算振幅和垂直位移：**

   $$
   \text{振幅} = \frac{\text{最大值} - \text{最小值}}{2}, \quad \text{垂直位移} = \frac{\text{最大值} + \text{最小值}}{2}
   $$

3. **确定相位移动：** 将实际数据点与标准正弦/余弦曲线进行比较
4. **使用技术工具：** 计算器进行正弦回归（sinusoidal regression）
5. **预测：** 仅在情境定义域内进行内插和外推

> **例 5：** 某地一年中最高温度 $30^\circ\text{C}$（7月），最低 $10^\circ\text{C}$（1月），周期 12 个月。建正弦模型。

$$
\text{振幅} = \frac{30 - 10}{2} = 10, \quad \text{中线} = \frac{30 + 10}{2} = 20, \quad b = \frac{2\pi}{12} = \frac{\pi}{6}
$$

设 7 月对应 $t = 6$（从1月算起），使用余弦模型：

$$
T(t) = 10\cos\left(\frac{\pi}{6}(t - 6)\right) + 20
$$

---

## 🔹 3.8 — The Tangent Function 正切函数

### 定义

正切函数 $f(\theta) = \tan\theta$ 表示终边的斜率：

$$
\tan\theta = \frac{\sin\theta}{\cos\theta}, \quad \cos\theta \neq 0
$$

### 关键特征

- **周期：** $\pi$（因为斜率每半圈重复一次）
- **垂直渐近线：** $\cos\theta = 0$，即 $\theta = \frac{\pi}{2} + k\pi,\; k\in\mathbb{Z}$
- 在相邻渐近线之间：$\tan$ 从 $-\infty$ 递增到 $+\infty$，图像从下凹（concave down）变为上凹（concave up）
- **定义域：** $\theta \neq \frac{\pi}{2} + k\pi,\; k\in\mathbb{Z}$

### 变换形式

$$
f(\theta) = a\tan(b\theta - c) + d
$$

- 垂直拉伸因子 $|a|$；若 $a < 0$，图像关于 $x$-轴反射，在每个周期内**递减**
- **周期** $= \dfrac{\pi}{|b|}$
- **相位移动** $= \dfrac{c}{b}$
- 垂直平移 $d$（拐点所在直线 $y = d$）

---

## 🔹 3.9 — Inverse Trigonometric Functions 反三角函数

### 定义

反三角函数的输入和输出与相应三角函数互换：
- **输入：** 一个数值（原函数值域中的值）
- **输出：** 一个角度

### 常用记法

$$
\arcsin x = \sin^{-1} x,\quad \arccos x = \cos^{-1} x,\quad \arctan x = \tan^{-1} x
$$

### 定义域限制

由于三角函数是周期性的，必须限制定义域才能得到一一对应：

| 函数 | 输入定义域 | 输出值域 |
|:----:|:----------:|:--------:|
| $\sin^{-1} x$ | $[-1, 1]$ | $\left[-\dfrac{\pi}{2},\; \dfrac{\pi}{2}\right]$ |
| $\cos^{-1} x$ | $[-1, 1]$ | $[0,\; \pi]$ |
| $\tan^{-1} x$ | $\mathbb{R}$ | $\left(-\dfrac{\pi}{2},\; \dfrac{\pi}{2}\right)$ |

> **注意：** $\arctan x$ 的图像有**水平渐近线** $y = \dfrac{\pi}{2}$ 和 $y = -\dfrac{\pi}{2}$，表示当 $x \to +\infty$ 时 $\arctan x \to \dfrac{\pi}{2}$，$x \to -\infty$ 时 $\arctan x \to -\dfrac{\pi}{2}$。

### 示例

> **例 6：** 求 $\sin^{-1}\left(\frac{1}{2}\right)$。

因为 $\sin\frac{\pi}{6} = \frac{1}{2}$ 且 $\frac{\pi}{6} \in \left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$：

$$
\sin^{-1}\left(\frac{1}{2}\right) = \frac{\pi}{6}
$$

---

## 🔹 3.10 — Trigonometric Equations and Inequalities 三角方程与不等式

### 求解三角方程

1. 使用反三角函数找到**基本解**（主值）
2. 由于三角函数是**周期性的**，通常有**无穷多解**
3. 若问题有定义域限制（如 $[0, 2\pi)$），需在范围内筛选所有解
4. 注意反函数只给出**一个主值**，需根据象限自行补充其他解

> **例 7a：** 在 $[0, 2\pi)$ 上解 $\sin\theta = \frac{\sqrt{2}}{2}$。

基本解：$\theta = \frac{\pi}{4}$。因 $\sin$ 在第二象限也为正，另一解为 $\pi - \frac{\pi}{4} = \frac{3\pi}{4}$。

$$
\theta = \frac{\pi}{4},\; \frac{3\pi}{4}
$$

> **例 7b：** 解 $\cos\theta = -\frac{1}{2}$，$\theta \in [0, 2\pi)$。

基本解（主值）：$\cos^{-1}\left(-\frac{1}{2}\right) = \frac{2\pi}{3}$。因 $\cos$ 在第三象限也为负，另一解为 $2\pi - \frac{2\pi}{3} = \frac{4\pi}{3}$。

$$
\theta = \frac{2\pi}{3},\; \frac{4\pi}{3}
$$

### 求解三角不等式

利用**单位圆**或**函数图像**来解不等式：

> **例 7c：** 在 $[0, 2\pi)$ 上解 $\sin\theta > \frac{1}{2}$。

**步骤：**
1. 先找等号成立的点：$\sin\theta = \frac{1}{2}$ 的解为 $\theta = \frac{\pi}{6}$ 和 $\frac{5\pi}{6}$。
2. 在单位圆上，$\sin\theta > \frac{1}{2}$ 对应 $y$-坐标大于 $\frac{1}{2}$ 的弧段。
3. 在 $[0, 2\pi)$ 上，解为 $\left(\frac{\pi}{6},\; \frac{5\pi}{6}\right)$。
4. 若考虑所有实数，加上周期性：$\left(\frac{\pi}{6} + 2\pi k,\; \frac{5\pi}{6} + 2\pi k\right),\; k \in \mathbb{Z}$。

> **例 7d：** 在 $[0, 2\pi)$ 上解 $\cos\theta \le -\frac{1}{2}$。

1. 等号成立处：$\theta = \frac{2\pi}{3}$ 和 $\frac{4\pi}{3}$。
2. 在单位圆上，$\cos\theta \le -\frac{1}{2}$ 对应 $x$-坐标 $\le -\frac{1}{2}$ 的弧段。
3. 解为 $\left[\frac{2\pi}{3},\; \frac{4\pi}{3}\right]$。

### 重要原则

- 解不等式时，先在 $[0, 2\pi)$ 或 $[0, \pi)$（对 $\tan$）上找到区间，再结合周期性推广。
- 涉及 $\tan$ 的不等式时，在单个周期 $(-\pi/2, \pi/2)$ 上分析后再通过 $+\pi k$ 推广。

---

## 🔹 3.11 — The Secant, Cosecant, and Cotangent Functions 正割、余割、余切

### 定义

**正割（Secant）：**

$$
\sec\theta = \frac{1}{\cos\theta},\quad \cos\theta \neq 0
$$

**余割（Cosecant）：**

$$
\csc\theta = \frac{1}{\sin\theta},\quad \sin\theta \neq 0
$$

**余切（Cotangent）：**

$$
\cot\theta = \frac{1}{\tan\theta} = \frac{\cos\theta}{\sin\theta},\quad \sin\theta \neq 0
$$

### 关键特征

| 函数 | 定义域限制 | 垂直渐近线 | 值域 | 周期 |
|:----:|:----------:|:----------:|:----:|:----:|
| $\sec\theta$ | $\cos\theta \neq 0$ | $\theta = \frac{\pi}{2} + k\pi$ | $(-\infty, -1] \cup [1, \infty)$ | $2\pi$ |
| $\csc\theta$ | $\sin\theta \neq 0$ | $\theta = k\pi$ | $(-\infty, -1] \cup [1, \infty)$ | $2\pi$ |
| $\cot\theta$ | $\sin\theta \neq 0$ | $\theta = k\pi$ | $\mathbb{R}$，相邻渐近线间**递减** | $\pi$ |

> **注意：** $\sec\theta$ 和 $\csc\theta$ 的图像永远不会取到 $(-1, 1)$ 之间的值，其图形是 $\cos$ 和 $\sin$ 图像取倒数后得到的 U 形曲线。

---

## 🔹 3.12 — Equivalent Representations of Trigonometric Functions 三角函数的等价表示

### 毕达哥拉斯恒等式（Pythagorean Identity）

由单位圆上的勾股定理：

$$
\sin^2\theta + \cos^2\theta = 1
$$

**常用变形：**

$$
\tan^2\theta + 1 = \sec^2\theta \quad\Longrightarrow\quad \tan^2\theta = \sec^2\theta - 1
$$

$$
\cot^2\theta + 1 = \csc^2\theta \quad\Longrightarrow\quad \cot^2\theta = \csc^2\theta - 1
$$

### 和角公式（Sum Identities）

**正弦和角公式：**

$$
\sin(\alpha + \beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta
$$

**余弦和角公式：**

$$
\cos(\alpha + \beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta
$$

### 差角公式（Difference Identities）

$$
\sin(\alpha - \beta) = \sin\alpha\cos\beta - \cos\alpha\sin\beta
$$

$$
\cos(\alpha - \beta) = \cos\alpha\cos\beta + \sin\alpha\sin\beta
$$

### 倍角公式（Double-Angle Identities）

令 $\alpha = \beta = \theta$：

$$
\sin(2\theta) = 2\sin\theta\cos\theta
$$

$$
\cos(2\theta) = \cos^2\theta - \sin^2\theta = 1 - 2\sin^2\theta = 2\cos^2\theta - 1
$$

### 示例

> **例 8：** 使用和角公式求 $\sin\frac{7\pi}{12}$。

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

## 🔹 3.13 — Trigonometry and Polar Coordinates 三角学与极坐标

### 极坐标系

极坐标以有序对 $(r, \theta)$ 表示点的位置：
- $r$ = 点到原点的距离（半径，通常 $r \geq 0$）
- $\theta$ = 从正 $x$-轴到点所在射线的角度

同一个点在极坐标系中可以有多种表示方式（例如 $(r, \theta)$ 和 $(-r, \theta + \pi)$ 表示同一点）。

### 极坐标 ↔ 直角坐标 转换

**极坐标 → 直角坐标：**

$$
\begin{cases}
x = r\cos\theta \\[4pt]
y = r\sin\theta
\end{cases}
$$

**直角坐标 → 极坐标：**

$$
\begin{cases}
r = \sqrt{x^2 + y^2} \\[6pt]
\theta =
\begin{cases}
\arctan\dfrac{y}{x}, & x > 0 \\[8pt]
\arctan\dfrac{y}{x} + \pi, & x < 0 \\[8pt]
\dfrac{\pi}{2}, & x = 0,\; y > 0 \\[8pt]
-\dfrac{\pi}{2}\;\left(\text{或 } \dfrac{3\pi}{2}\right), & x = 0,\; y < 0
\end{cases}
\end{cases}
$$

> 上述 $\theta$ 的完整分支实质上等价于 $\operatorname{atan2}(y, x)$ 函数。

### 复数与极坐标

复数 $a + bi$ 的极坐标形式（模-幅角形式）：

$$
a + bi = r(\cos\theta + i\sin\theta),\quad \text{其中 } r = \sqrt{a^2 + b^2},\quad \theta = \operatorname{atan2}(b, a)
$$

### 示例

> **例 9：** 将 $(x, y) = (1, \sqrt{3})$ 转换为极坐标。

$$
r = \sqrt{1^2 + (\sqrt{3})^2} = \sqrt{4} = 2
$$

$$
\theta = \arctan\frac{\sqrt{3}}{1} = \frac{\pi}{3}\quad (\text{因 } x > 0)
$$

极坐标为 $\left(2,\; \dfrac{\pi}{3}\right)$。

---

## 🔹 3.14 — Polar Function Graphs 极函数图像

### 极函数 $r = f(\theta)$

极函数由输入-输出对 $(\theta, r)$ 构成：
- **输入：** 角度 $\theta$
- **输出：** 半径 $r$

### 图像特征

- 输入值变化 $\rightarrow$ 从正 $x$-轴旋转的角度变化
- 输出值变化 $\rightarrow$ 到原点距离的变化
- 可通过限制 $\theta$ 的定义域来选取图像的特定部分

### 常见极函数图形

| 类型 | 形式示例 | 图像特征 |
|:----:|:---------|:---------|
| **圆** | $r = a$ | 半径为 $|a|$ 的圆 |
| **玫瑰线** | $r = a\sin(n\theta)$ 或 $r = a\cos(n\theta)$ | $n$ 为奇数时有 $n$ 瓣，偶数时有 $2n$ 瓣 |
| **心形线** | $r = a(1 \pm \sin\theta)$ 或 $r = a(1 \pm \cos\theta)$ | 心形图案 |
| **直线** | $\theta = \alpha$ | 过原点的射线 |

---

## 🔹 3.15 — Rates of Change in Polar Functions 极函数的变化率

### 半径变化分析

对于极函数 $r = f(\theta)$：

| $f(\theta)$ 符号 | 增减性 | 距离原点 |
|:---------------:|:------:|:--------:|
| $> 0$ | 递增 | **增加** |
| $< 0$ | 递减 | **增加** |
| $> 0$ | 递减 | **减少** |
| $< 0$ | 递增 | **减少** |

若函数在某区间内由增变减或由减变增 $\rightarrow$ 存在**极值点**（距离原点最近或最远的点）。

### 平均变化率

$r$ 关于 $\theta$ 在区间 $[\theta_1, \theta_2]$ 上的**平均变化率**为：

$$
\frac{\Delta r}{\Delta \theta} = \frac{f(\theta_2) - f(\theta_1)}{\theta_2 - \theta_1}
$$

- **几何意义：** 表示角度每增加 1 弧度时半径的平均变化量（单位：半径/弧度）
- 可用于估计区间内函数的值

### 示例

> **例 10：** 对极函数 $r = 2 + 3\sin\theta$，求 $\theta$ 从 $0$ 到 $\dfrac{\pi}{2}$ 的平均变化率。

$$
f(0) = 2 + 3\sin(0) = 2,\quad f\left(\frac{\pi}{2}\right) = 2 + 3\sin\left(\frac{\pi}{2}\right) = 2 + 3 = 5
$$

$$
\text{平均变化率} = \frac{5 - 2}{\frac{\pi}{2} - 0} = \frac{3}{\frac{\pi}{2}} = \frac{6}{\pi} \approx 1.91
$$

这意味着在此区间内，角度每增加 1 弧度，半径平均增加约 $1.91$ 单位。

---

## 📋 Unit 3 核心公式速查表

### 基本定义

$$
\sin\theta = y,\quad \cos\theta = x,\quad \tan\theta = \frac{y}{x} = \frac{\sin\theta}{\cos\theta}
$$

### 正弦型函数一般形式

$$
f(\theta) = a\sin(b\theta - c) + d \quad\text{或}\quad f(\theta) = a\cos(b\theta - c) + d
$$

$$
\text{振幅} = |a|,\quad \text{周期} = \frac{2\pi}{|b|},\quad \text{相位移动} = \frac{c}{b},\quad \text{中线 } y = d
$$

### 正切函数

$$
\tan\theta = \frac{\sin\theta}{\cos\theta},\quad \text{周期} = \pi
$$

$$
f(\theta) = a\tan(b\theta - c) + d,\quad \text{周期} = \frac{\pi}{|b|}
$$

### 倒数三角函数

$$
\sec\theta = \frac{1}{\cos\theta},\quad \csc\theta = \frac{1}{\sin\theta},\quad \cot\theta = \frac{\cos\theta}{\sin\theta}
$$

### 毕达哥拉斯恒等式

$$
\sin^2\theta + \cos^2\theta = 1,\quad \tan^2\theta + 1 = \sec^2\theta,\quad \cot^2\theta + 1 = \csc^2\theta
$$

### 和/差/倍角公式

$$
\sin(\alpha \pm \beta) = \sin\alpha\cos\beta \pm \cos\alpha\sin\beta
$$

$$
\cos(\alpha \pm \beta) = \cos\alpha\cos\beta \mp \sin\alpha\sin\beta
$$

$$
\sin(2\theta) = 2\sin\theta\cos\theta,\quad \cos(2\theta) = \cos^2\theta - \sin^2\theta
$$

### 极坐标 ↔ 直角坐标

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

### 平均变化率（极函数）

$$
\frac{\Delta r}{\Delta \theta} = \frac{f(\theta_2) - f(\theta_1)}{\theta_2 - \theta_1}
$$

---

> **总结：** Unit 3 从**周期现象**出发，通过**单位圆**引入三角函数，深入探讨**正弦型函数**的变换与建模，再拓展到**正切函数**、**倒数三角函数**、**三角恒等式**、**反三角函数**与**三角方程（含不等式）**，最后走进**极坐标系**，完成从直角坐标到极坐标的跨越。掌握这些内容，即掌握了 AP Precalculus 约 $30$–$35\%$ 的考试内容。🎯
