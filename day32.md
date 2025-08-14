---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 32

## [Bezout's identity](https://en.wikipedia.org/wiki/B%C3%A9zout%27s_identity)

Definition: For $a,b\in \mathbb{Z}$ with $\gcd (a,b)=d$ there exists $x,y\in \mathbb{Z}$ such that $ax+by=d$.

One of the most useful mathematical results that is needed to prove other important theorems is Bezout's identity. This identity has the really powerful result that $ax+by=1$ if $\gcd(a,b)=1$, which allows us to prove [Euclid's lemma](https://en.wikipedia.org/wiki/Euclid%27s_lemma) and unique prime factorization, which are widely used in mathematics.

First, we will prove the existence of this identity using (you probably guessed it) the minimal criminal method! Consider $a,b\in \mathbb{Z}$ where $a,b\neq 0$. Define the set $S$={$ax+by>0\mid x,y \in \mathbb{Z}$}. Let $x=1,y=0$ then we know that $a\in S$ which implies $S$ is nonempty. Since, all $x\in S$ have $x>0$, $S\subseteq \mathbb{N}$. Hence, we apply WOP which gives the lowest element $d=ax_0+by_0$. Using the division algorithm, $a$ can be written as $a=dq+r$ with $0\leq r <d$. Then, $r=a-dq = a-q(ax_0+by_0)$$=a(1-qx_0)-by_0q$. Note, that the remainder $r$ is in the form $ax+by$ and using the earlier definition we have that $r\in S \,\cup\, ${$0$}. However, $0\leq r<d$ which contradicts the minimality of $d$. Hence, $r$ can't be in $S$, which implies that $r=0$. Hence, $a=dq\implies d\mid a$. Similarly, $d\mid b$. Hence, $d$ is a common divisor of $a,b$.

Now we prove that $d$ is the greatest common divisor. Let, $c$ be any common divisor of $a,b$. Then, $c\mid a, c\mid b\implies a=ck,\, b=cm$ for $m,k\in \mathbb{Z}$. Since, $d=ax_0+by_0$ substituting we get $d=ckx_0+cmy_0=c(kx_0+my_0)$ which implies $c\mid d$. Since, $d>0$, $c\leq d$, $d$ is the greatest common divisor, completing the proof. From this if $\gcd(a,b)=1$, for $a,b\in \mathbb{Z}$ there exist $x,y\in \mathbb{Z}$ such that $ax+by=1$.

Note that this identity can be extended to more integers with a similar proof: for $a_1,a_2,\ldots,a_n$, there exist $x_1,x_2,\ldots,x_n$ such that $a_1x_1+a_2x_2+\ldots a_nx_n=d$ where $d=\gcd(a_1,a_2,...,a_n)$. Another important thing is that Bezout's doesn't just hold in the ring of integers. It can be extended to all [PIDs](https://en.wikipedia.org/wiki/Principal_ideal_domain) with a really similar proof to the one above. We call any integral domain in which Bezout's identity holds a Bezout domain.


<div class="day-nav-wrapper">
  <a href="./day31.html" class="day-nav__link">Previous: #31</a>
  <a href="./day33.html" class="day-nav__link">Next: #33</a>
</div>