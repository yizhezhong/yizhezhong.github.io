---
title: "2 - 基础"
date: 2023-02-12T03:02:31+00:00
description: 基础
menu:
  sidebar:
    name: 2 - 基础
    identifier: real-analysis-note-2-1
    parent: real-analysis-notes-2
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["数学","分析","实分析","笔记"]
categories: ["Basic"]
---

##### **定理 2.1.2**  

a) 如果 $z + a = a$ 对于某些 $z, a \in \mathbb{R}$，则 $z = 0$。  
b) 如果 $u \cdot b = b$ 对于某些 $u, b \in \mathbb{R}, b \ne 0$，则 $u = 1$。  
c) 如果 $a \in \mathbb{R}$，则 $a \cdot 0 = 0$  
证明：  
（占位符）

</br>

##### **定理 2.1.3**

a) 如果 $a \cdot b = 1$ 对于某些 $a, b \in \mathbb{R}, a \ne 0$，则 $b = 1/a$。  
b) 如果 $a \cdot b = 0$ 对于某些 $a, b \in \mathbb{R}$，则 $a$ 和 $b$ 中至少有一个为 0。  
证明：  
（占位符）  

</br>

##### **定义**

有理数是 $\mathbb{R}$ 的一个元素，可以写成 $b/a \in \mathbb{R}$ 的形式，其中 $a, b \in \mathbb{Z}$ 和 $a \ne 0$。 符号 $\mathbb{Q}$ 表示 $\mathbb{R}$ 中所有有理数的集合。  

</br>

##### **定理 2.1.4**

满足 $r^2 = 2$ 的数 r 不可能是有理数。  
证明：  
（占位符）

</br>

##### **2.1.5 $\mathbb{R}$的顺序属性**

存在 $\mathbb{P} \subseteq \mathbb{R}, \mathbb{P} \ne \emptyset$，满足：  
i) 加法闭包 
ii) 乘法闭包  
iii) 三分属性：如果 $a \in \mathbb{R}$，则恰好满足以下条件之一：  
$$
a\in \mathbb{P}, \ \ \ \ a = 0, \ \ \ \ -a \in \mathbb{P}
$$
</br>

##### **定义 2.1.6**

让$a, b \in \mathbb{R}$。  
a) 如果 $a - b \in \mathbb{P}$，那么我们写 $a > b$ 或 $b < a$。  
b) 如果 $a - b \in \mathbb{P} \cup \{0\}$，那么我们写 $a \geq b$ 或 $b \leq a$。  

</br>

##### **定理 2.1.7**  

让$a, b , c \in \mathbb{R}$。  
a) 如果 $a > b$ 和 $b > c$，则 $a > c$。  
b) 如果 $a > b$，则 $a + c > b + c$。  
c) 如果 $a > b$ 和 $c > 0$，则 $ca > cb$。  
如果 $a < b$ 和 $c < 0$，则 $ca < cb$。  
证明：  
（占位符）

</br>

##### **定理 2.1.8**

a) 如果 $a \in \mathbb{R}$ 和 $a \ne 0$，则 $a^2 > 0$。  
b) $1 > 0$。  
c) 如果 $n \in \mathbb{N}$，则 $n > 0$。  
证明：  
（占位符）

</br>

##### **定理 2.1.9**

如果 $a \in \mathbb{R}$ 满足每个 $\varepsilon > 0$ 的 $0 \le a < \varepsilon$，则 $a = 0$。  
证明：  
（占位符）

</br>

##### **定理 2.1.10**

如果 $ab > 0$，则要么  
i) $a > 0$ 和 $b > 0$，或  
ii) $a < 0$ 和 $b < 0$。  
证明：  
（占位符）

</br>

##### **推论 2.1.11**

如果 $a, b < 0$，则要么  
i) $a < 0$ 和 $b > 0$，或  
ii) $a > 0$ 和 $b < 0$。  

</br>

##### **定义**

$a \in \mathbb{R}$ 的绝对值 $|a|$ 定义为  
$$
|a| := 
\begin{cases}
a \ \ \ \ \ if \ \ a \ge 0 \\
-a \ \ if \ \ a < 0
\end{cases}
$$
</br>

##### **定理 2.2.2**

让 $a, b, c \in \mathbb{R}$, $c \ge 0$ 然后  
a) $|ab| = |a||b|$,  
b) $|a|^2 = a^2$,  
c) $|a| \le c$ 当且仅当 $-c \le a \le c$,  
d) $-|a| \le a \le |a|$。  
证明：  
（占位符）

</br>

##### **定理 2.2.3（三角不等式）**

如果 $a, b \in \mathbb{R}$，则 $|a + b| \le |a| + |b|$。  
证明：  
（占位符）

</br>

##### **推论 2.2.4**

如果 $a, b \in \mathbb{R}$，则  
a) $||a| - |b|| \le |a - b|$,  
b) $|a - b| \le |a| + |b|$。  

</br>

##### **推论 2.2.5**

让$a_1, a_2, ..., a_n \in \mathbb{R}$ 。 然后
$$
| \sum_{k = 1}^n a_k | \le \sum_{k = 1}^n |a_k|.
$$
</br>

##### **定义2.2.7**

让 $a \in \mathbb{R}$ 和 $\varepsilon > 0$。 那么集合 $V_\varepsilon (a) := \{x \in \mathbb{R} : |x - a| < \varepsilon \}$ 称为 $a$ 的 $\varepsilon$ 邻域。

</br>

##### **定理 2.2.8**

让$a \in \mathbb{R}$。 如果每个 $\varepsilon > 0$ 对应 $x \in V_\varepsilon (a)$，则 $x = a$。  
证明：  
（占位符）

</br>

##### **定义 2.3.1 和 2.3.2**

让$S \subseteq \mathbb{R}, S \ne \emptyset$。  
a) $S$ 的上限是一个数字 $u$，使得所有 $s \in S$ 的 $u \ge s$。 如果 $S$ 至少有一个上界，则称它在上界。  
b) $S$ 的下界是一个数字 $w$，使得所有 $s \in S$ 的 $w \le s$。 如果 $S$ 至少有一个下界，则称它在下界。  
c) 如果 $S$ 既有上界又有下界，则称它是有界的。 否则，它被称为是无界的。  
d) 如果 $S$ 在上面有界，那么 $S$ 的上界 $u$ 被称为 $S$ 的上界（最小上界），如果 $u \le v$ 对于 $S$ 的每个上界 $v$. 我们用 $sup \ S$ 表示 S 的上确界。  
e) 如果 $S$ 在下方有界，则 $S$ 的下界 $w$ 被称为 $S$ 的下界（最大下界），如果 $w \ge t$ 对于 $S$ 的每个下界 $t$. 我们用 $inf \ S$ 表示 S 的下确界。  

</br>

##### **引理 2.3.3**

让$S \subseteq \mathbb{R}, S \ne \emptyset$。 那么 $u$ 是 $sup \ S$ 当且仅当  
i) $u \ge s$ 对所有 $s \in S$，  
ii) 如果 $v < u$，则存在 $s' \in S$ 使得 $v < s'$。

</br>

##### **引理 2.3.4**

让$S \subseteq \mathbb{R}, S \ne \emptyset$。 那么 $u$ 是 $supS$ 当且仅当对于每个 $\varepsilon > 0$ 存在 $s_\varepsilon \in S$ 使得 $s_\varepsilon > u - \varepsilon$。

</br>

##### **2.3.6 $\mathbb{R}$的完整性属性**

上面有界的每个非空集 $S \subseteq \mathbb{R}$ 在 $\mathbb{R}$ 中都有一个上界。

</br>

##### **2.4.3 阿基米德性质**

如果 $x \in \mathbb{R}$，则存在 $n_x \in \mathbb{N}$ 使得 $x \le n_x$。

</br>

##### **推论 2.4.4**

如果 $S := \{ 1/n : n \in \mathbb{N} \}$，则 $inf \ S = 0$。

</br>

##### **推论 2.4.5**

如果 $x > 0$，则存在 $n_x \in \mathbb{N}$ 使得 $0 < 1/n_x < x$。

</br>

##### **推论 2.4.6**

如果 $x > 0$，则存在 $n_x \in \mathbb{N}$ 使得 $n_x - 1 \le x < n_x$。

</br>

##### **定理 2.4.7**

存在 $x \in \mathbb{P}$ 使得 $x^2 = 2$。  
证明：  
（占位符）

</br>

###### **推论**

如果 $x, y > 0$ 和 $y - x > 1$，则存在 $m \in \mathbb{N}$ 使得 $x < m < y$。  
证明：由于 $y - x > 1$，我们有 $x + 1 < y$。 将推论 2.6 应用于 x > 0，因此存在 $n_x \in \mathbb{N}$ 使得 $n_x - 1 \le x < n_x$。 所以 $n_x \le x + 1 < n_x + 1$。 现在，我们有 $x < n_x \le x + 1 < y$。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **定理2.4.8（密度定理）**

对于任何具有 $x < y$ 的 $x, y \in \Reals$，存在 $r \in \mathbb{Q}$ 使得 $x < r < y$。  
证明：如果 $x = 0$，根据推论 2.5，存在 $n_y \in \mathbb{N}$ 使得 $0 < 1/n_y < y$。 由于 $n_y \in \mathbb{N}$，我们有 $1/n_y \in \mathbb{Q}$。  
请注意，如果 $0 < x < r < y$， $r \in \mathbb{Q}$，我们可以得到 $-y < -r < -x < 0$ 使得 $-r \in \mathbb{Q}$。 因此，不失一般性，令$x > 0$。 将推论 2.5 应用于 $y - x > 0$，因此存在 $n \in \mathbb{N}$ 使得 $0 < 1/n < y - x$。 然后我们有 $ny - nx > 1$。 根据定理 2.11，存在 $m \in \mathbb{N}$ 使得 $nx < m < ny$。 它遵循 $x < m/n < y$，其中 $m/n \in \mathbb{Q}$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **推论 2.4.9**

对于任何具有 $x < y$ 的 $x, y \in \Reals$，存在 $z \in \mathbb{R} \backslash \mathbb{Q}$ 使得 $x < z < y$。  

</br>

##### **定义**

设 $a, b \in \mathbb{R}$ 为 $a < b$。  
开区间 $(a, b)$ 定义为
$$
(a, b) := \{x \in \mathbb{R} : a < x < b\},
$$
其中点 a 和 b 称为区间 $(a, b)$ 的端点。  
具有端点 $a$ 和 $b$ 的闭区间 $[a, b]$ 定义为  
$$
[a, b] := \{x \in \mathbb{R} : a \le x \le b\}.
$$
端点为 $a$ 和 $b$ 的半开区间定义为
$$
[a, b) := \{x \in \mathbb{R} : a \le x < b\},
$$
和
$$
(a, b] := \{x \in \mathbb{R} : a < x \le b\}.
$$
上述区间都是有界的，长度由 $b - a$ 定义。 If $a = b$、开区间 $(a, a) = \emptyset$ 和闭区间 $[a, a] = {a}$。  
无限开区间 $(a, \infty)$ 和 $(-\infty, b)$ 定义为
$$
(a, \infty) := \{x \in \mathbb{R} : x > a\},
$$
和
$$
(-\infty, b) := \{x \in \mathbb{R} : x < b\}.
$$
无限闭区间 $[a, \infty)$ 和 $(-\infty, b]$ 定义为
$$
[a, \infty) := \{x \in \mathbb{R} : x \ge a\},
$$
和
$$
(-\infty, b] := \{x \in \mathbb{R} : x \le b\}.
$$
没有端点的无限区间定义为
$$
(-\infty, \infty) := \mathbb{R}
$$
请注意，$-\infty$ 和 $\infty$ 都不是 $\mathbb{R}$ 的元素，而只是方便的符号。

</br>

##### **间隔的特征**

如果 $x, y \in I$ 与 $x < y$ 和 $I$ 是一个区间，那么对于任何 $t \in \mathbb{R}$ 使得 $t \in [x, y]$，我们有 $t \in I$。

</br>

##### **定理2.5.1（刻画定理）**

如果 $S \subseteq \mathbb{R}$ 包含至少两个点满足
$$
if \ x, y \in S \ and \ x < y, \ then \ [x, y] \subseteq S,
$$
那么 $S$ 是一个区间。  
证明：  
（占位符）

</br>

##### **定义**

区间序列 $I_n, n \in \mathbb{N}$ 称为嵌套，如果
$$
I_1 \supseteq I_2 \supseteq \ ... \ \supseteq I_n \supseteq I_{n+1} \supseteq \ ...,
$$
也就是说，所有 $n \in \mathbb{N}$ 的 $I_n \supseteq I_{n+1}$。

</br>

###### **例子**

为 $n \in \mathbb{N}$ 定义 $I_n := [0, 1/n]$。 由于 $I_n \supseteq I_{n+1}$ 对应所有 $n \in \mathbb{N}$，因此 $I_n$ 是嵌套的。 请注意，0 包含在所有区间中。 事实上，0 是唯一的公共点。  
证明：  
对于任何 $x > 0$，根据推论 2.4.5，存在 $n_x \in \mathbb{N}$ 使得 $0 < 1/n_x < x$。 回想一下 $I_{n_x} := [0, 1/n_x] = \{x \in \mathbb{R} : 0 \le x \le 1/n_x\}$。 所以，$x \notin I_{n_x}$.<span style="float:right;">$_{Q.E.D.}$</span>
我们写 $\cap^{\infty}_{n = 1} I_n = \{0\}$。  
请注意，如果 $J_{n_x} := (0, 1/n_x)$ 对应 $n \in \mathbb{N}$，则 $\cap^{\infty}_{n = 1} J_n = \emptyset$。

</br>

##### **2.5.2 嵌套区间属性**

如果 $I_n := [a_n, b_n]$ 是闭有界区间的嵌套序列，则存在 $\xi \in \mathbb{R}$ 使得 $\xi \in I_n$ 对所有 $n \in \mathbb{N}$。  
证明：  
（占位符）

</br>

##### **定理 2.5.3**

如果 $I_n := [a_n, b_n]$ 是闭有界区间的嵌套序列，使得
$$
inf\{b_n - a_n : n \in \mathbb{N}\} = 0,
$$
那么所有 $n \in \mathbb{N}$ 的 $\xi \in I_n$ 都是唯一的。  
证明：  
（占位符）

</br>

##### **定理 2.5.4**

集合 $\mathbb{R}$ 不可数。  
证明：  
（占位符）

</br>

##### **定理 2.5.5**

单位区间 [0, 1] 不可数。  
证明：  
（占位符）

</br>

</br>

##### **参考资料**

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 