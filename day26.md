---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 26

## [Euclidean Domain](https://en.wikipedia.org/wiki/Euclidean_domain)

Definition:  Let $R$ be a nontrivial commutative ring such that $ab=0\implies a=0$ or $b=0$. If $a,b \in R$ with $b\neq 0$, $ \exists \, q,r \in R $ such that $a=bq+r$ and $f(r)<f(b)$ or $f(r)=0$ for some euclidean function $f$. 

The formula above is something we have all seen since the time we learned long division but just haven't realized it. Given $a,b>0$ when we divide $a$ by $b$ using long division we always get two integers: the remainder $r$ and quotient $q$ at the end. We can represent this as $a=bq+r$. Notice, that $r$ will always be smaller than $b$. 

Now consider the ring [$\mathbb{R}[x]$](https://en.wikipedia.org/wiki/Polynomial_ring). This is a ring representing polynomials with real coefficients (We can also take $\mathbb{Z}[x]$ or $\mathbb{R}[x]$ which are subsets of $R[x]$). If $a(x),b(x) \in \mathbb{R}[x]$ are two polynomials such that $b(x)$ isn't a constant, then we can use polynomial long division to divide $a(x)$ by $b(x)$, which is something we learn in school too. Again, we get the polynomial quotient $q(x)$ and remainder $r(x)$, such that $a(x)=b(x)q(x)+r(x)$. We can't have $r(x)<b(x)$ since polynomials cant be compared by such an operator. But our definition allows for a function which is the degree function in this case s.t. $0 \leq\deg r(x)<\deg b(x)$. This allows us to prove one side of the [factor theorem](https://en.wikipedia.org/wiki/Factor_theorem). Consider a polynomial $f(x)$ where $f(a)=0$. Let $b(x)=x-a$ and then long division to get $f(x)=(x-a)q(x)+r(x)$ where $f(a)=(a-a)q(x)+r(x) \implies r(x)=0$. Hence, $(x-a)$ divides $f(x)$.

Note, that we defined the ring $R$ as such in the definition because for a space to be euclidean we need an [integral domain](https://en.wikipedia.org/wiki/Integral_domain) such that there are unique quotients and remainders, which requires the absence of zero divisors. We will show why later!

Similarly, consider the ring [$\mathbb{Z}[i]$](https://en.wikipedia.org/wiki/Gaussian_integer) which is the ring of Gaussian integers where an element $x\in \mathbb{Z}[i]$ is defined as $x=a+bi$ for some $a,b \in \mathbb{Z}$. We define the norm function $N(x)=N(a+bi)$ as $a^2+b^2$. We will prove the division algorithm exists in $\mathbb{Z}[x]$ and $\mathbb{Z}[i]$ later. Try to conjecture if $\mathbb{Z}[\sqrt{2}]$ where the Norm function is $a^2-2b^2$ is euclidean or not! What about $\mathbb{Z}[\sqrt{-5}]$?





<div class="day-nav-wrapper">
  <a href="./day25.html" class="day-nav__link">Previous: #25</a>
  <a href="./day27.html" class="day-nav__link">Next: #27</a>
</div>