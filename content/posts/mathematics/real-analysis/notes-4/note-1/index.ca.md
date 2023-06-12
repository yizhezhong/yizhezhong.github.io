---
title: "4 - Basics"
date: 2023-03-21T20:53:49+00:00
description: Basics
menu:
  sidebar:
    name: 4 - Basics
    identifier: real-analysis-note-4-1
    parent: real-analysis-notes-4
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["mathematics","analysis","real analysis","notes"]
categories: ["Basic"]
---

##### **Definition 4.1.1**

Let $A \subseteq \mathbb{R}$. A point $c \in \mathbb{R}$ is a cluster point of A if for every $\delta > 0$, there exists $x \in A, x \ne c$ such that $|x - c| < \delta$.  
rephrase: A point $c \in \mathbb{R}$ is a cluster point of A if there exists $x \in A, x \ne c$ in every $\delta-$neighborhood $V_\delta (c) = (c-\delta, c+\delta)$.

</br>

##### **Theorem 4.1.2**  

Let $A \subseteq \mathbb{R}$. A point $c \in \mathbb{R}$ is a cluster point of $A$ if and only if there exists a sequence $(a_n)$ in $A$ such that lim$(a_n) = c$ and $a_n \ne c$ for all $n \in \mathbb{N}$.  
proof:  
If $c \in \mathbb{R}$ is a cluster point of $A$, then for every $n \in \mathbb{N}$, there exists $a_n \in A, a_n \ne c$ such that $|a_n - c| < 1/n$. By theorem 3.1.10, since lim$(1/n) = 0$, we have lim$(a_n) = c$.  
Conversely, if there exists a sequence $(a_n)$ in $A$ such that lim$(a_n) = c$ and $a_n \ne c$ for all $n \in \mathbb{N}$, then for every $\delta > 0$, there exists $N(\delta) \in \mathbb{N}$ such that $|a_n - c| < \delta$ for all $n > N(\delta)$. Since $a_n \in A$ and $a_n \ne c$, the point c is a cluster point of $A$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Definition 4.1.4**  

Let $A \subseteq \mathbb{R}$, and let $c \in \mathbb{R}$ be a cluster point of $A$. For a function $f: A \rightarrow \mathbb{R}$, a real number $L$ is said to be the limit of $f$ at $c$ if for any $\varepsilon > 0$ , there exists $\delta > 0$  such that for any  $x \in A$ with $0 < | x - c| < \delta$, $|f(x) - L| < \varepsilon$.  
If $L$ is the limit of $f$ at $c$, then we also say that $f$ converges to $L$ at $c$. We often write  
$$
L = \lim_{x \to c}f(x) \ or \ L = \lim_{x \to c}f.
$$
We can also say "$f(x)$ approaches $L$ as $x$ approaches $c$." Written as  
$$
f(x) \rightarrow L \ as \ x \rightarrow c.
$$
If the limit of $f$ does not exist at $c$, we say that $f$ diverges at $c$.

</br>

##### **Theorem 4.1.5**  

If $f: A \rightarrow \mathbb{R}$ is and if $c$ is a cluster point of $A$, then $x$ can have only one limit at $c$.  
proof:  
Suppose $L$ and $L'$ are both limits of $f$ at $c$.  Then for any $\varepsilon > 0$, there exists $\delta(\varepsilon/2) > 0$  such that for any  $x \in A$ with $0 < | x - c| < \delta(\varepsilon/2)$, $|f(x) - L| < \varepsilon/2$.  Also, there exists $\delta'(\varepsilon/2) > 0$  such that for any  $x \in A$ with $0 < | x - c| < \delta'(\varepsilon/2)$, $|f(x) - L'| < \varepsilon/2$.  Let $\delta := inf\{\delta(\varepsilon/2), \delta'(\varepsilon/2)\}$, then for any  $x \in A$ with $0 < | x - c| < \delta$,
$$
|L - L'| \le |L - f(x)| + |f(x) + L'| < \varepsilon/2 + \varepsilon/2 = \varepsilon.
$$
Since $\varepsilon > 0$ is arbitrary, we have $L - L' = 0$. Therefore, $L = L'$. <span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Theorem 4.1.6**  

Let $f: A \rightarrow \mathbb{R}$ and let $c$ be a cluster point of $A$. Then the following statements are equivalent:  
i) $\lim_{x \to c}f(x) = L$.  
ii) Given any $\varepsilon$-neighborhood of $L$, there exists $\delta$-neighborhood of $c$ such that for any $\ x \in V_\delta(c) \cap A$ where $x \ne c$, $f(x) \in V_\varepsilon(L)$.  
proof:  
By definition, $\lim_{x \to c}f(x) = L$ is equivalent as saying that for any $\varepsilon > 0$ , there exists $\delta > 0$  such that for any  $x \in A$ with $0 < | x - c| < \delta$, $|f(x) - L| < \varepsilon$. We can establish the equivalent statement that for any $\varepsilon > 0$, there exists $\delta > 0$ such that for any  $x \in A$ with $x \in V_\delta(c) \backslash \{c\}$, $f(x) \in V_\epsilon(L)$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Theorem 4.1.8 (Sequential Criterion)**  

Let $f: A \rightarrow \mathbb{R}$ and let $c$ be a cluster point of $A$. Then the following statements are equivalent:  
i) $\lim_{x \to c}f(x) = L$.  
ii) Given any sequence $(x_n)$ that converges to $c$, where $x_n \ne c$ for all $n \in \mathbb{N}$, the sequence $(f(x_n))$ converges to $L$.  
proof:  
Assume $\lim_{x \to c}f(x) = L$. Suppose sequence $(x_n)$ in $A$ converges to $c$, where $x_n \ne c$ for all $n \in \mathbb{N}$. Let $\varepsilon > 0$ be given. By definition 4.1.4, there exists $\delta > 0$ such that for any $x \in A$ with $0 < | x - c | < \delta$, $| f(x) - L | < \varepsilon$. Since sequence $(x_n)$ converges to $c$, there exists $K(\delta) \in \mathbb{N}$ such that for all $n > K(\delta)$, $| x_n - c| < \delta$. Then for all $n > K(\delta)$, $| f(x_n) - L | < \varepsilon$. Therefore, the sequence $(f(x_n))$ converges to $L$.  
Conversely, we give a proof by contrapositive. If i) is not true, then there exists a $\varepsilon$-neighborhood of $L$ such that for all $\delta$-neighborhood of $c$, there exists a point $x_\delta \in A \cap V_\delta(c), x_\delta \ne c$ but $f(x_\delta) \notin V_\varepsilon(L)$. So, for all $n \in \mathbb{N}$, the $(1/n)$-neighborhood of $c$, i.e., $V_{1/n}(c) = \{x \in A : 0 < |x - c| < 1/n\}$, there exists a point $x_{n} \in A \cap V_{1/n}(c), x_{n} \ne c$ but $f(x_{n}) \notin V_\varepsilon(L) = \{y \in \mathbb{R} : |y - L| < \varepsilon\}$. So, the sequence $(x_n)$ converges to $c$, but $f(x_n)$ does not converge to $L$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **4.1.9 Divergence Criteria**  

Let $A \subseteq \mathbb{R}$, let $f: A \rightarrow \mathbb{R}$ and let $c \in \mathbb{R}$ be a cluster point of $A$.  
a) If $L \in \mathbb{R}$, then f does not have limit $L$ at $c$ if and only if there exist a sequence $(x_n)$ in $A$ such that $x_n \ne c$ for all $n \in \mathbb{N}$ and $(x_n)$ converges to $c$ but $(f(x_n))$ does not converge to $L$.  
b) The function $f$ does not have a limit at $c$ if and only if there exist a sequence $(x_n)$ in $A$ such that $x_n \ne c$ for all $n \in \mathbb{N}$ and $(x_n)$ converges to $c$ but $(f(x_n))$ does not converge in $\mathbb{R}$.  
proof:  
(placeholder)

</br>

##### **Definition 4.2.1**  

Let $A \subseteq \mathbb{R}$, let $f: A \rightarrow \mathbb{R}$ and let $c \in \mathbb{R}$ be a cluster point of $A$.  We say that $f$ is bounded on a neighborhood of $c$ if there exists $V_\delta(c)$ and a constant $M > 0$ such that for all $x \in A \cap V_\delta(c)$, $| f(x) | \le M$.

</br>

##### **Theorem 4.2.2**  

Let $A \subseteq \mathbb{R}$, let $f: A \rightarrow \mathbb{R}$. If $f$ has a limit at $c$ then $f$ is bounded on some neighborhood of $c$.  
proof:  
Let $L := \lim_{x \to c}f$. Then for an $\varepsilon > 0$, there exists $\delta > 0$ such that for any  $x \in A$ with $0 < | x - c| < \delta$, we have$|f(x) - L| < \varepsilon$. Then by Corollary 2.2.4 (a) and Theorem 2,2,2 (d), $|f(x) | - | L | \le ||f(x)| - |L|| \le |f(x) - L| < \varepsilon$. So $f$ is bounded by $M = |L| + \varepsilon$ if $c \notin A$. If $c \in A$, we can take $M = sup\{|f(c), |L| + \varepsilon\}$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Definition 4.2.3**  

Let $A \subseteq \mathbb{R}$ and let $f$ and $g$ be functions defined on $A$ to $\mathbb{R}$. Then for all $x \in A$, we define the sum $f + g$, the difference $f - g$, and the product $fg$ as
$$
(f + g)(x) := f(x) + g(x), \\
(f - g)(x) := f(x) - g(x), \\
(fg)(x) := f(x)g(x).
$$
If $b \in \mathbb{R}$, then for all $x \in A$, we define the multiple $bf$ as  
$$
(bf)(x) := bf(x).
$$
If $h(x) \ne 0$ for all $x \in A$. Then for all $x \in A$, we define the quotient $f/h$ as  
$$
(\frac{f}{h})(x) := \frac{f(x)}{h(x)}.
$$
</br>

##### **Theorem 4.2.4**  

Let $A \subseteq \mathbb{R}$ and let $f$ and $g$ be functions on $A$ to $\mathbb{R}$, and let $c \in \mathbb{R}$ be a cluster point of $A$. Let $b \in \mathbb{R}$.  
a) If $\lim_{x \to c}f(x) = L$ and $\lim_{x \to c}g(x) = M$, then  
$$
\lim_{x \to c}(f + g)(x) = L + M, \\
\lim_{x \to c}(f - g)(x) = L - M, \\
\lim_{x \to c}(fg)(x) = LM, \\
\lim_{x \to c}(bf)(x) = bL.
$$
b) If $h: A \rightarrow \mathbb{R}$, if $h(x) \ne 0$ for all $x \in A$, and if $\lim_{x \to c}h(x) = H \ne 0$, then  
$$
\lim_{x \to c}(\frac{f}{h})(x) = \frac{L}{H}.
$$
proof:  
(placeholder)

</br>

##### **Theorem 4.2.6**  

Let $A \subseteq \mathbb{R}$, let $f: A \rightarrow \mathbb{R}$ and let $c \in \mathbb{R}$ be a cluster point of $A$. If $a \le f(x) \le b$ for all $x \in A, x \ne c$, and if $\lim_{x \to c}f(x)$ exists, then $a \le \lim_{x \to c}f(x) \le b$.  
proof:  
(placeholder)

</br>

##### **Theorem 4.2.7 (Squeeze Theorem)**  

Let $A \subseteq \mathbb{R}$ and let $f, g, h$ be functions on $A$ to $\mathbb{R}$, and let $c \in \mathbb{R}$ be a cluster point of $A$. If $f(x) \le g(x) \le h(x)$ for all $x \in A, x\ne c$, and if $\lim_{x \to c}f(x) = L = \lim_{x \to c}h(x)$, then $\lim_{x \to c}g(x) = L$.  
proof:  
(placeholder)

</br>

##### **Theorem 4.2.9**  

Let $A \subseteq \mathbb{R}$, let $f: A \rightarrow \mathbb{R}$ and let $c \in \mathbb{R}$ be a cluster point of $A$. If $\lim_{x \to c}f(x) > 0$ [respectively, $\lim_{x \to c}f(x) < 0$], then there exists a neighborhood $V_\delta (c)$ of $c$ such that $f(x) > 0$ [respectively, $f(x) < 0$] for all $x \in A \cap V_\delta(c), x \ne c$.  
proof:  
(placeholder)

</br>

##### **Theorem 4.3.2**  

Let $A \subseteq \mathbb{R}$, let $f : A \rightarrow \mathbb{R}$, and let $c \in \mathbb{R}$ be a cluster point of $A \cap (c, \infty)$. Then the following statements are equivalent:  
i) $\lim_{x \to c+}f = L$.  
ii) For all sequence $(x_n)$ converges to $c$ such that $x_n \in A \cap (c, \infty)$, $n \in \mathbb{N}$, the sequence $(f(x_n))$ converges to $L$.  
proof:  
Assume $\lim_{x \to c+}f(x) = L$. Suppose sequence $(x_n)$ in $A \cap (c, \infty)$ converges to $c$. Let $\varepsilon > 0$ be given. By definition 4.3.1, there exists $\delta > 0$ such that for any $x \in A$ with $0 < x - c < \delta$, $| f(x) - L | < \varepsilon$. Since sequence $(x_n)$ converges to $c$, there exists $K(\delta) \in \mathbb{N}$ such that for all $n > K(\delta)$, $x_n - c = |x_n - c| < \delta$. Then for all $n > K(\delta)$, $| f(x_n) - L | < \varepsilon$. Therefore, the sequence $(f(x_n))$ converges to $L$.  
Conversely, we give a proof by contrapositive. If i) is not true, then there exists a $\varepsilon$-neighborhood of $L$ such that for all $\delta$-neighborhood of $c$, there exists a point $x_\delta \in A \cap V_\delta(c), x_\delta > c$ but $f(x_\delta) \notin V_\varepsilon(L)$. So, for all $n \in \mathbb{N}$, the $(1/n)$-neighborhood of $c$, i.e., $V_{1/n}(c) = \{x \in A : 0 < |x - c| < 1/n\}$, there exists a point $x_{n} \in A \cap V_{1/n}(c), x_{n} > c$ but $f(x_{n}) \notin V_\varepsilon(L) = \{y \in \mathbb{R} : |y - L| < \varepsilon\}$. So, the sequence $(x_n)$ converges to $c$, but $f(x_n)$ does not converge to $L$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **references**  

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
