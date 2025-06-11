---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 14

## [Cauchy Integral Formula](https://en.wikipedia.org/wiki/Cauchy%27s_integral_formula)

Definition: Let $U \subseteq \mathbb{C}$ be an open set, let $\Gamma$ be a positively oriented simple closed contour in $U$ whose interior lies in $U$, and let $f : U \to \mathbb{C}$ be holomorphic. Then, for any $z_0$ in the interior of $\Gamma$, we have  $$f(z_0) = \frac{1}{2\pi i} \int_{\Gamma} \frac{f(z)}{z - z_0}\, dz.$$

Using the Cauchy Integral Theorem, we can do rather astonishing integrals, but with the cauchy Integral Formula, we can do far more. As an immediate consequence of the theorem we can see that holomorphic functions are rather rigid: as soon as we know values of $f$ at every point around $\Gamma$, that pins down the values in the interior of $\Gamma$ too. This is completely different from differentiable functions $R^2 \to R$, where a function that is 0 along $\Gamma$ could be 1 at some point in the interior. This shows just how powerful of a condition complex differentiability is.

Now lets prove this theorem! Consider the function $$F:U \to C$$ which is given by $\frac{f(z)-f(z_0)}{z-z_0}$ when $z \neq z_0$, and $f'(z_0)$ when $z=z_0$. It is clear that F is holomorphic everywhere except $z_0$, so by invariance of the path, we deform $\Gamma$ into a circle $\lvert z-z_0 \rvert = \varepsilon$ around $z_0$ without changing the integral. Hence we have, $\int_{\Gamma} F(z)dz= \int_{\lvert z-z_0 \rvert =\varepsilon} F(z)dz$. By the [ML inequality](https://en.wikipedia.org/wiki/Estimation_lemma), $\lvert \int_{\lvert z-z_0 \rvert =\varepsilon} F(z)dz \rvert \leq \sup_{\lvert z-z_0 \rvert = \varepsilon} F(z) \times 2 \pi \varepsilon$. But $F$ is bounded, say by $M$, in a neighborhood of $z_0$ since $F$ is continuous, which makes it bounded on a compact set, such as $z:\lvert z-z_0 \rvert \leq \varepsilon$. Thus, the integral tends to 0, since it doesn't depend on $\varepsilon$. This implies that $\int_{\Gamma} \frac{f(z)}{z-z_0}dz=f(z_0)\int_{\Gamma}.\frac{dz}{z-z_0}$. Now, we shrink $\Gamma$ to a small circle $\Gamma'$ centered at $z_0$ and using contour integration we can compute that $\int_{\Gamma'}\frac{dz}{z-z_0}=2\pi i$. Hence, $\int_{\Gamma} \frac{f(z)}{z-z_0}dz=2\pi i f(z_0)$. $\blacksquare$

Using this theorem we can compute complex integrals and show results such as $\int_{-\infty}^{\infty} \frac{\cos x}{1+x^2} dx= \frac{\pi}{e}$ or $\int_{-\infty}^{\infty} \frac{dx}{1+x^4} = \frac{\pi}{\sqrt{2}}$. Try showing either of these! (Hint: Use a semi-circle contour and don't forget the poles in the second integral). Under, the hypothesis of the Cauchy Integral formula, we can also show using induction that for $n \geq 0$, we have $$f^{(n)}(z_0) = \frac{n!}{2\pi i} \int_{\Gamma} \frac{f(z)}{(z - z_0)^{n+1}}\, dz.$$ While we won't go into the proof, using this fact we can show that if $f:U \to C$ is holomorphic at a point $z_0 \in U$, then its derivative $f'$ is also holomorphic at $z_0$. This sheds light onto the cool notion that if a complex function is differentiable once, it is differentiable infinitely! Note, that this is not the case for real functions. Try to come up with a function which is differentiable everywhere, but its derivative isn't continuous, which means that $f'$ isn't differentiable either. Another really important consequence is [Morera's Theorem](https://en.wikipedia.org/wiki/Morera%27s_theorem), which states that if $U \subseteq \mathbb{C}$ is an open set and $f : U \to \mathbb{C}$ is a continuous function and for any closed contour $\Gamma$ in $U$, we have $\int_{\Gamma} f(z)dz=0$, then $f$ is holomorphic. Try to find a special result that this theorem gives for every triangle $\Gamma$ in $U$!



<div class="day-nav-wrapper">
  <a href="./day13.html" class="day-nav__link">Previous: #13</a>
  <a href="./day15.html" class="day-nav__link">Next: #15</a>
</div>