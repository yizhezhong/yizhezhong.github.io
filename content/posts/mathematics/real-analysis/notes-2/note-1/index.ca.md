---
title: "2 - Basics"
date: 2023-02-12T03:02:31+00:00
description: Basics
menu:
  sidebar:
    name: 2 - Basics
    identifier: real-analysis-note-2-1
    parent: real-analysis-notes-2
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["mathematics","analysis","real analysis","notes"]
categories: ["Basic"]
---

##### **Theorem 2.1.2**  

a) If $z + a = a$ for some $z, a \in \mathbb{R}$, then $z = 0$.  
b) If $u \cdot b = b$ for some $u, b \in \mathbb{R}, b \ne 0$, then $u = 1$.  
c) If $a \in \mathbb{R}$, then $a \cdot 0 = 0$.  
proof:  
(placeholder)

</br>

##### **Theorem 2.1.3**  

a) If $a \cdot b = 1$ for some $a, b \in \mathbb{R}, a \ne 0$, then $b = 1/a$.  
b) If $a \cdot b = 0$ for some $a, b \in \mathbb{R}$, then at least one of $a$ and $b$ is 0.  
proof:  
(placeholder)

</br>

##### **Definition**  

A rational number is an element of $\mathbb{R}$ that can be written in the form $b/a \in \mathbb{R}$, where $a, b \in \mathbb{Z}$ and $a \ne 0$. The notation $\mathbb{Q}$ denotes the set of all rational numbers in $\mathbb{R}$.

</br>

##### **Theorem 2.1.4**  

A number r satisfies $r^2 = 2$ cannot be rational.  
proof:  
(placeholder)

</br>

##### **2.1.5 The Order Properties of $\mathbb{R}$**  

There exists $\mathbb{P} \subseteq \mathbb{R}, \mathbb{P} \ne \emptyset$,  satisfying:  
i) Closure under addition  
ii) Closure under multiplication  
iii) Trichotomy Property: If $a \in \mathbb{R}$, then exactly one of the following holds:
$$
a\in \mathbb{P}, \ \ \ \ a = 0, \ \ \ \ -a \in \mathbb{P}
$$
</br>

##### **Definition 2.1.6**  

Let $a, b \in \mathbb{R}$.  
a) If $a - b \in \mathbb{P}$, then we write $a > b$ or $b < a$.  
b) If $a - b \in \mathbb{P} \cup \{0\}$, then we write $a \geq b$ or $b \leq a$. 

</br>

##### **Theorem 2.1.7**  

Let $a, b , c \in \mathbb{R}$.  
a) If $a > b$ and $b > c$, then $a > c$.  
b) If $a > b$, then $a + c > b + c$.  
c) If $a > b$ and $c > 0$, then $ca > cb$.  
	If $a < b$ and $c < 0$, then $ca < cb$.  
proof:  
(placeholder)

</br>

##### **Theorem 2.1.8**  

a) If $a \in \mathbb{R}$ and $a \ne 0$, then $a^2 > 0$.  
b) $1 > 0$.  
c) If $n \in \mathbb{N}$, then $n > 0$.  
proof:  
(placeholder)

</br>

##### **Theorem 2.1.9**  

If $a \in \mathbb{R}$ satisfies $0 \le a < \varepsilon$ for every $\varepsilon > 0$, then $a = 0$.  
proof:  
(placeholder)

</br>

##### **Theorem 2.1.10**  

If $ab > 0$, then either  
i) $a > 0$ and $b > 0$, or  
ii) $a < 0$ and $b < 0$.   
proof:  
(placeholder)

</br>

##### **Corollary 2.1.11**  

If $a, b < 0$, then either  
i) $a < 0$ and $b > 0$, or  
ii) $a > 0$ and $b < 0$. 

</br>

##### **Definition**  

The absolute value $|a|$ for $a \in \mathbb{R}$​ is defined by  
$$
|a| := 
\begin{cases}
a \ \ \ \ \ if \ \ a \ge 0 \\
-a \ \ if \ \ a < 0
\end{cases}
$$
</br>

##### **Theorem 2.2.2**  

Let $a, b, c \in \mathbb{R}$, $c \ge 0$ Then  
a) $|ab| = |a||b|$,  
b) $|a|^2 = a^2$,  
c) $|a| \le c$ if and only if $-c \le a \le c$,  
d) $-|a| \le a \le |a|$.  
proof:  
(placeholder)

</br>

##### **Theorem 2.2.3 (Triangular Inequality)**  

If $a, b \in \mathbb{R}$, then $|a + b| \le |a| + |b|$.  
proof:  
(placeholder)

</br>

##### **Corollary 2.2.4**  

If $a, b \in \mathbb{R}$, then  
a) $||a| - |b|| \le |a - b|$,  
b) $|a - b| \le |a| + |b|$.

</br>

##### **Corollary 2.2.5**  

Let $a_1, a_2, ..., a_n \in \mathbb{R}$​. Then  
$$
| \sum_{k = 1}^n a_k | \le \sum_{k = 1}^n |a_k|.
$$
</br>

##### **Definition 2.2.7**  

Let $a \in \mathbb{R}$ and $\varepsilon > 0$. Then the set $V_\varepsilon (a) := \{x \in \mathbb{R} : |x - a| < \varepsilon \}$ is called the $\varepsilon$-neighborhood of $a$.

</br>

##### **Theorem 2.2.8**  

Let $a \in \mathbb{R}$. If $x \in V_\varepsilon (a)$ for every $\varepsilon > 0$, then $x = a$.  
proof:  
(placeholder)

</br>

##### **Definition 2.3.1 & 2.3.2**  

Let $S \subseteq \mathbb{R}, S \ne \emptyset$.  
a) An upper bound of $S$ is a number $u$ such that $u \ge s$ for all $s \in S$.  If $S$ has at least one upper bound, then it is said to be bounded above.   
b) An lower bound of $S$ is a number $w$ such that $w \le s$ for all $s \in S$.  If $S$ has at least one lower bound, then it is said to be bounded below.  
c) If $S$ is both bounded above and bounded below, then it is said to be bounded. Otherwise, it is said to be unbounded.  
d) If $S$ is bounded above, then an upper bound $u$ of $S$ is said to be a supremum (least upper bound) of $S$ if $u \le v$ for every upper bound $v$ of $S$. We denote a supremum of S by $sup \ S$.  
e) If $S$ is bounded below, then an lower bound $w$ of $S$ is said to be a infimum (greatest lower bound) of $S$ if $w \ge t$ for every lower bound $t$ of $S$. We denote a infimum of S by $inf \ S$.

</br>

##### **Lemma 2.3.3**  

Let $S \subseteq \mathbb{R}, S \ne \emptyset$.  Then $u$ is $sup \ S$ if and only if  
i) $u \ge s$ for all $s \in S$,  
ii) if $v < u$, then there exists $s' \in S$ such that $v < s'$.

</br>

##### **Lemma 2.3.4**  

Let $S \subseteq \mathbb{R}, S \ne \emptyset$.  Then $u$ is $supS$ if and only if for every $\varepsilon > 0$ there exists $s_\varepsilon \in S$ such that $s_\varepsilon > u - \varepsilon$.

</br>

##### **2.3.6 The completeness Property of $\mathbb{R}$**  

Every nonempty set $S \subseteq \mathbb{R}$ bounded above has a supremum in $\mathbb{R}$.

</br>

##### **2.4.3 Archimedean Property**  

If $x \in \mathbb{R}$, then there exists $n_x \in \mathbb{N}$ such that $x \le n_x$.

</br>

##### **Corollary 2.4.4**  

If $S := \{ 1/n : n \in \mathbb{N} \}$, then $inf \ S = 0$.  

</br>

##### **Corollary 2.4.5**  

If $x > 0$, there exists $n_x \in \mathbb{N}$ such that $0 < 1/n_x < x$.

</br>

##### **Corollary 2.4.6**  

If $x > 0$, there exists $n_x \in \mathbb{N}$ such that $n_x - 1 \le x < n_x$.

</br>

##### **Theorem 2.4.7**  

There exists $x \in \mathbb{P}$ such that $x^2 = 2$.  
proof:  
(placeholder)

</br>

###### **Corollary**  

If $x, y > 0$ with $y - x > 1$, there exists $m \in \mathbb{N}$ such that $x < m < y$.  
Proof: Since $y - x > 1$, we have $x + 1 < y$. Apply Corollary 2.6 to x > 0, so there exists $n_x \in \mathbb{N}$ such that $n_x - 1 \le x < n_x$. So $n_x \le x + 1 < n_x + 1$. Now, we have $x < n_x \le x + 1 < y$. <span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Theorem 2.4.8 (The Density Theorem)**  

For any $x, y \in \Reals$ with $x < y$, there exists $r \in \mathbb{Q}$ such that $x < r < y$.  
Proof: If $x = 0$, by Corollary 2.5, there exists $n_y \in \mathbb{N}$ such that $0 < 1/n_y < y$.  Since $n_y \in \mathbb{N}$,  we have $1/n_y \in \mathbb{Q}$.
Notice that if $0 < x < r < y$ where $r \in \mathbb{Q}$, we can have $-y < -r < -x < 0$ such that $-r \in \mathbb{Q}$. Thus , without loss of generality, let $x > 0$. Apply Corollary 2.5 to  $y - x > 0$, so there exists $n \in \mathbb{N}$ such that $0 < 1/n < y - x$. Then we have $ny - nx > 1$. By Theorem 2.11,  there exists $m \in \mathbb{N}$ such that $nx < m < ny$. It follows that $x < m/n < y$, where $m/n \in \mathbb{Q}$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

##### **Corollary 2.4.9**  

For any $x, y \in \Reals$ with $x < y$, there exists $z \in \mathbb{R} \backslash \mathbb{Q}$ such that $x < z < y$.  

</br>

##### **Definition**  

Let $a, b \in \mathbb{R}$ with $a < b$.  
The open interval $(a, b)$ is defined as  
$$
(a, b) := \{x \in \mathbb{R} : a < x < b\},
$$
where the points a and b are called the endpoints of the interval $(a, b)$.   
The closed interval $[a, b]$ with the endpoints $a$ and $b$ is defined as  
$$
[a, b] := \{x \in \mathbb{R} : a \le x \le b\}.
$$
The half open intervals with the endpoints $a$ and $b$ are defined as  
$$
[a, b) := \{x \in \mathbb{R} : a \le x < b\},
$$
and
$$
(a, b] := \{x \in \mathbb{R} : a < x \le b\}.
$$
The above intervals are all bounded and has length defined by $b - a$. If $a = b$, the open interval $(a, a) = \emptyset$, and the closed interval $[a, a] = {a}$.   
The infinite open intervals $(a, \infty)$ and  $(-\infty, b)$ are defined as  
$$
(a, \infty) := \{x \in \mathbb{R} : x > a\},
$$
and
$$
(-\infty, b) := \{x \in \mathbb{R} : x < b\}.
$$
The infinite closed intervals $[a, \infty)$ and  $(-\infty, b]$ are defined as  
$$
[a, \infty) := \{x \in \mathbb{R} : x \ge a\},
$$
and
$$
(-\infty, b] := \{x \in \mathbb{R} : x \le b\}.
$$
The infinite interval with no endpoints is defined as  
$$
(-\infty, \infty) := \mathbb{R}
$$
Notice that neither $-\infty$ nor $\infty$ are elements of $\mathbb{R}$, but only convenient symbols.

</br>

##### **Characterization of Intervals**  

If $x, y \in I$ with $x < y$ and $I$ an interval, then for any $t \in \mathbb{R}$ such that $t \in [x, y]$, we have $t \in I$.

</br>

##### **Theorem 2.5.1 (Characterization Theorem)**  

If $S \subseteq \mathbb{R}$ contains at least two points had satisfy  
$$
if \ x, y \in S \ and \ x < y, \ then \ [x, y] \subseteq S,
$$
then $S$ is an interval.  
proof:  
(placeholder)

</br>

##### **Definition**  

A sequence of intervals $I_n, n \in \mathbb{N}$, is called nested if  
$$
I_1 \supseteq I_2 \supseteq \ ... \ \supseteq I_n \supseteq I_{n+1} \supseteq \ ...,
$$
that is, $I_n \supseteq I_{n+1}$ for all $n \in \mathbb{N}$.

</br>

##### **Example**  

Define $I_n := [0, 1/n]$ for $n \in \mathbb{N}$. Since $I_n \supseteq I_{n+1}$ for all $n \in \mathbb{N}$, $I_n$ is nested. Notice that 0 is contained in all intervals. In fact, 0 is the only such common point.  
Proof:  
For any $x > 0$, by Corollary 2.4.5, there exists $n_x \in \mathbb{N}$ such that $0 < 1/n_x < x$. Recall that $I_{n_x} := [0, 1/n_x] = \{x \in \mathbb{R} : 0 \le x \le 1/n_x\}$. So, $x \notin I_{n_x}$.<span style="float:right;">$_{Q.E.D.}$</span>  
We write $\cap^{\infty}_{n = 1} I_n = \{0\}$.  
Notice that If $J_{n_x} := (0, 1/n_x)$ for $n \in \mathbb{N}$, then  $\cap^{\infty}_{n = 1} J_n = \emptyset$.

</br>

##### **2.5.2 Nested Interval Property**  

If $I_n := [a_n, b_n]$ is a nested sequence of closed bounded intervals, then there exists $\xi \in \mathbb{R}$ such that $\xi \in I_n$ for all $n \in \mathbb{N}$.  
Proof:  
(placeholder)

</br>

##### **Theorem 2.5.3**  

If $I_n := [a_n, b_n]$ is a nested sequence of closed bounded intervals such that  
$$
inf\{b_n - a_n : n \in \mathbb{N}\} = 0,
$$
then $\xi \in I_n$ for all $n \in \mathbb{N}$ is unique.  
Proof:  
(placeholder)

</br>

##### **Theorem 2.5.4**  

The set $\mathbb{R}$ is not countable.  
Proof:  
(placeholder)

</br>

##### **Theorem 2.5.5**  

The unit interval [0, 1] is not countable.  
Proof:  
(placeholder)

</br>

</br>

##### **references**  

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
