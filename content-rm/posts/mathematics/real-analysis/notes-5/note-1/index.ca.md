---
title: "5 - Basics"
date: 2023-04-18T20:33:18+00:00
description: Basics
menu:
  sidebar:
    name: 5 - Basics
    identifier: real-analysis-note-5-1
    parent: real-analysis-notes-5
    weight: 10
hero: images/posts/real-analysis-notes.jpg
tags: ["mathematics","analysis","real analysis","notes"]
categories: ["Basic"]
---

Theorem 5.1.3 (Sequential Criterion for Continuity)  
A function $f : A \rightarrow \mathbb{R}$ is continuous at $c \in A$ if and only if for every sequence $(x_n)$ in $A$ that converges to $c$, the sequence $(f(x_n))$ converges to $f(c)$.  
proof:  
Assume $f : A \rightarrow \mathbb{R}$ is continuous at $c \in A$. Suppose sequence $(x_n)$ in $A$ converges to $c$. Let $\varepsilon > 0$ be given. By definition 5.1.1, there exists $\delta > 0$ such that for any $x \in A$ with $| x - c | < \delta$, $| f(x) - f(c) | < \varepsilon$. Since sequence $(x_n)$ converges to $c$, there exists $K(\delta) \in \mathbb{N}$ such that for all $n > K(\delta)$, $| x_n - c| < \delta$. Then for all $n > K(\delta)$, $| f(x_n) - f(c) | < \varepsilon$. Therefore, the sequence $(f(x_n))$ converges to $L$.  
Conversely, we give a proof by contrapositive. If $f : A \rightarrow \mathbb{R}$ is not continuous at $c \in A$, then there exists a $\varepsilon$-neighborhood of $f(c)$ such that for all $\delta$-neighborhood of $c$, there exists a point $x_\delta \in A \cap V_\delta(c)$ but $f(x_\delta) \notin V_\varepsilon(f(c))$. So, for all $n \in \mathbb{N}$, the $(1/n)$-neighborhood of $c$, i.e., $V_{1/n}(c) = \{x \in A : 0 < |x - c| < 1/n\}$, there exists a point $x_{n} \in A \cap V_{1/n}(c), x_{n} \ne c$ but $f(x_{n}) \notin V_\varepsilon(f(c)) = \{y \in \mathbb{R} : |y - f(c)| < \varepsilon\}$. So, the sequence $(x_n)$ converges to $c$, but $f(x_n)$ does not converge to $f(c)$.<span style="float:right;">$_{Q.E.D.}$</span>

</br>

Theorem 5.2.6  
Let $A, B \subseteq \mathbb{R}$ and let $f : A \rightarrow \mathbb{R}$ and $g : B \rightarrow \mathbb{R}$ be functions such that $f(A) \subseteq B$. If $f$ is continuous at a point $c \in A$ and $g$ is continuous at $b = f(c) \in B$, then the composition $g \circ f : A \rightarrow \mathbb{R}$ is continuous at $c$.  
proof:  
Since $g$ is continuous at $b$, there exists $\delta > 0$ such that for any $x \in B$ with $| x - b | < \delta$, $| g(x) - g(b) | < \varepsilon$. Since $f$ is continuous at $c$, there exists $\gamma > 0$ such that for any $x \in A$ with $| x - c | < \gamma$, $| f(x) - f(c) | < \delta$. Since $f(A) \subseteq B$, if $x \in A$ with $| x - c | < \gamma$, then $f(x) \in B$, so $| f(x) - f(c) | = | f(x) - b | < \delta$ implies $| g(f(x)) - g(b) | < \varepsilon$.<span style="float:right;">$_{Q.E.D.}$</span>

##### **references**  

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
