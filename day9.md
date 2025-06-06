---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 9

## [Liouville's Theorem](https://en.wikipedia.org/wiki/Liouville%27s_theorem_(complex_analysis))

Definition: Every holomorphic function $$f : \mathbb{C} \to \mathbb{C}$$ for which there exists a positive number $$M$$ such that $$ \lvert f(z) \rvert \leq M$$ for all $$z \in \mathbb{C}$$ is constant.

Yesterday, we discussed differentiability on the complex plane. Now, we tie it back to one of the main classes of functions that we study in complex analysis, the so-called [holomorphic functions](https://en.wikipedia.org/wiki/Holomorphic_function). For any open set $$ U \subseteq C$$ and $$f :C \to C$$, if $$f$$ is differentiable at every point (i.e. the real and imaginary parts of $$f$$ satisfy the Cauchy–Riemann equations) then we say that $$f$$ is a holomorphic function. For some $$z_0 \in U$$ we say that f is holomorphic at $$z_0$$ if it is holomorphic in some neighborhood of $$z_0$$. This just means that for a function to be holomorphic at a point we must check some disk such that $$ \lvert z-z_0 \rvert < \varepsilon$$ for some $$\varepsilon>0$$.

It is important to note that holomorphic functions are often referred to as analytic functions. However, analytic functions are based on having a convergent power series, which we look over later. Luckily, the two notions are equivalent in the case of complex functions. Another important related notion: A holomorphic function $$f : \mathbb{C} \to \mathbb{C}$$ (i.e., one defined on all of $$\mathbb{C}$$) is said to be an entire function. Additionally, holomorphic functions have some really nice properties. Let $$f$$ and $$g$$ be two holomorphic functions on some open set $$U \subseteq \mathbb{C}$$; then $$f \pm g$$ and $$fg$$ are holomorphic on $$U$$, and if $$g(z) \neq 0$$ for all $$z \in U$$, then $$\frac{f}{g}$$ is also holomorphic; moreover, if $$f : U \to V$$ and $$g : V \to \mathbb{C}$$ are holomorphic, then $$g \circ f : U \to \mathbb{C}$$ is also holomorphic. While we wont prove these properties, the proofs aren't too hard and are based on using the definition of a limit for a function. 

Liouville's Theorem has a quite elegant proof. Given two points, choose two balls with the given points as centers and of equal radius. If the radius is large enough, the two balls will coincide except for an arbitrarily small proportion of their volume. Since $$f$$ is bounded, the averages of it over the two balls are arbitrarily close, and so $$f$$ assumes the same value at any two points. $$\square$$ There is another commonly used proof involving Cauchy's Integral Formula which we will discuss later.

An important improvement of this theorem is [Picard's Little Theorem](https://en.wikipedia.org/wiki/Picard_theorem) which states that if $$f$$ is an entire function, and there exists two complex numbers $$w_1$$ and $$w_2$$, such that for all $$z \in C$$, $$f(z) \neq w_1$$ and $$f(z) \neq w_2$$, then $$f$$ is constant. This theorem is much stronger because  a bounded function misses lots of values: in fact, a function bounded by $$M$$ misses every complex number $$w$$ with $$\lvert w \rvert \geq M$$. We will also discuss another extremely important corollary of this theorem, that you are probably familiar with, called the [Fundamental theorem of algebra](https://en.wikipedia.org/wiki/Fundamental_theorem_of_algebra) later.



<div class="day-nav-wrapper">
  <a href="./day8.html" class="day-nav__link">Previous: #8</a>
  <a href="./day10.html" class="day-nav__link">Next: #10</a>
</div>