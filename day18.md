---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 18

## [Branch Point](https://en.wikipedia.org/wiki/Branch_point)

Definition: A branch point of a multivalued function is a point such that if the function is $$n$$-valued (has $$n$$ values) at that point, all of its neighborhoods contain a point that has more than $$n$$ values.

Today we see how does complex analysis make use of analytic continuation directly. These branch points are really important for us to understand [Reimann Surfaces](https://en.wikipedia.org/wiki/Riemann_surface) which we discuss later! Let us consider the function $$f(z)= \sqrt{z} $$ at $$z=0$$. It isn't differentiable there and it turns out that the situation gets even worse. It turns out that it isn't even a function in the neighborhood of $$z=0$$. let us consider a circle $$\lvert z \rvert = \varepsilon$$, around the origin and look at its image under $$f$$. At $$z=\varepsilon$$, we have $$f(z)=\sqrt{\varepsilon}$$ and at $$z=\varepsilon e^{i\theta}$$, $$f(z)=\sqrt{z}e^{i \theta/2}. But,$$ if $$\theta= 2\pi$$, $$f(z)=\sqrt{\varepsilon}e^{i \pi}=-\sqrt{\varepsilon}$$ and $$\varepsilon e^{2\pi i}=\varepsilon.$$ So we get different of $f$ depending on how we write it. The problem is that $f$ needs to take on two different values at $\varepsilon$ and at every $$z \neq 0$$: every complex number has two distinct square roots and $f$ can't choose between one.

Based on this we can understand branch points intuitively. Let $\Omega \subseteq \mathbb{C}$ be an open set and $f : \Omega \to \mathbb{C}$ a function; for $z_0 \in \Omega$, define the curve $\gamma_\varepsilon(t) = f(z_0 + \varepsilon e^{2\pi i t})$; we say $z_0$ is a branch point of $f$ if, for any sufficiently small $\varepsilon > 0$, the values $\gamma_\varepsilon(0) \ne \gamma_\varepsilon(1)$. This mean's that after we go around a small circle around $z_0$ we don't get back to where we started. But, this isn't enough. If $f$ is a function in $\Omega$, then it must be the case that $\gamma_\varepsilon(0)=f(z_0+\varepsilon)$ is equal to $\gamma_\varepsilon(1)=f(z_0e^{2\pi i}+\varepsilon)$. Hence, we add that if we have information about $f$ in a small portion near $z_0 + \varepsilon$, then we want to extend the domain of $f$ a bit at a time, going around the circle until we get to $z_0e^{2\pi i}+ \varepsilon$; when that happens we can say $z_0$ is a branch point if we don't get back to the value we started with.


Now let us see how this relates to analytic continuity. Let $z_0 \in \mathbb{C}$ and suppose $f$ is holomorphic on a set containing points arbitrarily close to $z_0$; let $\varepsilon > 0$ and $z_1 = z_0 + \varepsilon/2$ with $\lvert z_1 - z_0 \rvert < \varepsilon$; if there exist analytic continuations $f_1$ and $f_2$ of $f$ to regions $U_1 = {z \in \mathbb{C} : \lvert z - z_0 \rvert = \varepsilon/2,\ \Im z \geq \Im z_0}$ and $U_2 = {z \in \mathbb{C} : \lvert z - z_0 \rvert = \varepsilon/2,\ \Im z \leq \Im z_0}$ respectively, such that $f_1(z_1) = f_2(z_1) = f(z_1)$ but $f_1(z_0 - \varepsilon/2) \ne f_2(z_0 - \varepsilon/2)$, then $z_0$ is a branch point of $f$. Through this we can easily conclude that it is not possible to extend $f$ to an analytic function in the neighborhood of $z_0$ even if we remove $z_0$ from consideration: $f$ does not extend analytically to ${z \in \mathbb{C} : 0 < \lvert z - z_0 \rvert < \varepsilon}$ for any $\varepsilon > 0$.

Notice, that this is the exact situation we face when dealing with $f(z)=\sqrt{z}$. It's perfectly balanced as long as we stay away from 0. We could define the function on {$${ z \in \mathbb{C} : \lvert z - 1 \rvert < \tfrac{1}{2} } $$} by specifying that $f(1)=1$. But as soon as the region wraps around 0 we can't define an analytic square root function. Try to figure out a branch point of the [natural logarithm](https://en.wikipedia.org/wiki/Natural_logarithm)!




<div class="day-nav-wrapper">
  <a href="./day17.html" class="day-nav__link">Previous: #17</a>
  <a href="./day19.html" class="day-nav__link">Next: #19</a>
</div>