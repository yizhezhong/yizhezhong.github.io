---
title: "3 - Basics"
date: 2023-02-18T04:49:46+00:00
description: Basics
menu:
  sidebar:
    name: 3 - Basics
    identifier: real-analysis-note-3-1
    parent: real-analysis-notes-3
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["mathematics","analysis","real analysis","notes"]
categories: ["Basic"]
---

##### **Definition 3.1.1**

A sequence of real numbers (a sequence in R) is a function from $\mathbb{N}$ to $\mathbb{R}$. 

##### **Definition 3.1.3**

A sequence of real numbers $X = (x_n)$ is convergent if there exists $x \in \mathbb{R}$ such that $|x_n - x| < \varepsilon$ for all $n > k_\varepsilon$, where $\varepsilon > 0$ is arbitrary and $k_\varepsilon \in \mathbb{N}$ depends on $\varepsilon$. The number $x$ is called the limit of $X$ and $X$ is said to converge to $x$. Otherwise, the sequence is divergent.

##### **Theorem 3.1.4**

The limit of a sequence $X = (x_n)$ is unique if it exists.  
proof:  
Suppose the sequence X has two limits $x$ and $x'$......

</br>

##### **Theorem 3.3.2 (Monotone Convergence Theorem)**  

A monotone sequence in $\mathbb{R}$ is convergent if and only if it is bounded. Further:  
a) If $X = (x_n)$ is a bounded increasing sequence, then  
$$
lim(x_n) = sup\{x_n : n \in \mathbb{N} \}.
$$
b) If $Y = (y_n)$ is a bounded decreasing sequence, then  
$$
lim(y_n) = inf\{y_n : n \in \mathbb{N} \}.
$$
proof:  
Theorem 3.2.2 shows that every convergent sequence is bounded. If a monotone sequence in $\mathbb{R}$ is bounded, then it is either increasing or decreasing.  
a) If $X = (x_n)$ is a bounded increasing sequence, then there exists an upper bound $M$ such that $x_n < M$ for all $n \in \mathbb{N}$. Then  by Completeness Property 2.3.6, it has a supremum $x^* = sup\{x_n : n \in \mathbb{N} \}$. The for any $\varepsilon > 0$, we have $x^* - \varepsilon < x_k$ for some $k \in \mathbb{N}$. Then for all $n \ge k$, we have $x^* - \varepsilon < x_k \le x_n \le x^* < x^* + \varepsilon$. Therefore, $X$ converges to $x^*$.  
b) If $Y = (y_n)$ is a bounded decreasing sequence, then  $X = (x_n) := -Y = (-y_n)$ is an increasing sequence. From a), we have $lim(x_n) = sup\{x_n : n \in \mathbb{N} \} = sup\{-y_n : n \in \mathbb{N} \ = -inf\{y_n : n \in \mathbb{N} \}$. Therefore, $limY = -limX = inf\{y_n : n \in \mathbb{N} \}$​.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Theorem 3.4.7 (Monotone Subsequence Theorem)**  

If $X = (x_n)$ is a sequence in $\mathbb{R}$, then $X$ has a monotone subsequence.  
proof:  
We say $x_m$ is a peak if $x_m \ge x_n$ for all $n \ge m$.  
Case 1: If X has infinitely many peaks, then we can list them by increasing subscripts $x_{m_1}, x_{m_2}, ..., x_{m_k}, ....$ Since each term is a peak, we have  
$$
x_{m_1} \ge x_{m_2} \ge \ ... \ \ge x_{m_k} \ge \ ....
$$
This sequence is a monotone decreasing subsequence of $X$.  
Case 2: If $X$ only has finitely many peaks. then we can list them by increasing subscripts $x_{m_1}, x_{m_2}, ..., x_{m_r}$. Let $s_k := m_r + k$ for $k \in \mathbb{N}$. Then $x_{s_k}$ is not a peak for all $k \in \mathbb{N}$. So, $x_{s_{k+1}} \ge x_{s_k}$ for all $k \in \mathbb{N}$. Therefore, we can obtain a monotone increasing sequence $x_{s_1}, x_{s_2}, ... , x_{s_k}, x_{s_{k+1}}, ...$ which is a subsequence of $X$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Theorem 3.4.8 (The Bolzano-Weierstrass Theorem)**  

A bounded sequence in $\mathbb{R}$ has a convergent subsequence.  
proof 1:  
Let $X = (x_n)$ be a bounded sequence in $\mathbb{R}$. By theorem 3.4.7, $X$ has a monotone subsequence. Since the subsequence is also bounded, by theorem 3.3.2, the subsequence is convergent.  
proof 2:  
Let $X = (x_n)$ be a bounded sequence in $\mathbb{R}$. Then the set $\{x_n : n \in \mathbb{N}\}$ is contained in $I := [a, b]$. Take $n_1 := 1$, and bisect $I_1$ into $I'_1$ and $I''_1$. Then divide $\{n \in \mathbb{N} : n > n_1\}$ into  
$$
A_1 := \{n \in \mathbb{N} : n > n_1, n \in I'_1\}, \ B_1 := \{n \in \mathbb{N} : n > n_1, n \in I''_1\}
$$
Then at least one of $A_1, B_1$ is infinite. Say $A_1$ is infinite, then we can bisect $I_2$ into $I'_2$ and $I''_2$ by taking $n_2 := infA_1$ and divide $A_1$ into $A_2, B_2$. Continuing this way, we can obtain a sequence of nested interval $I_1 \supseteq I_2 \supseteq ... \supseteq I_k \supseteq ...$ and a subsequence $(x_{n_k})$ of $X$ such that $x_{n_k} \in I_k$ for $k \in \mathbb{N}$. Notice that the length of $I_k$, also written as $b_k - a_k$, is $(b-a)/2^{k-1}$. So, $inf\{b_n - a_n : n \in \mathbb{N}\} = 0$. By theorem 2.5.3, there exists a unique common point $\xi \in I_k$ for all $k \in \mathbb{N}$. Then since $x_{n_k}$ and $\xi$ are both in $I_k$, we have $|x_{n_k} - \xi| \le (b-a)/2^{k-1}$. Therefore the subsequence $(x_{n_k})$ converges to $\xi$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Definition 3.5.1**  

Cauchy sequence is a sequence of real number $(x_n)$ such that for any $\varepsilon > 0$, there exists $N(\varepsilon) \in \mathbb{N}$ such that for any natural numbers $n, m \ge H(\varepsilon)$, $|x_n - x_m| < \varepsilon$.

</br>

##### **Theorem 3.5.5 (Cauchy Convergence Criterion)**  

A sequence in $\mathbb{R}$ is convergent if and only if it is a Cauchy sequence.  
proof:  
By Lemma 3.5.3, if a sequence in $\mathbb{R}$ is convergent, then it is a Cauchy sequence. Conversely, if $X := (x_n)$ is a Cauchy sequence, then by Lemma 3.5.4, it is bounded. By theorem 3.4.8, there exists a subsequence $X' = (x_{n_k})$ converges to some $x^* \in \mathbb{R}$. Since $X$ is a Cauchy sequence, given $\varepsilon > 0$, there exists $H(\varepsilon/2)$ such that for $n, m \ge H(\varepsilon/2)$, $|x_n - x_m| < \varepsilon/2$. Since $X'$ converges to $x^*$, there exists a natural number $n_K \ge H(\varepsilon/2)$ such that $|x_{n_K} - x^*| < \varepsilon/2$. So, $|x_n - x_{n_K}| < \varepsilon/2$ for $n \ge H(\varepsilon/2)$. Therefore, $|x_n - x^*| = |x_n - x_{n_K} + x_{n_K} - x^*| \le |x_n - x_{n_K}| + |x_{n_K} - x^*| < \varepsilon/2 + \varepsilon/2 = \varepsilon$. Therefore, the sequence $X$ is convergent.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

</br>

##### **references**  

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
