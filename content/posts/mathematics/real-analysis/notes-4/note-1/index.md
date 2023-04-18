---
title: "4 - 基础"
date: 2023-03-21T20:53:49+00:00
description: 基础
menu:
  sidebar:
    name: 4 - 基础
    identifier: real-analysis-note-4-1
    parent: real-analysis-notes-4
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["数学","分析","实分析","笔记"]
categories: ["Basic"]
---



##### **定义 4.1.1**

设 $A \subseteq \mathbb{R}$，若对于任意 $\delta > 0$，都存在 $x \in A, x \ne c$，满足 $|x - c| < \delta$，则点 $c \in \mathbb{R}$ 是 $A$ 的一个聚点。  
重新表述：若对于任意 $\delta > 0$，在每个 $\delta-$邻域 $V_\delta (c) = (c-\delta, c+\delta)$ 中，都存在 $x \in A, x \ne c$，则点 $c \in \mathbb{R}$ 是 $A$ 的一个聚点。

</br>

##### **定理 4.1.2**

设 $A \subseteq \mathbb{R}$。点 $c \in \mathbb{R}$ 是 $A$ 的聚点，当且仅当存在数列 $(a_n)$ 满足 lim$(a_n) = c$ 且 $a_n \ne c$ 对所有 $n \in \mathbb{N}$ 成立。  
证明：  
如果 $c \in \mathbb{R}$ 是 $A$ 的聚点，则对于任意 $n \in \mathbb{N}$，都存在 $a_n \in A, a_n \ne c$，满足 $|a_n - c| < 1/n$。由定理 3.1.10，因为 lim$(1/n) = 0$，所以有 lim$(a_n) = c$。  
反之，如果存在数列 $(a_n)$ 满足 lim$(a_n) = c$ 且 $a_n \ne c$ 对所有 $n \in \mathbb{N}$ 成立，则对于任意 $\delta > 0$，都存在 $N(\delta) \in \mathbb{N}$，满足对所有 $n > N(\delta)$，都有 $|a_n - c| < \delta$。由于 $a_n \in A$ 且 $a_n \ne c$，点 $c$ 是 $A$ 的聚点。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **定义 4.1.4**

设 $A \subseteq \mathbb{R}$，$c \in \mathbb{R}$ 是 $A$ 的聚点。对于函数 $f: A \rightarrow \mathbb{R}$，如果存在实数 $L$，使得对于任意 $\varepsilon > 0$，都存在 $\delta > 0$，使得对于任意满足 $0 < |x-c| < \delta$ 的 $x \in A$，都有 $|f(x) - L| < \varepsilon$，则称 $L$ 是 $f$ 在 $c$ 处的极限。如果 $f$ 在 $c$ 处收敛于 $L$，我们也称为：
$$
L = \lim_{x \to c}f(x) \ or \ L = \lim_{x \to c}f.
$$
我们也可以说："$f(x)$ 当 $x$ 趋近于 $c$ 时趋近于 $L$"，表示为
$$
f(x) \rightarrow L \ as \ x \rightarrow c.
$$
如果 $f$ 在 $c$ 处不存在极限，我们称 $f$ 在 $c$ 处发散。

</br>

##### **定理 4.1.5**

如果 $f: A \rightarrow \mathbb{R}$，$c$ 是 $A$ 的聚点，则 $f$ 在 $c$ 处的极限唯一。  
proof:  
设 $L$ 和 $L'$ 都是 $f$ 在 $c$ 处的极限。则对于任意 $\varepsilon > 0$，都存在 $\delta(\varepsilon/2) > 0$，使得对于任意满足 $0 < |x-c| < \delta(\varepsilon/2)$ 的 $x \in A$，都有 $|f(x) - L| < \varepsilon/2$。同样地，存在 $\delta'(\varepsilon/2) > 0$，使得对于任意满足 $0 < |x-c| < \delta'(\varepsilon/2)$ 的 $x \in A$，都有 $|f(x) - L'| < \varepsilon/2$。令 $\delta := \inf{\delta(\varepsilon/2), \delta'(\varepsilon/2)}$，则对于任意满足 $0 < |x-c| < \delta$ 的 $x \in A$，都有
$$
|L - L'| \le |L - f(x)| + |f(x) + L'| < \varepsilon/2 + \varepsilon/2 = \varepsilon.
$$
由于 $\varepsilon > 0$ 是任意的，故有 $L - L' = 0$，即 $L = L'$。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **定理 4.1.6**

设 $f:A\rightarrow \mathbb{R}$，$c$ 是 $A$ 的聚点，则下列陈述等价： i) $\lim_{x \to c}f(x) = L$。 ii) 对于任意 $\varepsilon$ 邻域 $V_\varepsilon(L)$，都存在 $\delta$ 邻域 $V_\delta(c)$，使得对于任意 $x \in V_\delta(c) \cap A$，其中 $x\neq c$，有 $f(x) \in V_\varepsilon(L)$。  
证明：  
根据定义，$\lim_{x \to c}f(x) = L$ 相当于对于任意 $\varepsilon > 0$，都存在 $\delta > 0$，使得对于任意 $x \in A$，满足 $0 < | x - c| < \delta$，有 $|f(x) - L| < \varepsilon$。我们可以建立等价的陈述：对于任意 $\varepsilon > 0$，都存在 $\delta > 0$，使得对于任意 $x \in A$，满足 $x \in V_\delta(c) \backslash {c}$，有 $f(x) \in V_\epsilon(L)$。证毕。

</br>

##### **定理 4.1.8 (顺序准则)**

设$f: A \rightarrow \mathbb{R}$，$c$ 是$A$的一个聚点。则以下陈述等价：  
i) $\lim_{x \to c}f(x) = L$。  
ii) 对于任意收敛于$c$的序列$(x_n)$，其中$n \in \mathbb{N}$，且对于所有$n \in \mathbb{N}$，都有$x_n \ne c$，序列$(f(x_n))$ 收敛于$L$。  
证明：  
假设 $\lim_{x \to c}f(x) = L$。假设序列 $(x_n)$ 在$A$中收敛于$c$，其中$n \in \mathbb{N}$，且对于所有$n \in \mathbb{N}$，都有$x_n \ne c$。给定 $\varepsilon > 0$。根据定义 4.1.4，存在 $\delta > 0$，使得对于任意 $x \in A$，且 $0 < | x - c | < \delta$，都有 $| f(x) - L | < \varepsilon$。由于序列 $(x_n)$ 收敛于 $c$，因此存在 $K(\delta) \in \mathbb{N}$，使得对于所有 $n > K(\delta)$，都有 $| x_n - c| < \delta$。那么对于所有 $n > K(\delta)$，都有 $| f(x) - L | < \varepsilon$。因此，序列 $(f(x_n))$ 收敛于$L$。  
反过来，我们采用反证法来证明。如果i)不成立，则存在$L$的一个$\varepsilon$-邻域，使得对于$c$的所有$\delta$-邻域，都存在一个点$x_\delta \in A \cap V_\delta(c)$，且 $x_\delta \ne c$，但 $f(x_\delta) \notin V_\varepsilon(L)$。因此，对于所有 $n \in \mathbb{N}$，$c$的$(1/n)$-邻域，即 $V_{1/n}(c) = {x \in A : 0 < |x - c| < 1/n}$，都存在一个点 $x_{n} \in A \cap V_{1/n}(c)$，且 $x_{n} \ne c$，但 $f(x_{n}) \notin V_\varepsilon(L) = {y \in \mathbb{R} : |x - L| < \varepsilon}$。因此，序列 $(x_n)$ 收敛于 $c$，但 $f(x_n)$ 不收敛于 $L$。<span style="float:right;">$_{证毕}$</span>

</br>

##### **4.1.9 发散准则**

设 $A \subseteq \mathbb{R}$，$f: A \rightarrow \mathbb{R}$，$c \in \mathbb{R}$ 是 $A$ 的簇点。  
a) 如果 $L \in \mathbb{R}$，则 $f$ 在 $c$ 处没有极限当且仅当存在序列 $(x_n)$，其中 $(x_n)$ 中所有元素均不等于 $c$，$(x_n)$ 收敛于 $c$，但 $(f(x_n))$ 不收敛于 $L$。  
b) 函数 $f$ 在 $c$ 处没有极限当且仅当存在序列 $(x_n)$，其中 $(x_n)$ 中所有元素均不等于 $c$，$(x_n)$ 收敛于 $c$，但 $(f(x_n))$ 在 $\mathbb{R}$ 中不收敛。  
证明：  
（占位）

</br>

##### **定义 4.2.1**

设 $A \subseteq \mathbb{R}$，$f: A \rightarrow \mathbb{R}$，$c \in \mathbb{R}$ 是 $A$ 的簇点。若存在 $V_\delta(c)$ 和常数 $M>0$，使得对于所有 $x \in A \cap V_\delta(c)$，$|f(x)| \le M$，则我们称 $f$ 在 $c$ 的某个邻域上有界。

</br>

##### **定理 4.2.2**

设 $A \subseteq \mathbb{R}$，$f: A \rightarrow \mathbb{R}$。如果 $f$ 在 $c$ 处有极限，则 $f$ 在 $c$ 的某个邻域上有界。  
证明：  
设 $L := \lim_{x \to c}f$。那么，对于任意的 $\varepsilon > 0$，存在 $\delta > 0$，使得对于任意满足 $0 < |x-c|<\delta$ 的 $x \in A$，我们有 $|f(x) - L| < \varepsilon$。于是，根据推论 2.2.4 (a) 和定理 2.2.2 (d)，我们有 $|f(x)|-|L| \le ||f(x)| - |L|| \le |f(x)-L|<\varepsilon$。因此，如果 $c \notin A$，则 $f$ 由 $M=|L|+\varepsilon$ 划定的范围内有界。如果 $c \in A$，我们可以取 $M=\operatorname{sup}{|f(c)|,|L|+\varepsilon}$。

</br>

##### **定义 4.2.3**

设 $A \subseteq \mathbb{R}$，$f$ 和 $g$ 是定义在 $A$ 到 $\mathbb{R}$ 的函数。对于所有 $x \in A$，我们定义它们的和 $f+g$，差 $f-g$ 和积 $fg$ 为
$$
(f + g)(x) := f(x) + g(x), \\
(f - g)(x) := f(x) - g(x), \\
(fg)(x) := f(x)g(x).
$$
若 $b \in \mathbb{R}$，则对于所有 $x \in A$，我们定义它们的倍数 $bf$ 为
$$
(bf)(x) := bf(x).
$$
如果 $h(x) \neq 0$ 对于所有 $x \in A$，则对于所有 $x \in A$，我们定义它们的商 $f/h$ 为
$$
(\frac{f}{h})(x) := \frac{f(x)}{h(x)}.
$$
</br>

##### **定理 4.2.4**

设 $A \subseteq \mathbb{R}$，$f$ 和 $g$ 是 $A$ 到 $\mathbb{R}$ 的函数，$c \in \mathbb{R}$ 是 $A$ 的聚点，$b \in \mathbb{R}$。  
a) 如果 $\lim_{x \to c}f(x) = L$ 和 $\lim_{x \to c}g(x) = M$，那么
$$
\lim_{x \to c}(f + g)(x) = L + M, \\
\lim_{x \to c}(f - g)(x) = L - M, \\
\lim_{x \to c}(fg)(x) = LM, \\
\lim_{x \to c}(bf)(x) = bL.
$$
b) 如果 $h: A \rightarrow \mathbb{R}$，对于所有 $x \in A$，$h(x) \neq 0$，并且 $\lim_{x \to c}h(x) = H \neq 0$，那么
$$
\lim_{x \to c}(\frac{f}{h})(x) = \frac{L}{H}.
$$
证明：  
（待定）

</br>

##### **定理 4.2.6**

设 $A\subseteq \mathbb{R}$，$f:A\rightarrow\mathbb{R}$，$c\in\mathbb{R}$ 是 $A$ 的集簇点。如果对于所有 $x\in A,x\neq c$ 都有 $a\leq f(x)\leq b$，且 $\lim_{x\to c}f(x)$ 存在，则有 $a\leq\lim_{x\to c}f(x)\leq b$。  
证明： （暂缺）

</br>

##### **定理 4.2.7（夹逼定理）**

设 $A\subseteq \mathbb{R}$，$f,g,h$ 是 $A$ 上的函数，值域为 $\mathbb{R}$，$c\in\mathbb{R}$ 是 $A$ 的集簇点。如果对于所有 $x\in A,x\neq c$ 都有 $f(x)\leq g(x)\leq h(x)$，且 $\lim_{x\to c}f(x)=L=\lim_{x\to c}h(x)$，则有 $\lim_{x\to c}g(x)=L$。  
证明： （暂缺）

</br>

##### **定理 4.2.9**

设 $A\subseteq \mathbb{R}$，$f:A\rightarrow\mathbb{R}$，$c\in\mathbb{R}$ 是 $A$ 的集簇点。如果 $\lim_{x\to c}f(x)>0$ [或 $\lim_{x\to c}f(x)<0$]，则存在 $c$ 的某个邻域 $V_\delta(c)$，使得对于所有 $x\in A\cap V_\delta(c),x\neq c$，都有 $f(x)>0$ [或 $f(x)<0$]。  
证明： （暂缺）

</br>

##### **定理 4.3.2**

设$A \subseteq \mathbb{R}$，$f : A \rightarrow \mathbb{R}$，$c \in \mathbb{R}$是$A \cap (c, \infty)$的一个聚点。则以下命题等价：  
i) $\lim_{x \to c+}f = L$。  
ii) 对于所有收敛于$c$的序列$(x_n)$，其中$x_n \in A \cap (c, \infty), n \in \mathbb{N}$，序列$(f(x_n))$都收敛于$L$。  
证明：  
假设$\lim_{x \to c+}f(x) = L$。设序列$(x_n)$在$A \cap (c, \infty)$中收敛于$c$。给定$\varepsilon > 0$。根据定义4.3.1，存在$\delta > 0$，对于任意满足$0 < x - c < \delta$的$x \in A$，都有$| f(x) - L | < \varepsilon$。由于序列$(x_n)$收敛于$c$，存在$K(\delta) \in \mathbb{N}$，使得对于所有$n > K(\delta)$，都有$x_n - c = |x_n - c| < \delta$。因此，对于所有$n > K(\delta)$，都有$| f(x) - L | < \varepsilon$。因此，序列$(f(x_n))$收敛于$L$。  
反过来，我们通过反证法证明。如果i)不成立，则存在一个$\varepsilon$邻域，对于所有$\delta$邻域，都存在一个点$x_\delta \in A \cap V_\delta(c), x_\delta > c$，但$f(x_\delta) \notin V_\varepsilon(L)$。因此，对于所有$n \in \mathbb{N}$，$(1/n)$-邻域$V_{1/n}(c) = {x \in A : 0 < |x - c| < 1/n}$都存在一个点$x_{n} \in A \cap V_{1/n}(c), x_{n} > c$，但$f(x_{n}) \notin V_\varepsilon(L) = {y \in \mathbb{R} : |x - L| < \varepsilon}$。因此，序列$(x_n)$收敛于$c$，但$f(x_n)$不收敛于$L$。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

</br>

###### **参考资料**

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
