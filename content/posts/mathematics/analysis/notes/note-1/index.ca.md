---
title: "(1) Prove the density of the rational numbers in the real numbers"
date: 2023-02-12T03:02:31+00:00
description: Prove the density of the rational numbers in the real numbers
menu:
  sidebar:
    name: (1) Prove the density of the rational numbers in the real numbers
    identifier: note-1
    parent: Analysis Notes
    weight: 10
hero: images/posts/analysis-notes.jpg
tags: ["mathematics","analysis","real analysis","notes"]
categories: ["Basic"]
---

##### **Statement**

**For any $x, y \in \Reals$ with $x < y$, there exists $r \in \mathbb{Q}$ such that $x < r < y$.**

</br>  

###### **Lemma 1**  

If $x > 0$, there exists $n_x \in \mathbb{N}$ such that $0 < 1/n_x < x$.

###### **Lemma 2**  

If $x > 0$, there exists $n_x \in \mathbb{N}$ such that $n_x - 1 \le x < n_x$.

###### **Lemma 3**  

If $x, y > 0$ with $y - x > 1$, there exists $m \in \mathbb{N}$ such that $x < m < y$.  

###### **proof of Lemma 3** 

Since $y - x > 1$, we have $x + 1 < y$. Apply Lemma 2 to x > 0, so there exists $n_x \in \mathbb{N}$ such that $n_x - 1 \le x < n_x$. So $n_x \le x + 1 < n_x + 1$. Now, we have $x < n_x \le x + 1 < y$. <span style="float:right;">$_{Q.E.D.}$</span>

</br>  

###### **proof of the statement**   

If $x = 0$, by Lemma 1,  there exists $n_y \in \mathbb{N}$ such that $0 < 1/n_y < y$.  Since $n_y \in \mathbb{N}$,  we have $1/n_y \in \mathbb{Q}$.
Notice that if $0 < x < r < y$ where $r \in \mathbb{Q}$, we can have $-y < -r < -x < 0$ such that $-r \in \mathbb{Q}$. Thus , without loss of generality, let $x > 0$. Apply Lemma 1 to  $y - x > 0$, so there exists $n \in \mathbb{N}$ such that $0 < 1/n < y - x$. Then we have $ny - nx > 1$. By Lemma 3,  there exists $m \in \mathbb{N}$ such that $nx < m < ny$. It follows that $x < m/n < y$, where $m/n \in \mathbb{Q}$. <span style="float:right;">$_{Q.E.D.}$</span>

</br>  

###### **references**  

Bartle, R. G. (2018). *Introduction to real analysis, 4th edition*. Wiley. 
