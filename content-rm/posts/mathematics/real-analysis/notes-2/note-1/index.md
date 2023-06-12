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

a) 如果存在 $z, a \in \mathbb{R}$ 使得 $z + a = a$，那么 $z = 0$。
b) 如果存在 $u, b \in \mathbb{R}, b \neq 0$ 使得 $u \cdot b = b$，那么 $u = 1$。
c) 对于任意 $a \in \mathbb{R}$，有 $a \cdot 0 = 0$。
证明：
(占位符)

</br>

##### **定理 2.1.3**

a) 如果存在 $a, b \in \mathbb{R}, a \neq 0$ 使得 $a \cdot b = 1$，那么 $b = 1/a$。
b) 如果存在 $a, b \in \mathbb{R}$ 使得 $a \cdot b = 0$，那么 $a$ 和 $b$ 中至少有一个为 0。
证明：
(占位符)

</br>

##### **定义**

有理数是指可以写成 $b/a$ 的形式的 $\mathbb{R}$ 中的元素，其中 $a, b \in \mathbb{Z}$ 且 $a \neq 0$。记号 $\mathbb{Q}$ 表示所有有理数构成的集合。

</br>

##### **定理 2.1.4**

满足 $r^2 = 2$ 的数 $r$ 不能是有理数。
证明：
(占位符)

</br>

##### **2.1.5 $\mathbb{R}$ 的序性质**

存在 $\mathbb{P} \subseteq \mathbb{R}, \mathbb{P} \neq \emptyset$ 满足：
i) 加法封闭性
ii) 乘法封闭性
iii) 三歧性：如果 $a \in \mathbb{R}$，则以下三者之一成立：

$$
a\in \mathbb{P}, \ \ \ \ a = 0, \ \ \ \ -a \in \mathbb{P}
$$
</br>

##### **定义 2.1.6**

设 $a, b \in \mathbb{R}$。
a) 如果 $a - b \in \mathbb{P}$，那么我们写作 $a > b$ 或 $b < a$。
b) 如果 $a - b \in \mathbb{P} \cup {0}$，那么我们写作 $a \geq b$ 或 $b \leq a$。

</br>

##### **定理 2.1.7**

设 $a, b, c \in \mathbb{R}$。  
a) 若 $a > b$ 且 $b > c$，则 $a > c$。  
b) 若 $a > b$，则 $a + c > b + c$。  
c) 若 $a > b$ 且 $c > 0$，则 $ca > cb$。  
    若 $a < b$ 且 $c < 0$，则 $ca < cb$。

证明：（待补充）

</br>

##### **定理 2.1.8**

a) 若 $a \in \mathbb{R}$ 且 $a \ne 0$，则 $a^2 > 0$。  
b) $1 > 0$。   
c) 若 $n \in \mathbb{N}$，则 $n > 0$。

证明：（待补充）

</br>

##### **定理 2.1.9**

若 $a \in \mathbb{R}$ 满足对于任意 $\varepsilon > 0$ 都有 $0 \le a < \varepsilon$，则 $a = 0$。

证明：（待补充）

</br>

##### **定理 2.1.10**

若 $ab > 0$，则以下命题之一成立：  
i) $a > 0$ 且 $b > 0$；  
ii) $a < 0$ 且 $b < 0$。  
证明：（待补充）

</br>

##### **引理 2.1.11**

若 $a, b < 0$，则以下命题之一成立：  
i) $a < 0$ 且 $b > 0$；  
ii) $a > 0$ 且 $b < 0$。

</br>

##### 定义

对于 $a \in \mathbb{R}$，定义绝对值 $|a|$ 如下：

$$
|a| := 
\begin{cases}
a \ \ \ \ \ if \ \ a \ge 0 \\
-a \ \ if \ \ a < 0
\end{cases}
$$
</br>

##### **定理 2.2.2**

设 $a, b, c \in \mathbb{R}$，$c \ge 0$，则  
a) $|ab| = |a||b|$，  
b) $|a|^2 = a^2$，  
c) $|a| \le c$ 当且仅当 $-c \le a \le c$，  
d) $-|a| \le a \le |a|$。  
证明：  
（占位符）

</br>

##### **定理 2.2.3（三角不等式）**

设 $a, b \in \mathbb{R}$，则 $|a + b| \le |a| + |b|$。  
证明：  
（占位符）  

</br>

##### **推论 2.2.4**

设 $a, b \in \mathbb{R}$，则  
a) $||a| - |b|| \le |a - b|$，  
b) $|a - b| \le |a| + |b|$。  

</br>

##### **推论 2.2.5**

设 $a_1, a_2, ..., a_n \in \mathbb{R}$。则

$$
| \sum_{k = 1}^n a_k | \le \sum_{k = 1}^n |a_k|.
$$
</br>

##### **定义2.2.7**

设 $a \in \mathbb{R}$ 和 $\varepsilon > 0$。则称集合 $V_\varepsilon (a) := {x \in \mathbb{R} : |x - a| < \varepsilon }$ 为 $a$ 的 $\varepsilon$ 邻域。

</br>

##### **定理 2.2.8**

设 $a \in \mathbb{R}$。如果对于任意的 $\varepsilon > 0$，$x \in V_\varepsilon (a)$，则 $x = a$。  
证明：  
（占位符）

</br>

##### **定义 2.3.1 & 2.3.2**

设 $S \subseteq \mathbb{R}, S \ne \emptyset$  
a) 若存在一个数 $u$，使得对于所有 $s \in S$，有 $u \ge s$，则 $u$ 是 $S$ 的一个上界。若 $S$ 至少有一个上界，则称 $S$ 是有上界的。   
b) 若存在一个数 $w$，使得对于所有 $s \in S$，有 $w \le s$，则 $w$ 是 $S$ 的一个下界。若 $S$ 至少有一个下界，则称 $S$ 是有下界的。   
c) 若 $S$ 既有上界又有下界，则称 $S$ 是有界的；否则，称 $S$ 是无界的。   
d) 若 $S$ 有上界，则若 $u$ 是 $S$ 的一个上界，且对于所有 $S$ 的上界 $v$，有 $u \le v$，则称 $u$ 是 $S$ 的上确界（或最小上界），记作 $sup \ S$。   
e) 若 $S$ 有下界，则若 $w$ 是 $S$ 的一个下界，且对于所有 $S$ 的下界 $t$，有 $w \ge t$，则称 $w$ 是 $S$ 的下确界（或最大下界），记作 $inf \ S$。

</br>

##### **引理 2.3.3**

设 $S \subseteq \mathbb{R}, S \ne \emptyset$。则 $u$ 是 $S$ 的上确界，当且仅当  
i) $u \ge s$，对于所有 $s \in S$， ii) 若 $v < u$，则存在 $s' \in S$，使得 $v < s'$。

</br>

##### **引理 2.3.4**

设 $S \subseteq \mathbb{R}, S \ne \emptyset$。则 $u$ 是 $S$ 的上确界，当且仅当对于每个 $\varepsilon > 0$，存在 $s_\varepsilon \in S$，  使得 $s_\varepsilon > u - \varepsilon$。

</br>

##### **2.3.6 $\mathbb{R}$ 的完备性质**

对于每个非空的 $S \subseteq \mathbb{R}$，如果 $S$ 有上界，则 $S$ 在 $\mathbb{R}$ 中有上确界。

</br>

##### **2.4.3 阿基米德性质**

如果 $x \in \mathbb{R}$，则存在 $n_x \in \mathbb{N}$，使得 $x \le n_x$。

</br>

##### **推论 2.4.4**

如果 $S := { 1/n : n \in \mathbb{N} }$，则 $inf \ S = 0$。

</br>

##### **推论 2.4.5**

如果 $x > 0$，则存在 $n_x \in \mathbb{N}$，使得 $0 < 1/n_x < x$。

</br>

##### **推论 2.4.6**

如果 $x > 0$，则存在 $n_x \in \mathbb{N}$，使得 $n_x - 1 \le x < n_x$。

</br>

##### **定理 2.4.7**

存在 $x \in \mathbb{P}$，使得 $x^2 = 2$。   
证明： （占位符）

</br>

###### **推论**

如果 $x, y > 0$ 且 $y - x > 1$，则存在 $m \in \mathbb{N}$，使得 $x < m < y$。   
证明：  
由于 $y - x > 1$，因此 $x + 1 < y$。对 $x > 0$ 应用推论 2.6，因此存在 $n_x \in \mathbb{N}$，使得 $n_x - 1 \le x < n_x$。因此 $n_x \le x + 1 < n_x + 1$。现在，我们有 $x < n_x \le x + 1 < y$。<span style="float:right;">$_{证毕}$</span>

</br>

##### **定理 2.4.8（密度定理）**

对于任意的 $x, y \in \Reals$，其中 $x < y$，存在 $r \in \mathbb{Q}$，使得 $x < r < y$。  
证明：  
如果 $x = 0$，则根据推论 2.5，存在 $n_y \in \mathbb{N}$，使得 $0 < 1/n_y < y$。由于 $n_y \in \mathbb{N}$，因此 $1/n_y \in \mathbb{Q}$。请注意，如果 $0 < x < r < y$，其中 $r \in \mathbb{Q}$，我们可以有 $-y < -r < -x < 0$，使得 $-r \in \mathbb{Q}$。因此，不失一般性，假设 $x > 0$。对 $y - x > 0$ 应用推论 2.5，因此存在 $n \in \mathbb{N}$，使得 $0 < 1/n < y - x$。然后我们有 $ny - nx > 1$。根据定理 2.11，存在 $m \in \mathbb{N}$，使得 $nx < m < ny$。由此得出 $x < m/n < y$，其中 $m/n \in \mathbb{Q}$。<span style="float:right;">$_{证毕}$</span>

</br>

##### **推论 2.4.9**

对于任意的 $x, y \in \Reals$，其中 $x < y$，存在 $z \in \mathbb{R} \backslash \mathbb{Q}$，使得 $x < z < y$。

</br>

##### **定义**

设$a,b \in \mathbb{R}$且$a < b$  
开区间$(a,b)$定义为
$$
(a, b) := \{x \in \mathbb{R} : a < x < b\},
$$
其中点$a$和$b$被称为区间$(a,b)$的端点。  
闭区间$[a,b]$定义为，端点为$a$和$b$：
$$
[a, b] := \{x \in \mathbb{R} : a \le x \le b\}.
$$
半开区间定义为，端点为$a$和$b$：

$$
[a, b) := \{x \in \mathbb{R} : a \le x < b\},
$$
以及

$$
(a, b] := \{x \in \mathbb{R} : a < x \le b\}.
$$
上述区间都是有界的，长度由$b-a$定义。如果$a=b$，则开区间$(a,a) = \emptyset$，闭区间$[a,a] = {a}$。

无限开区间$(a,\infty)$和$(-\infty,b)$定义为：

$$
(a, \infty) := \{x \in \mathbb{R} : x > a\},
$$
以及

$$
(-\infty, b) := \{x \in \mathbb{R} : x < b\}.
$$
无限闭区间$[a,\infty)$和$(-\infty,b]$定义为：

$$
[a, \infty) := \{x \in \mathbb{R} : x \ge a\},
$$
以及

$$
(-\infty, b] := \{x \in \mathbb{R} : x \le b\}.
$$
没有端点的无限区间定义为：

$$
(-\infty, \infty) := \mathbb{R}
$$
请注意，$-\infty$和$\infty$都不是$\mathbb{R}$的元素，而只是方便的符号。

</br>

##### **区间特性**

如果$x, y \in I$，且$x<y$，其中$I$为区间，则对于任何$t \in \mathbb{R}$，如果$t \in [x,y]$，则$t \in I$。

</br>

##### **定理 2.5.1（刻画定理）**

如果 $S \subseteq \mathbb{R}$ 包含至少两个满足条件的点：

$$
如果 \ x, y \in S \ 且 \ x < y, \ 那么 \ [x, y] \subseteq S,
$$
那么 $S$ 是一个区间。

证明：
（占位符）

</br>

##### **定义**

如果 $I_n, n \in \mathbb{N}$ 是一系列区间，满足

$$
I_1 \supseteq I_2 \supseteq \ ... \ \supseteq I_n \supseteq I_{n+1} \supseteq \ ...,
$$
即对于所有 $n \in \mathbb{N}$，都有 $I_n \supseteq I_{n+1}$，则称 $I_n$ 为嵌套的区间。

</br>

##### **例子**

定义 $I_n := [0, 1/n]$，$n \in \mathbb{N}$。由于对于所有 $n \in \mathbb{N}$，都有 $I_n \supseteq I_{n+1}$，所以 $I_n$ 是嵌套的。请注意，0 包含在所有区间中。实际上，0 是唯一的这样的共同点。

证明：  
对于任何 $x > 0$，由推论 2.4.5，存在 $n_x \in \mathbb{N}$，使得 $0 < 1/n_x < x$。回顾一下，$I_{n_x} := [0, 1/n_x] = {x \in \mathbb{R} : 0 \le x \le 1/n_x}$。因此，$x \notin I_{n_x}$。<span style="float:right;">$*{Q.E.D.}$</span>
我们写成 $\cap^{\infty}*{n = 1} I_n = {0}$。  
请注意，如果 $J_{n_x} := (0, 1/n_x)$，则 $\cap^{\infty}_{n = 1} J_n = \emptyset$。

</br>

##### **定理 2.5.2 嵌套区间性质**

如果 $I_n := [a_n, b_n]$ 是一系列闭合有界区间的嵌套序列，则存在 $\xi \in \mathbb{R}$，使得对于所有 $n \in \mathbb{N}$，都有 $\xi \in I_n$。

证明：
（占位符）

</br>

##### **定理 2.5.3**

如果 $I_n := [a_n, b_n]$ 是一系列闭合有界区间的嵌套序列，满足

$$
inf\{b_n - a_n : n \in \mathbb{N}\} = 0,
$$
那么 $\xi \in I_n$ 对于所有 $n \in \mathbb{N}$ 都是唯一的。

证明：
（占位符）

</br>

##### **定理 2.5.5**

单位区间 $[0,1]$ 不可列举。  
证明:  
(占位符)

</br>

</br>

##### **参考资料**

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 