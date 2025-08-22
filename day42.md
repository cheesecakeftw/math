---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 42

## [Freshman's Dream](https://en.wikipedia.org/wiki/Freshman%27s_dream)

Definition: $(x+y)^p=x^p+y^p$ in $\mathbb{Z}_p$ and $(f(x))^p \equiv f(x^p) $ in the ring of polynomials $\mathbb{Z}_p[x]$ when $p$ is a prime.

The funny thing is that this equation is one of the most well known erroneous equations for the case $n\in \mathbb{N}$ and integers $x,y\neq 0$. When we all saw equations of the form $(a+b)^2$, $(a+b)^3$ for the very first time most of us thought that the powers distribute over the terms to give $(a+b)^2=a^2+b^2$ and $(a+b)^3=a^3+b^3$. Hence, the name! But, it is quite easy to see using distributivity why this result is false (or just a counterexample). But, maybe we can salvage this "dream" for it to be true somewhere.

It turns out that you can! This mistake ends up being true in commutative rings modulo $p$. Consider the expansion $(x+y)^p$ where $p$ is prime and $x,y\in \mathbb{Z}_p$. Using the [binomial theorem](https://en.wikipedia.org/wiki/Binomial_theorem) we know that the nth coefficient will be $\binom{p}{n} = \frac{p!}{n!\,(p-n)!}.$ When $0<n<p$ both $n!$ and $(p-n)!$ are coprime with $p$ since all factors are less than $p$. Since, a binomial coefficient is always an integer, the nth coefficient will be divisible by $p$ because $n<p$ leaving atleast one factor of $p$ in the coefficient making the term $0$ in the ring $\mathbb{Z}_p$. The only terms that remain are when $n=0$ and $n=p$, which have coefficients $1$. Hence, $(x+y)^p=x^p+y^p$.

This can be extended to the polynomial ring too. Here, there is a special identity which states that $(x+1)^p\equiv x^p+1$ in the ring $\mathbb{Z}p[x]$ for prime $p$. Note that the theorem holds for any polynomial $f(x)=a_nx^n+a_{n-1}x^{n-1}+\ldots +a_0$ such that $(f(x))^p = a_nx^{np}+a_{n-1}x^{(n-1)p}+\ldots +a_0$.  The proof of this follows from the proof in $\mathbb{Z}_p$ since $a_n^p\equiv a_n$ by Fermat's Little theorem! This identity helps us compute polynomials like $(x^2+x+1)^{5}\equiv x^{10}+x^{5}+1$ in $\mathbb{Z}_5[x]$ in seconds. Can you find $(x^2+x+1)^{25}$ in the same ring? What about $(2x^2+x+1)^{125}$?



<div class="day-nav-wrapper">
  <a href="./day41.html" class="day-nav__link">Previous: #41</a>
  <a href="./day43.html" class="day-nav__link">Next: #43</a>
</div>


