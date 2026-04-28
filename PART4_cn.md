# 📦 UNIT 4: Functions Involving Parameters, Vectors, and Matrices

> **⚠️ 重要提示**：Unit 4 为**拓展内容**（Additional Topics Available to Schools），**不纳入 AP 考试范围**，由学校根据当地要求自行决定是否教授。

---

## 🔷 4.1 — Parametric Functions（参数函数）

### 核心概念

一个**参数函数**将一个输入（参数 $t$）映射到一个输出有序对：

$$f(t) = (x(t),\; y(t))$$

- $x(t)$ 和 $y(t)$ 是两个**独立**的关于 $t$ 的函数
- $t$ 是参数（通常代表时间）
- 图像由所有点 $(x(t), y(t))$ 按 $t$ 递增顺序**描绘而成**（不是线性插值连线，而是点集构成的曲线）

### 数值表生成

给定参数值 $t_i$ 在定义域内，可生成数值表：

$$(x_i, y_i) = (x(t_i),\; y(t_i))$$

### 定义域与图像

$$\text{domain}(f) = \{t \in \mathbb{R} \mid t \text{ 有意义}\}$$

- 定义域常被限制，导致图像有起点和终点
- 参数函数的图像**可能不通过垂线检验**（vertical line test），但它仍然是一个函数（因为每个 $t$ 唯一确定一个 $(x,y)$）

### 📌 示例

> **例**：给定 $f(t) = (t^2,\; t+1)$，$t \in [0, 3]$
>
> | $t$ | $(x(t), y(t))$ |
> |:---:|:--------------:|
> | $0$ | $(0, 1)$ |
> | $1$ | $(1, 2)$ |
> | $2$ | $(4, 3)$ |
> | $3$ | $(9, 4)$ |
>
> 这些点按 $t$ 递增顺序描绘出一条抛物线弧。

---

## 🔷 4.2 — Parametric Functions Modeling Planar Motion（参数函数建模平面运动）

### 核心概念

参数函数可用于建模**粒子在平面上的运动**：

$$f(t) = (x(t),\; y(t))$$

- 图像表示粒子在时刻 $t$ 的**位置**
- $x(t)$：水平位置分量；$y(t)$：垂直位置分量

### 关键特征

| 特征 | 方法 |
|------|------|
| 水平极值 | $x(t)$ 的最大/最小值 |
| 垂直极值 | $y(t)$ 的最大/最小值 |
| $x$ 截距 | 解 $y(t)=0$ 得 $t$，再代入 $x(t)$ 得 $x$ 坐标 |
| $y$ 截距 | 解 $x(t)=0$ 得 $t$，再代入 $y(t)$ 得 $y$ 坐标 |

### 📌 示例

> **例**：$f(t) = (\cos t,\; \sin t)$，$t \in [0, 2\pi]$
>
> - $x(t)$ 最大值 $= 1$（$t=0$），最小值 $= -1$（$t=\pi$）
> - $y(t)$ 最大值 $= 1$（$t=\frac{\pi}{2}$），最小值 $= -1$（$t=\frac{3\pi}{2}$）
> - $x$ 截距：$y(t)=0 \Rightarrow \sin t = 0 \Rightarrow t=0,\pi,2\pi$，代入得点 $(1,0)$ 和 $(-1,0)$
> - $y$ 截距：$x(t)=0 \Rightarrow \cos t = 0 \Rightarrow t=\frac{\pi}{2},\frac{3\pi}{2}$，代入得点 $(0,1)$ 和 $(0,-1)$

---

## 🔷 4.3 — Parametric Functions and Rates of Change（参数函数与变化率）

### 运动方向分析

随着参数 $t$ 增加，粒子的运动方向由 $x(t)$ 和 $y(t)$ 的单调性决定：

$$
\begin{aligned}
x(t) \text{ 随 } t \text{ 增大而增大} &\Rightarrow \text{向右移动} \\
x(t) \text{ 随 } t \text{ 增大而减小} &\Rightarrow \text{向左移动} \\
y(t) \text{ 随 } t \text{ 增大而增大} &\Rightarrow \text{向上移动} \\
y(t) \text{ 随 } t \text{ 增大而减小} &\Rightarrow \text{向下移动}
\end{aligned}
$$

### 平均变化率

在区间 $[t_1, t_2]$ 上：

$$\text{AROC}_x = \frac{x(t_2) - x(t_1)}{t_2 - t_1}$$

$$\text{AROC}_y = \frac{y(t_2) - y(t_1)}{t_2 - t_1}$$

**曲线的斜率**（当 $\text{AROC}_x \neq 0$ 时）：

$$\text{slope} = \frac{y(t_2) - y(t_1)}{x(t_2) - x(t_1)} = \frac{\text{AROC}_y}{\text{AROC}_x}$$

### 同一曲线的不同参数化

同一条平面曲线可以用不同的参数函数以不同方向、不同速度遍历。

### 📌 示例

> **例**：$f(t) = (t,\; t^2)$，$t \in [0, 2]$
>
> 在 $[0, 2]$ 上：$x(t)$ 从 $0$ 增大到 $2$（向右），$y(t)$ 从 $0$ 增大到 $4$（向上），所以粒子向右上方运动。
>
> 平均变化率：$\text{AROC}_x = \frac{2-0}{2-0}=1$，$\text{AROC}_y = \frac{4-0}{2-0}=2$
>
> 曲线斜率 $= \frac{2}{1}=2$

---

## 🔷 4.4 — Parametrically Defined Circles and Lines（参数化定义的圆与直线）

### 单位圆（逆时针）

从点 $(1,0)$ 开始，绕原点逆时针一周：

$$(x(t),\; y(t)) = (\cos t,\; \sin t), \quad 0 \leq t \leq 2\pi$$

### 任意圆/椭圆（变换后）

通过变换可得到任意圆心、半径的圆或椭圆：

$$(x(t),\; y(t)) = (h + a\cos t,\; k + b\sin t)$$

- $(h, k)$：中心
- $a > 0$：水平方向半轴长度；$b > 0$：垂直方向半轴长度
- 若 $a = b$ 则为圆；若 $a \neq b$ 则为椭圆

### 直线的参数化

从点 $(x_1, y_1)$ 到点 $(x_2, y_2)$ 的线段：

$$(x(t),\; y(t)) = (x_1 + \Delta x \cdot t,\; y_1 + \Delta y \cdot t), \quad t \in [0,1]$$

其中 $\Delta x = x_2 - x_1$，$\Delta y = y_2 - y_1$。

更一般地：

$$(x(t),\; y(t)) = (x_1 + v_x t,\; y_1 + v_y t)$$

其中 $v_x$ 和 $v_y$ 是 $x$ 和 $y$ 关于 $t$ 的变化率。

### 📌 示例

> **例**：写出圆心在 $(2, -1)$、半径为 $3$ 的圆的参数方程。
>
> $$(x(t), y(t)) = (2 + 3\cos t,\; -1 + 3\sin t), \quad 0 \leq t \leq 2\pi$$
>
> **例**：从 $(1,2)$ 到 $(5,6)$ 的线段参数化。
>
> $$(x(t), y(t)) = (1 + 4t,\; 2 + 4t), \quad 0 \leq t \leq 1$$

---

## 🔷 4.5 — Implicitly Defined Functions（隐式定义函数）

### 核心概念

一个涉及两个变量的方程可以隐式地定义一个或多个函数：

$$F(x, y) = 0$$

### 求解显式形式

将方程解出其中一个变量，可以得到显式函数：

$$y = f(x) \quad \text{或} \quad x = g(y)$$

解出的函数图像是原方程图像的一部分或全部。

### 协变分析

对于隐式定义函数上的相邻有序对（当 $x$ 变化很小时）：

$$ \frac{\Delta y}{\Delta x} > 0 \Rightarrow x \text{ 和 } y \text{ 同时增加或同时减少} $$

$$ \frac{\Delta y}{\Delta x} < 0 \Rightarrow x \text{ 增加时 } y \text{ 减小（或反之）} $$

$$ \frac{\Delta y}{\Delta x} = 0 \Rightarrow \text{水平区间} $$

$$ \frac{\Delta x}{\Delta y} = 0 \Rightarrow \text{垂直区间} $$

### 📌 示例

> **例**：$x^2 + y^2 = 25$
>
> 解出 $y$：$y = \pm\sqrt{25 - x^2}$，定义域 $x \in [-5, 5]$
>
> 这定义了**两个**函数（上半圆和下半圆）。
>
> 在点 $(3,4)$ 附近：$x$ 增加时 $y$ 减小（$\frac{\Delta y}{\Delta x} < 0$）。

---

## 🔷 4.6 — Conic Sections（圆锥曲线）

### 抛物线（Parabola）

顶点在 $(h, k)$，$a \neq 0$：

**开口向上/下**：

$$y - k = a(x - h)^2$$

- $a > 0$：开口向上
- $a < 0$：开口向下

**开口向左/右**：

$$x - h = a(y - k)^2$$

- $a > 0$：开口向右
- $a < 0$：开口向左

### 椭圆（Ellipse）

中心在 $(h, k)$，水平半径 $a > 0$，垂直半径 $b > 0$：

$$\frac{(x - h)^2}{a^2} + \frac{(y - k)^2}{b^2} = 1$$

- 当 $a = b$ 时，椭圆退化为**圆**
- $a$：水平方向半轴长；$b$：垂直方向半轴长

### 双曲线（Hyperbola）

中心在 $(h, k)$，$a > 0$，$b > 0$：

**左右开口**：

$$\frac{(x - h)^2}{a^2} - \frac{(y - k)^2}{b^2} = 1$$

- $a$：实半轴长（从中心到顶点的距离）
- $b$：虚半轴长

*渐近线*：$y - k = \pm\frac{b}{a}(x - h)$

**上下开口**：

$$\frac{(y - k)^2}{a^2} - \frac{(x - h)^2}{b^2} = 1$$

- $a$：实半轴长（从中心到顶点的距离）
- $b$：虚半轴长

*渐近线*：$y - k = \pm\frac{a}{b}(x - h)$

### 📌 示例

> **例**：判断 $\frac{(x-1)^2}{4} + \frac{(y+2)^2}{9} = 1$ 的图形。
>
> 这是椭圆，中心 $(1,-2)$，$a=2$（水平半径），$b=3$（垂直半径）。
>
> **例**：$y - 3 = 2(x + 1)^2$ 是什么？
>
> 这是抛物线，顶点 $(-1, 3)$，开口向上。

---

## 🔷 4.7 — Parametrization of Implicitly Defined Functions（隐式函数的参数化）

### 核心思想

参数化 $(x(t), y(t))$ 满足隐式方程：代入后方程对定义域内所有 $t$ 成立。

### 显式函数的参数化

如果 $y = f(x)$，可参数化为：

$$(x(t), y(t)) = (t,\; f(t))$$

如果 $f$ 可逆，其反函数可参数化为：

$$(x(t), y(t)) = (f(t),\; t)$$

### 圆锥曲线的参数化

**椭圆**（中心 $(h,k)$，半径 $a>0, b>0$）：

$$(x(t), y(t)) = (h + a\cos t,\; k + b\sin t), \quad 0 \leq t \leq 2\pi$$

**双曲线**（左右开口，中心 $(h,k)$，$a>0, b>0$）：

$$(x(t), y(t)) = (h + a\sec t,\; k + b\tan t), \quad 0 \leq t \leq 2\pi,\; t \neq \frac{\pi}{2}, \frac{3\pi}{2}$$

> ⚠️ 注意：$\sec t$ 和 $\tan t$ 在 $t = \frac{\pi}{2}$ 和 $t = \frac{3\pi}{2}$ 处无定义，需排除这些点。

**双曲线**（上下开口，中心 $(h,k)$，$a>0, b>0$）：

$$(x(t), y(t)) = (h + a\tan t,\; k + b\sec t), \quad 0 \leq t \leq 2\pi,\; t \neq \frac{\pi}{2}, \frac{3\pi}{2}$$

### 📌 示例

> **例**：参数化 $y = x^2$，$x \in [-2, 2]$
>
> $$(x(t), y(t)) = (t,\; t^2), \quad -2 \leq t \leq 2$$
>
> **例**：参数化 $\frac{x^2}{9} + \frac{y^2}{4} = 1$
>
> $$(x(t), y(t)) = (3\cos t,\; 2\sin t), \quad 0 \leq t \leq 2\pi$$

---

## 🔷 4.8 — Vectors（向量）

### 向量定义

向量是**有向线段**。在平面中：

$$\overrightarrow{P_1P_2} = \langle a, b \rangle$$

其中 $a = x_2 - x_1$，$b = y_2 - y_1$。

- **起点**（tail）：$P_1$；**终点**（head）：$P_2$
- **零向量**：$\langle 0, 0 \rangle$

### 模长（Magnitude）

$$|\vec{v}| = \sqrt{a^2 + b^2}$$

### 标量乘法

$$k \cdot \langle a, b \rangle = \langle ka, kb \rangle$$

结果向量平行于原向量。

### 向量加法

$$\langle a_1, b_1 \rangle + \langle a_2, b_2 \rangle = \langle a_1 + a_2, \; b_1 + b_2 \rangle$$

图形上：三角形法则（首尾相连）。

### 点积（Dot Product）

$$\langle a_1, b_1 \rangle \cdot \langle a_2, b_2 \rangle = a_1a_2 + b_1b_2$$

**几何意义**：

$$\vec{u} \cdot \vec{v} = |\vec{u}|\,|\vec{v}|\cos\theta$$

其中 $\theta \in [0, \pi]$ 是两个向量之间的夹角。

**垂直条件**：若两个非零向量的点积为零，则 $\vec{u} \perp \vec{v}$。

### 单位向量

模长为 1 的向量。与 $\vec{v}$ 同方向的单位向量：

$$\hat{v} = \frac{\vec{v}}{|\vec{v}|}$$

### 基向量表示

$$\langle a, b \rangle = a\hat{i} + b\hat{j}$$

其中 $\hat{i} = \langle 1, 0 \rangle$，$\hat{j} = \langle 0, 1 \rangle$。

### 正弦与余弦定理

向量加法形成的三角形可用**正弦定理**和**余弦定理**求解。

### 📌 示例

> **例**：$\vec{u} = \langle 3, 4 \rangle$，$\vec{v} = \langle 1, -2 \rangle$
>
> $|\vec{u}| = \sqrt{3^2 + 4^2} = 5$
>
> $|\vec{v}| = \sqrt{1^2 + (-2)^2} = \sqrt{5}$
>
> $\vec{u} + \vec{v} = \langle 4, 2 \rangle$
>
> $\vec{u} \cdot \vec{v} = 3(1) + 4(-2) = 3 - 8 = -5$
>
> $\cos\theta = \frac{-5}{5 \cdot \sqrt{5}} = -\frac{1}{\sqrt{5}}$，所以 $\theta > 90^\circ$

---

## 🔷 4.9 — Vector-Valued Functions（向量值函数）

> 💡 本部分涉及变化率的概念。**速度向量**的严格定义需要微积分中的导数；此处以直观方式介绍其含义。

### 位置向量

粒子的位置可表示为向量值函数：

$$\vec{p}(t) = x(t)\hat{i} + y(t)\hat{j} \quad \text{或} \quad \vec{p}(t) = \langle x(t), y(t) \rangle$$

位置向量的模长给出粒子到原点的**距离**：

$$|\vec{p}(t)| = \sqrt{[x(t)]^2 + [y(t)]^2}$$

### 速度向量

速度向量描述了位置随时间的变化情况（需要微积分中的导数概念来严格定义，此处直观理解）：

$$\vec{v}(t) \text{ 的分量反映位置变化的快慢和方向}$$

- 若 $x(t)$ 随 $t$ 增大而增大 $\Rightarrow$ 向右移动
- 若 $x(t)$ 随 $t$ 增大而减小 $\Rightarrow$ 向左移动
- 若 $y(t)$ 随 $t$ 增大而增大 $\Rightarrow$ 向上移动
- 若 $y(t)$ 随 $t$ 增大而减小 $\Rightarrow$ 向下移动

速度向量的**模长**给出粒子的**速率**（speed）：

$$\text{speed} = |\vec{v}(t)| = \sqrt{\text{(水平变化率)}^2 + \text{(垂直变化率)}^2}$$

### 📌 示例

> **例**：$\vec{p}(t) = \langle 3\cos t, 2\sin t \rangle$
>
> 在 $t = \frac{\pi}{2}$ 时：位置 $\vec{p}(\frac{\pi}{2}) = \langle 0, 2 \rangle$，距离原点 $= 2$
>
> 在 $t = 0$ 时：$x(t)=3\cos t$ 从 $3$ 开始减小（向左趋势），$y(t)=2\sin t$ 从 $0$ 开始增大（向上趋势）

---

## 🔷 4.10 — Matrices（矩阵）

### 矩阵定义

一个 $n \times m$ 矩阵是有 $n$ 行 $m$ 列的数组。

$$A_{n \times m} = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1m} \\ a_{21} & a_{22} & \cdots & a_{2m} \\ \vdots & \vdots & \ddots & \vdots \\ a_{n1} & a_{n2} & \cdots & a_{nm} \end{bmatrix}$$

### 矩阵乘法

**条件**：第一个矩阵的列数等于第二个矩阵的行数。

若 $A$ 是 $n \times p$，$B$ 是 $p \times m$，则乘积 $C = AB$ 是 $n \times m$ 矩阵。

$$c_{ij} = \sum_{k=1}^{p} a_{ik} \cdot b_{kj}$$

即 $c_{ij}$ 是 $A$ 的第 $i$ 行与 $B$ 的第 $j$ 列的点积。

### 📌 示例

> **例**：$A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$，$B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}$
>
> $$AB = \begin{bmatrix} 1(5)+2(7) & 1(6)+2(8) \\ 3(5)+4(7) & 3(6)+4(8) \end{bmatrix} = \begin{bmatrix} 19 & 22 \\ 43 & 50 \end{bmatrix}$$

---

## 🔷 4.11 — The Inverse and Determinant of a Matrix（矩阵的逆与行列式）

### 单位矩阵（Identity Matrix）

$I$ 是对角线为 $1$、其余为 $0$ 的方阵：

$$I_{2\times 2} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$$

性质：$A \cdot I = A$，$I \cdot A = A$

### 逆矩阵

若 $A^{-1}$ 是 $A$ 的逆矩阵，则：

$$A \cdot A^{-1} = A^{-1} \cdot A = I$$

### $2 \times 2$ 矩阵的逆

若 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$，当 $\det(A) \neq 0$ 时：

$$A^{-1} = \frac{1}{\det(A)} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

### 行列式（Determinant）

对于 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$：

$$\det(A) = ad - bc$$

### 行列式的几何意义

若 $2 \times 2$ 矩阵的两列（或两行）是 $\mathbb{R}^2$ 中从原点出发的向量，则：

$$|\det(A)| = \text{由两向量张成的平行四边形的面积}$$

$\det(A) = 0 \iff$ 两向量**平行**（共线，面积为 $0$）。

### 可逆条件

$$A \text{ 可逆} \iff \det(A) \neq 0$$

### 📌 示例

> **例**：$A = \begin{bmatrix} 2 & 3 \\ 1 & 4 \end{bmatrix}$
>
> $\det(A) = 2(4) - 3(1) = 8 - 3 = 5 \neq 0$，所以可逆。
>
> $$A^{-1} = \frac{1}{5} \begin{bmatrix} 4 & -3 \\ -1 & 2 \end{bmatrix} = \begin{bmatrix} \frac{4}{5} & -\frac{3}{5} \\ -\frac{1}{5} & \frac{2}{5} \end{bmatrix}$$

---

## 🔷 4.12 — Linear Transformations and Matrices（线性变换与矩阵）

### 线性变换的定义

线性变换 $L: \mathbb{R}^2 \to \mathbb{R}^2$ 将输入向量映射到输出向量，输出的每个分量是输入分量的常数倍之和：

$$L\left(\begin{bmatrix} x \\ y \end{bmatrix}\right) = \begin{bmatrix} a_{11}x + a_{12}y \\ a_{21}x + a_{22}y \end{bmatrix}$$

### 零向量性质

$$L(\vec{0}) = \vec{0}$$

### 线性变换与矩阵的对应

每个线性变换 $L: \mathbb{R}^2 \to \mathbb{R}^2$ 对应唯一的 $2 \times 2$ 矩阵 $A$：

$$L(\vec{v}) = A\vec{v}$$

反之，每个 $2 \times 2$ 矩阵 $A$ 定义了一个线性变换。

### 批量变换

若 $A$ 是 $2 \times 2$ 变换矩阵，$V$ 是 $2 \times n$ 输入向量矩阵（即 $n$ 个输入向量排成 $2$ 行），则 $AV$ 是 $2 \times n$ 输出向量矩阵。

### 📌 示例

> **例**：$A = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix}$，$\vec{v} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}$
>
> $$L(\vec{v}) = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix} \begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} 2 \\ 6 \end{bmatrix}$$
>
> 这表示水平拉伸 2 倍、垂直拉伸 3 倍。

---

## 🔷 4.13 — Matrices as Functions（矩阵作为函数）

### 变换与矩阵的关联

线性变换 $(x, y) \mapsto (a_{11}x + a_{12}y, \; a_{21}x + a_{22}y)$ 关联矩阵：

$$\begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}$$

### 旋转矩阵

将向量逆时针旋转角度 $\theta$ 的变换：

$$R_\theta = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix}$$

### 单位向量的映射

线性变换对单位向量 $\hat{i} = \langle 1, 0 \rangle$ 和 $\hat{j} = \langle 0, 1 \rangle$ 的映射提供了确定关联矩阵的关键信息。

### 行列式与区域伸缩

$$|\det(A)| = \text{变换对区域面积的缩放倍数}$$

### 复合变换

两个线性变换的复合仍是线性变换。复合变换的矩阵是各变换矩阵的**乘积**：

$$L_2 \circ L_1 \quad \text{对应矩阵} \quad A_2 A_1$$

### 逆变换

若 $L(\vec{v}) = A\vec{v}$，则逆变换为：

$$L^{-1}(\vec{v}) = A^{-1}\vec{v}$$

满足 $L^{-1}(L(\vec{v})) = \vec{v}$。

### 📌 示例

> **例**：旋转 $90^\circ$ 的矩阵：
>
> $$R_{90^\circ} = \begin{bmatrix} \cos 90^\circ & -\sin 90^\circ \\ \sin 90^\circ & \cos 90^\circ \end{bmatrix} = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}$$
>
> 对 $\vec{v} = \langle 2, 3 \rangle$ 应用：
>
> $$\begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 2 \\ 3 \end{bmatrix} = \begin{bmatrix} -3 \\ 2 \end{bmatrix}$$
>
> 即点 $(2,3)$ 逆时针旋转 $90^\circ$ 后到达 $(-3,2)$。

---

## 🔷 4.14 — Matrices Modeling Contexts（矩阵建模情境）

### 状态转移模型

情境中给出两个状态之间的转移率（百分比变化），可构建转移矩阵来建模状态在离散时间间隔中的变化。

### 预测未来状态

设 $M$ 为转移矩阵，$\vec{s}_0$ 为初始状态向量，则：

$$\vec{s}_1 = M\vec{s}_0$$

$$\vec{s}_n = M^n \vec{s}_0$$

### 稳态（Steady State）

当经过多次转移后，状态分布不再变化：

$$M\vec{s} = \vec{s}$$

即 $\vec{s}$ 经过一次转移后保持不变。

### 预测过去状态

使用转移矩阵的**逆**：

$$\vec{s}_{-1} = M^{-1}\vec{s}_0$$

$$\vec{s}_{-n} = M^{-n}\vec{s}_0$$

### 📌 示例

> **例**：某城市每年有 $10\%$ 的居民从市区搬到郊区，$5\%$ 的居民从郊区搬到市区。
>
> 转移矩阵（第1行/列对应市区，第2行/列对应郊区）：
>
> $$M = \begin{bmatrix} 0.90 & 0.05 \\ 0.10 & 0.95 \end{bmatrix}$$
>
> 初始状态：$\vec{s}_0 = \begin{bmatrix} 1000 \\ 500 \end{bmatrix}$（市区1000人，郊区500人）
>
> 一年后：
>
> $$\vec{s}_1 = \begin{bmatrix} 0.90 & 0.05 \\ 0.10 & 0.95 \end{bmatrix} \begin{bmatrix} 1000 \\ 500 \end{bmatrix} = \begin{bmatrix} 900 + 25 \\ 100 + 475 \end{bmatrix} = \begin{bmatrix} 925 \\ 575 \end{bmatrix}$$
>
> 稳态求解：$M\vec{s} = \vec{s}$
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
> 两式等价，得 $s_2 = 2s_1$。即稳态比例为 $s_1 : s_2 = 1 : 2$。
>
> 总人口 $1500$，所以稳态时：市区 $500$ 人，郊区 $1000$ 人（$\frac{1}{3}$ 市区 : $\frac{2}{3}$ 郊区）。

---

## 📊 Unit 4 快速汇总

| Topic | 名称 | 核心概念 | 课时 |
|:-----:|------|---------|:----:|
| **4.1** | 参数函数 | $f(t) = (x(t), y(t))$ | 2 |
| **4.2** | 参数函数建模平面运动 | 位置、极值、截距 | 2 |
| **4.3** | 参数函数与变化率 | 方向分析、平均变化率、斜率 | 2 |
| **4.4** | 参数化定义的圆与直线 | 单位圆、任意圆、线段参数化 | 2 |
| **4.5** | 隐式定义函数 | $F(x,y)=0$、协变分析 | 2 |
| **4.6** | 圆锥曲线 | 抛物线、椭圆、双曲线方程 | 3 |
| **4.7** | 隐式函数的参数化 | 参数化圆锥曲线 | 2 |
| **4.8** | 向量 | 模长、加法、点积、单位向量 | 3 |
| **4.9** | 向量值函数 | 位置向量、速度向量、速率 | 1 |
| **4.10** | 矩阵 | 定义、矩阵乘法 | 2 |
| **4.11** | 矩阵的逆与行列式 | $\det(A)$、$A^{-1}$、几何意义 | 2 |
| **4.12** | 线性变换与矩阵 | $L(\vec{v}) = A\vec{v}$ | 1 |
| **4.13** | 矩阵作为函数 | 旋转、复合、逆变换 | 3 |
| **4.14** | 矩阵建模情境 | 转移矩阵、稳态 | 3 |
| | **总计** | | **28 课时** |

> 🎯 **Unit 4** 虽然不纳入 AP 考试，但它是衔接**大学线性代数**和**多元微积分**的重要桥梁！掌握好参数化、向量和矩阵的基础，将为后续学习打下坚实基础。
