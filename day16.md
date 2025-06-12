---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 16

## [The Residue Theorem](https://en.wikipedia.org/wiki/Residue_theorem)

Definition: Suppose that $\Gamma$ is a closed contour oriented positively, and that $f$ is holomorphic on and inside $\Gamma$, except at a finite number of singular points $z_1, \dots, z_n$. Then $\int_{\Gamma} f(z)\,dz = 2\pi i \sum_{k=1}^{n} \operatorname{Res}(f; z_k)$.

Today we explore how series can be used in complex analysis! Before we prove the Residue theorem, which is a simple restatement of the Cauchy Integral Formula, let's remember that for some integer $n$ the integral $\int_{\lvert z-z_0 \rvert =r} (z-z_0)^n dz $ is 0 when $n \neq -1$ and is $2\pi i$ when $n =-1$. This result is quite easy to get using Contour integration, and is the exact problem we discussed back then. While, we won't go into it right now, know that we can freely differentiate and integrate power and Laurent series term by term. Now, lets prove the theorem! We know that we can represent $f$ in a deleted neighborhood of $z_0$ by using the laurent series $\sum_{n=-\infty}^{\infty}a_n(z-z_0)^n$. Then if $r$ is small enough for the [Laurent series](https://en.wikipedia.org/wiki/Laurent_series) to converge for $0<\lvert z-z_0 \rvert \leq r$, then we have $\int_{\lvert z-z_0 \rvert =r} f(z)dz=\sum_{n=-\infty}^{\infty}a_n \int_{\lvert z-z_0 \rvert =r} (z-z_0)^n dz = 2\pi i a_{-1}$ since all the other terms in the sum integrate to 0. Thus, the $a_{-1}$, coefficient must be special and it is! We call it the residue of $f$ at $z_0$ and write $a_{-1}=\operatorname{Res}(f; z_0)$. Now, if $\Gamma$ is a small circle around $z_0$, then it is obvious that $\int_{\Gamma} f(z)\,dz = 2\pi i \sum_{k=1}^{n} \operatorname{Res}(f; z_0)$. If $\Gamma$ is larger with several singularities, then we add all the contributions from each residue. $\blacksquare$

Now, let's go over some examples. Before, that it is important to note that if $f$ has a simple pole at $z_0$, then $ \operatorname{Res}(f; z_0)=\lim_{z \to z_0} (z-z_0)f(z)$. Thus, for instance if $f(z)=\frac{1}{z^2+1}$, we can easily compute $ \operatorname{Res}(f; i)$. Here, $\operatorname{Res}(f; i)=\lim_{z \to i} \frac{z-i}{z^2+1} = \lim_{z \to i}\frac{1}{z+i}=\frac{1}{2i}$. Now, lets compute $ \operatorname{Res}(f; i)$ for $f(z)=(z^2+i)^{-3}$.  We have, $\frac{1}{(z^2+i)^{3}}=\frac{1/(z+i)^3}{(z-i)^3}=\frac{1 / ((z - i) + 2i)^3}{(z - i)^3}=\frac{1}{(2i)^3}(1 + \frac{z - i}{2i})^{-3} \frac{1}{(z - i)^3}$ =$$\frac{i}{8} (1 - 3\frac{z - i}{2i} + 6(\frac{z - i}{2i})^2 - \cdots) \frac{1}{(z - i)^3}$$ = $$\cdots + \frac{i}{8} \times 6 \times \frac{1}{-4} \times \frac{1}{z - i} + \cdots = \cdots + \frac{-3i}{16} \cdot \frac{1}{z - i} + \cdots$$. Hence, the residue is $\frac{-3i}{16}$! This theorem can also be used on the integral $$\int_{-\infty}^{\infty} \frac{e^{itx}}{x^2 + 1} \, dx$$ which arises in probability theory and can't be solved using basic calculus.

The Residue Theorem can also be used to solve the very famous [Basel Problem](https://en.wikipedia.org/wiki/Basel_problem) which states that $$\sum_{n=1}^{\infty} \frac{1}{n^2} = \frac{\pi^2}{6}$$. This problem was first solved by Euler. The problem can be solved by integrating the function $\frac{\pi \cot(\pi z)}{z^2}$. You might be utterly confused right now looking at the function. But, $\cot(\pi z)$ has poles exactly at the integers we needed and when we tweak it a bit, the residues become related to the series we wanted the sum of. The answer to this problem is too long to go over right now, but is definitely worth trying!




<div class="day-nav-wrapper">
  <a href="./day15.html" class="day-nav__link">Previous: #15</a>
  <a href="./day17.html" class="day-nav__link">Next: #17</a>
</div>