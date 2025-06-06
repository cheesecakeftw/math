---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 10

## [Taylor Series](https://en.wikipedia.org/wiki/Taylor_series)

Definition: Much of complex analysis is (or at least can be) stated in terms of Taylor series. Given a function $$f(z)$$, we can express it as

$$
f(z) = \sum_{n=0}^{\infty}
a_n(z - z_0)^n, \,\  \text{where} \,\ a_n=\frac{f^{(n)}(z_0)}{n!}
$$

for some $$z_0 \in \mathbb{C}$$ and some complex numbers $$a_n$$.

Today we will discuss something most people who have taken calculus are familiar with and extend it to the complex plane. Before we get into the complex plane, lets consider the real function $$f : R \to R$$ where $$f(x)=e^{-1/x^2}$$ when $$x \neq 0$$ and 0 when $$x=0$$. Then $$f$$ is infinitely differentiable at 0, and all its derivatives at 0 are 0, so the power series is simply 0. This is certainly a well behaved power series everywhere, but the problem is that the power series has nothing to do with the actual function $$f$$: it converges to the wrong function. Also, note that $$f$$ doesn't extend to a differentiable function on the neighborhood of 0 in $$C$$. A truly magical aspect of complex analysis is that if we construct a power series for a differentiable function $$f(z)$$ in this way, then it actually converges to $$f(z)$$ in some open neighborhood of $$z_0$$.

Specifically, if $$f:U \to C$$ is a differentiable function and $$z_0 \in U$$ and $$B_r(z_0) \subseteq U$$, then the power series converges to $$f(z)$$ in $$B_r(z_0)$$. We wont go over the proof of this theorem because its long and requires integrals which we haven't introduced yet. Additionally, if $$f$$ has a convergent power series of some positive radius centered at every point of $$U$$, then we say that $$f$$ is holomorphic. Again, we wont be going over the proof yet. Now, we know that the power series will be convergent around $$z_0$$ for sure, but what about the radius of the disk? It turns out there is an elegant formula for that denoted by the [radius of convergence](https://en.wikipedia.org/wiki/Radius_of_convergence): $$ R = \frac{1}{\lim \sup \lvert a_n\rvert ^{1/n}}$$. Here, $$\sup \lvert a_n\rvert$$, represents the maximum the series will attain, which is the definition of [supremum](https://en.wikipedia.org/wiki/Infimum_and_supremum). For example, commonly seen series $$\sum_{n=1}^{\infty} (nz)^n$$, doesn't define an analytic function in the neighborhood of 0 which is quite easy to see intuitively. If $$a_n=n^n$$ then, $$ \lvert a_n\rvert ^{1/n}=n$$, so $$\lim \sup n = \infty$$, so the radius of converge is 0.

For this R, the series converges if $$\lvert z-z_0 \rvert <R$$ and diverges if  $$\lvert z-z_0 \rvert >R$$. But what about $$\lvert z-z_0 \rvert =R$$? This situation is much more complicated. It may converge everywhere on the circle, diverge everywhere or might converge at some points and diverge at some points (Evaluate $$f(z)= \sum_{n=1}^{\infty} \frac{z^n}{n^2}$$ at $$R$$ ). 

Now lets analyze an interesting phenomenon of real functions, define $$f(x)=\frac{1}{x}$$, which has the power series expansion $$\sum_{n=0}^{\infty}x^n$$, which converges when  $$ \lvert x\rvert <1$$. This makes sense because at $$x=1$$ $$f(x)$$ becomes undefined. Now consider $$f(x)=\frac{1}{1+x^2}$$. Its power series expansion is $$\sum_{n=0}^{\infty}(-1)^nx^{2n}$$, which converges at $$ \lvert x\rvert <1$$. But, why? Nothing bad at happens at $$x=1$$. But when we consider what happens in all of $$C$$ as well, then something bad does indeed happen at $$x=±i$$. So, it makes sense only when we consider things from the complex point of view as well.


<div class="day-nav-wrapper">
  <a href="./day9.html" class="day-nav__link">Previous: #9</a>
  <a href="./day11.html" class="day-nav__link">Next: #11</a>
</div>