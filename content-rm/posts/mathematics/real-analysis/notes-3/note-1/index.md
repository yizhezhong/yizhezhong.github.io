---
title: "3 - 基础"
date: 2023-02-18T04:49:46+00:00
description: 基础
menu:
  sidebar:
    name: 3 - 基础
    identifier: real-analysis-note-3-1
    parent: real-analysis-notes-3
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["数学","分析","实分析","笔记"]
categories: ["Basic"]
---

##### **定义 3.1.1**

实数序列（在 $\mathbb{R}$ 中的序列）是从 $\mathbb{N}$ 到 $\mathbb{R}$ 的函数。

</br>

##### **定义 3.1.3**

实数序列 $X = (x_n)$ 收敛于 $x$，当且仅当存在 $x \in \mathbb{R}$，使得对于所有 $n > k_\varepsilon$，都有 $|x_n - x| < \varepsilon$，其中 $\varepsilon > 0$ 是任意的，$k_\varepsilon \in \mathbb{N}$ 依赖于 $\varepsilon$。数字 $x$ 被称为 $X$ 的极限，$X$ 收敛于 $x$。否则，序列是发散的。

</br>

##### **定理 3.1.4**

如果一个序列 $X = (x_n)$ 的极限存在，那么它是唯一的。  
证明：  
假设序列 $X$ 有两个极限 $x$ 和 $x'$......

</br>

##### **定理 3.3.2（单调收敛定理）**

在$\mathbb{R}$中的单调数列当且仅当有界时收敛。进一步地：  
a）如果$X = (x_n)$是有界的递增数列，则
$$
lim(x_n) = sup\{x_n : n \in \mathbb{N} \}.
$$
b）如果$Y = (y_n)$是有界的递减数列，则
$$
lim(y_n) = inf\{y_n : n \in \mathbb{N} \}.
$$
证明：  
定理3.2.2表明每个收敛的数列都是有界的。如果$\mathbb{R}$中的单调数列是有界的，则它要么是递增的，要么是递减的。  
a）如果$X = (x_n)$是有界的递增数列，则存在上界$M$，使得对于所有的$n \in \mathbb{N}$都有$x_n < M$。因此，根据完备性质2.3.6，它有一个上确界$x^* = sup{x_n : n \in \mathbb{N} }$。对于任意的$\varepsilon > 0$，存在$k \in \mathbb{N}$使得$x^* - \varepsilon < x_k$。然后，对于所有$n \ge k$，我们有$x^* - \varepsilon < x_k \le x_n \le x^* < x^* + \varepsilon$。因此，$X$收敛于$x^*$。  
b）如果$Y = (y_n)$是有界的递减数列，则$X = (x_n) := -Y = (-y_n)$是递增数列。从a）中，我们有$lim(x_n) = sup{x_n : n \in \mathbb{N} } = sup{-y_n : n \in \mathbb{N} } = -inf{y_n : n \in \mathbb{N} }$。因此，$limY = -limX = inf{y_n : n \in \mathbb{N} }$。 <span style="float:right;">$ _{Q.E.D.}$</span>

</br>

##### **定理3.4.7 (单调子序列定理)**

如果 $X = (x_n)$ 是 $\mathbb{R}$ 中的一个数列，则 $X$ 有一个单调子序列。  
证明：  
我们称 $x_m$ 是峰值，如果 $x_m \ge x_n$ 对于所有 $n \ge m$ 成立。  
情况1：如果 $X$ 有无限多个峰值，则我们可以按递增的下标列出它们 $x_{m_1}, x_{m_2}, ..., x_{m_k}, ....$。由于每个术语都是峰值，我们有
$$
x_{m_1} \ge x_{m_2} \ge \ ... \ \ge x_{m_k} \ge \ ....
$$
这个序列是 $X$ 的单调递减子序列。  
情况2：如果 $X$ 只有有限多个峰值，则我们可以按递增的下标列出它们 $x_{m_1}, x_{m_2}, ..., x_{m_r}$。对于 $k \in \mathbb{N}$，令 $s_k := m_r + k$。则 $x_{s_k}$ 对于所有 $k \in \mathbb{N}$ 都不是峰值。因此，$x_{s_{k+1}} \ge x_{s_k}$ 对于所有 $k \in \mathbb{N}$ 成立。因此，我们可以获得一个单调递增的序列 $x_{s_1}, x_{s_2}, ... , x_{s_k}, x_{s_{k+1}}, ...$，它是 $X$ 的一个子序列。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **定理3.4.8 (Bolzano-Weierstrass定理)**

在$\mathbb{R}$中的有界序列具有收敛的子序列。  
证明1：
设$X=(x_n)$是$\mathbb{R}$中的有界序列。由定理3.4.7可知，$X$具有单调子序列。由于该子序列也是有界的，根据定理3.3.2，该子序列是收敛的。  
证明2：  
设$X=(x_n)$是$\mathbb{R}$中的有界序列。则集合${x_n:n \in \mathbb{N}}$包含在区间$I:=[a,b]$中。取$n_1:=1$，并将$I_1$一分为二为$I'_1$和$I''_1$。然后将${n \in \mathbb{N}:n>n_1}$分成
$$
A_1 := \{n \in \mathbb{N} : n > n_1, n \in I'_1\}, \ B_1 := \{n \in \mathbb{N} : n > n_1, n \in I''_1\}
$$
则$A_1$和$B_1$中至少有一个是无限的。假设$A_1$是无限的，则我们可以通过取$n_2:=\inf A_1$将$I_2$一分为二为$I'_2$和$I''_2$，并将$A_1$分成$A_2$和$B_2$。以此类推，我们可以得到一系列嵌套区间$I_1\supseteq I_2\supseteq\cdots\supseteq I_k\supseteq\cdots$和序列$X$的子序列$(x_{n_k})$，使得对于$k\in \mathbb{N}$，$x_{n_k}\in I_k$。注意到$I_k$的长度，即$b_k-a_k$，为$(b-a)/2^{k-1}$。因此，$\inf{b_n-a_n:n\in \mathbb{N}}=0$。根据定理2.5.3，对于所有的$k\in\mathbb{N}$，都存在唯一的公共点$\xi \in I_k$。因为$x_{n_k}$和$\xi$都在$I_k$中，所以我们有$|x_{n_k}-\xi|\leq(b-a)/2^{k-1}$。因此，子序列$(x_{n_k})$收敛于$\xi$。 <span style="float:right;">$_{\text{Q.E.D.}}$</span>

</br>

##### **定义 3.5.1**

Cauchy 序列是一个实数序列 $(x_n)$，满足对于任意 $\varepsilon > 0$，存在 $N(\varepsilon) \in \mathbb{N}$，使得对于任意自然数 $n, m \ge H(\varepsilon)$，有 $|x_n - x_m| < \varepsilon$。

</br>

##### **定理 3.5.5 (Cauchy 收敛准则)**

一个实数序列收敛当且仅当它是一个 Cauchy 序列。  
证明：  
根据引理 3.5.3，如果一个实数序列收敛，那么它是一个 Cauchy 序列。反之，如果 $X := (x_n)$ 是一个 Cauchy 序列，则根据引理 3.5.4，它是有界的。根据定理 3.4.8，存在一个子序列 $X' = (x_{n_k})$ 收敛于某个 $x^* \in \mathbb{R}$。由于 $X$ 是一个 Cauchy 序列，对于任意 $\varepsilon > 0$，存在 $H(\varepsilon/2)$ 使得对于 $n, m \ge H(\varepsilon/2)$，有 $|x_n - x_m| < \varepsilon/2$。由于 $X'$ 收敛于 $x^*$，存在自然数 $n_K \ge H(\varepsilon/2)$，使得 $|x_{n_K} - x^*| < \varepsilon/2$。因此，对于 $n \ge H(\varepsilon/2)$，有 $|x_n - x_{n_K}| < \varepsilon/2$。因此，$|x_n - x^*| = |x_n - x_{n_K} + x_{n_K} - x^*| \le |x_n - x_{n_K}| + |x_{n_K} - x^*| < \varepsilon/2 + \varepsilon/2 = \varepsilon$。因此，序列 $X$ 是收敛的。<span style="float:right;">$_{Q.E.D.}$</span>

</br>

</br>

###### **参考资料**

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
