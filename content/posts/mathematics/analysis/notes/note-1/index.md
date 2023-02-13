---
title: "（1）证明有理数集在实数域稠密"
date: 2023-02-12T03:02:31+00:00
description: 证明有理数在实数域稠密
menu:
  sidebar:
    name: （1）证明有理数在实数域稠密
    identifier: note-1
    parent: 分析笔记
    weight: 10
hero: images/posts/analysis-notes.jpg
tags: ["数学","分析","实分析","笔记"]
categories: ["Basic"]
---

##### **定理**

**对于满足 $x < y$ 的任何实数$x, y$，存在 $r \in \mathbb{Q}$ 使得 $x < r < y$。**

</br>

###### **引理 1**

如果 $x > 0$，则存在 $n_x \in \mathbb{N}$ 使得 $0 < 1/n_x < x$。

###### **引理 2**

如果 $x > 0$，则存在 $n_x \in \mathbb{N}$ 使得 $n_x - 1 \le x < n_x$。

###### **引理 3**

如果 $x, y > 0$ 且 $y - x > 1$，则存在 $m \in \mathbb{N}$ 使得 $x < m < y$。

###### **引理 3 的证明**

从 $y - x > 1$ 开始，我们有 $x + 1 < y$。 将引理 2 应用于 x > 0，因此存在 $n_x \in \mathbb{N}$ 使得 $n_x - 1 \le x < n_x$。 所以$n_x \le x + 1 < n_x + 1$。 现在，我们有 $x < n_x \le x + 1 < y$。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

###### **定理的证明**

如果 $x = 0$，根据引理 1，存在 $n_y \in \mathbb{N}$ 使得 $0 < 1/n_y < y$。 由于 $n_y \in \mathbb{N}$，我们有 $1/n_y \in \mathbb{Q}$。
我们注意到，如果 $0 < x < r < y$， $r \in \mathbb{Q}$，就可以得到 $-y < -r < -x < 0$ 使得 $-r \in \mathbb{Q}$。 因此，不失一般性，让$x > 0$。 将引理 1 应用于 $y - x > 0$，因此存在 $n \in \mathbb{N}$ 使得 $0 < 1/n < y - x$。 然后我们有 $ny - nx > 1$。 根据引理 3，存在 $m \in \mathbb{N}$ 使得 $nx < m < ny$。 由此得到 $x < m/n < y$，其中 $m/n \in \mathbb{Q}$。 <span style="float:right;">$_{Q.E.D.}$</span>

</br>

###### **参考资料**

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
