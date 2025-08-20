---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 38

## [Lagrange's Theorem](https://en.wikipedia.org/wiki/Lagrange%27s_theorem_(number_theory))

Definition: For all polynomials $f$ in $\mathbb{Z}_p[x]$ (ring of polynomials with coefficients in $\mathbb{Z}_p$) with prime $p$, either every coefficient of $f$ is null or $f(x)=0$ has at most $\deg{f}$ solutions in $\mathbb{Z}_p$.

We have been using the general case of this theorem in $\mathbb{Z}$ from middle school by saying that a polynomial with degree $n$ can't have more than $n$ roots. But why? Before, we prove the theorem let us define the division algorithm in $\mathbb{Z}_p[x]$. If $a(x),b(x) \in \mathbb{Z}_p[x]$ such that $b(x)$ isn't a constant, then there exist quotient $q(x)$ and remainder $r(x)$, such that $a(x)=b(x)q(x)+r(x)$ such that $0 \leq\deg r(x)<\deg b(x)$. The proof follows from $\mathbb{Z}$ but instead we use WOP on the degrees.

Now we prove the theorem. Let $f\in \mathbb{Z}[x]$ be an integer polynomial. Using basic modular arithmetic rules, if $f(x)\equiv 0 \pmod{p}$ then $g(x)=f(x\pmod{p})\equiv 0\pmod{p}$ where $g(x)\in\mathbb{Z}_p[x]$. Hence, both versions in $\mathbb{Z}[x]$ and $\mathbb{Z}_p[x]$ are equivalent.

WLOG let $f\in \mathbb{Z}_p[x]$. We prove it with induction on $n=\deg{f}$. If $\deg{f}=0$ then $f$ has no roots because its a constant and the statement holds true. If $\deg{f}\geq 1$ and there are no roots the statement holds again. Assume that any polynomial $h\in\mathbb{Z}_p[x]$ with $\deg h\leq n-1$ has at most $\deg h$ roots in $\mathbb{Z}_p$. Now we consider the case where $\deg{f}\geq 1$ and $f$ has a root $a$ in $\mathbb{Z}_p[x]$. Since the ring's a field we apply the division algorithm to $f$ and the polynomial $x-a$ getting $f(x)=g(x)(x-a)+r$ for some polynomial $g(x)$ and constant $r$ since $\deg{r}<1$. THen, $f(a)=0\implies r=0$. Hence, roots of $f$ are roots of $g$. By the induction hypothesis there are at most $\deg{g}\leq\deg{f}-1$ roots. Hence, $f$ has atmost $\deg{g}+1=(n-1)+1=\deg{f}$ roots, completing the proof.

This proof can be generalized to any integral domain $R$ such that if $f(x)$ is a polynomial with degree $n>0$, the polynomial equation $f(a)=0$ has at most $n=\deg{f(x)}$ roots in $R$. Try proving Wilson's theorem using this theorem now!




<div class="day-nav-wrapper">
  <a href="./day37.html" class="day-nav__link">Previous: #37</a>
  <a href="./day39.html" class="day-nav__link">Next: #39</a>
</div>


