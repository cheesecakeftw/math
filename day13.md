---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 13

## [The Cauchy Integral Theorem](https://en.wikipedia.org/wiki/Cauchy%27s_integral_theorem)

Definition: Let $\Gamma$ be a closed contour in $\mathbb{C}$, and suppose that $f(z)$ is holomorphic on $\Gamma$ and its interior. Then 
$$
\int_{\Gamma} f(z)\, dz = 0.
$$

Today we properly go over one of the most celebrated complex analysis theorems, after foreshadowing it yesterday. One important thing to remember is that this shouldn't be confused with the Cauchy Integral Formula, which we go over later. The real power of complex analysis comes from results such as the Cuachy Integral Formula and the residue theorem, which are built upon this theorem. Regardless, we can still compute some integrals that would be really tough without complex analysis using this theorem. How would you evaluate $\int_{-\infty}^{\infty} \frac{1-\cos x}{x^2}dx = \pi $ without complex analysis? Give it a try, but with complex analysis its a standard answer. We won't be going over the entire proof because its too long for this blog, but it isn't too hard and makes use of the Cauchy Integral Theorem and the ML Inequality, tools which we have gone over.

Before we evaluate that integral, lets prove the Cauchy Integral theorem with only the additional hypothesis that $$f'$$ is continuous on $\Gamma$ and its interior. It turns out that the proof is quite simple and follows from a main theorem in multivariable calculus called [Green's Theorem](https://en.wikipedia.org/wiki/Green%27s_theorem). Green’s Theorem states that for a positively oriented, closed curve $\Gamma$ enclosing a region $D$,$$ \int_{\Gamma} (P\, dx + Q\, dy) = \iint_D \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right) dx\,dy
$$. Moving onto the proof, firstly we write $$f(z)=u(x,y)+iv(x,y)$$ and $$dz=dx+idy$$, from the definition of a complex function. Then, $$
\int_{\Gamma} f(z)\, dz = \int_{\Gamma} \left( (u(x, y)\, dx - v(x, y)\, dy) + i(u(x, y)\, dy + v(x, y)\, dx) \right)$$ after multiplying. Then, By Green's Theorem, we have $$
\int_{\Gamma} f(z)\, dz = \iint_{D} \left[ \left( -\frac{\partial v}{\partial x} - \frac{\partial u}{\partial y} \right) + i\left( \frac{\partial u}{\partial x} - \frac{\partial v}{\partial y} \right) \right].
$$ By the Cauchy-Reimann equations, we have $\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}$ and $\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}$. Hence, the integrand of the double integral is $0$. $\blacksquare$

One important consequence of the Cauchy Integral Theorem is that the integral of a function along a closed contour doesn't depend heavily on the choice of contour. The contour could be a square, semicircle or even keyhole shaped. Also, an interesting fact: we say that $\Gamma$ is nullhomologous and if the contour is composed of $\Gamma_1$ and $\Gamma_2$ curves then, $$
\int_{\Gamma_1} f(z)\, dz = \int_{\Gamma_2} f(z)\, dz $$ since they have to add up to 0. Similarly, we can manipulate larger combinations of $\Gamma_n$ too. Now that we have talked about integrating holomorphic functions, where we find that the integral of a holomorphic $f(z)$ over a closed contour takes on very special values, lets consider $\bar z $ which is not a holomorphic function. In fact, we call it an [antiholomorphic function](https://en.wikipedia.org/wiki/Antiholomorphic_function). It seems that $\bar z $ has a lot in common with holomorphic functions, so maybe it has similar properties with respect to integrals? It turns out thats not the case at all! For a closed contour $\Gamma$ with area $D$, $$\int_{\Gamma} \bar{z}\, dz = 2i \times \text{Area}(D)$$. This can be easily shown using Green's Theorem again. Since, $$ D \in \mathbb{R}$$ and $ D > 0$, the integral can take on any purely imaginary positive value, which is quite a contrast from a holomorphic function!



<div class="day-nav-wrapper">
  <a href="./day12.html" class="day-nav__link">Previous: #12</a>
</div>
