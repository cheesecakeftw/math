---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 7

## [Arzelà–Ascoli theorem](https://en.wikipedia.org/wiki/Arzel%C3%A0%E2%80%93Ascoli_theorem)

Definition: Let $$X \subseteq R$$ be a bounded set, and let $$F$$ be a uniformly bounded and uniformly equicontinuous infinite family of functions $$f : X \to R$$. Then there exists a uniformly convergent subsequence $$f_1, f_2, \dots \in F$$. 

Now that we have talked about convergence before, lets talk about equicontinuity and how it relates to the Arzelà–Ascoli theorem. We say that a family of functions $$F$$ is [uniformly equicontinuous](https://en.wikipedia.org/wiki/Equicontinuity) if for all $$\varepsilon>0$$, there exists a $$\delta >0$$, such that whenever $$z,w \in X$$ are such that $$\lvert z-w \rvert < \delta$$, and $$f \in F$$, then $$\lvert f(z)-f(w) \rvert < \varepsilon$$. While, we wont go into it right now, $$F$$ can also be pointwise equicontinuous or uniformly equicontinuous. This relates back to differentiable functions as gives us the property that if $$\lvert f'(x) \rvert \leq M$$ for all $$x \in [a,b]$$, then $$F$$ is uniformly equicontinuous, and if $$F$$ is also uniformly bounded, the Arzelà–Ascoli theorem guarantees a uniformly convergent subsequence. Showing that $$F$$ will be equicontinious is fairly trivial using the [Triangle inequality](https://en.wikipedia.org/wiki/Triangle_inequality). Fascinatingly, this inequality is something that is taught very early but has applications extending to all types of higher math.

However, proving the Arzelà–Ascoli theorem is much more challenging. The proof is a clever diagonalization argument and uses the previously discussed Bolzano–Weierstrass theorem and the Heine Borel Theorem. First, one uses Bolzano–Weierstrass repeatedly on the values at a dense enumeration of rationals to extract a diagonal subsequence that converges at every rational point. Then Heine–Borel lets you cover the closed interval with finitely many small neighborhoods around those rationals, and equicontinuity ensures that being close at each chosen rational forces the functions to be close everywhere. Hence, the subsequence converges uniformly. The full proof is rigorous and pretty long so we wont be showing the complete proof here, but it isn't too hard. Click the heading if you want to see the complete proof! This theorem is crucial in proving the Riemann Mapping Theory in Complex Analysis, which we will discuss later.

The best way to visualize this theorem is to try out an example. On $$[0, \pi]$$, take $$f_n(x) = \frac{\sin(nx)}{n}$$. We have $$\lvert f_n(x) \rvert \leq \frac{1}{n} \leq 1$$ and $$f_n'(x) = \cos(nx) \implies \lvert f_n'(x) \rvert \leq 1$$. So $$\{f_n\}$$ is uniformly bounded and equicontinuous. By Arzelà–Ascoli, some subsequence converges uniformly. One subsequence is $$f_n \to 0$$ which does converge uniformly. Try to find other such subsequences of $$\{f_n\}$$ that converge uniformly!


<div class="day-nav-wrapper">
  <a href="./day6.html" class="day-nav__link">Previous: #6</a>
  <a href="./day8.html" class="day-nav__link">Next: #8</a>
</div>