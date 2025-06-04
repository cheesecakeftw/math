---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 5

## [Uniform and Pointwise Convergence](https://en.wikipedia.org/wiki/Uniform_convergence)

Definition: If there is some function $$f : U \to \mathbb{C}$$ such that for every $$\varepsilon > 0$$, there is some $$N > 0$$ so that whenever $$z \in U$$ and $$n > N$$, then $$\lvert f_n(z) - f(z) \rvert < \varepsilon$$, then we say that $$f_n$$ converges uniformly to $$f$$.

Now that we are talking about limits, lets see what would be the "limit" of a sequence. The easiest way to understand convergence is through an example! Consider the functions $$ f_n : [0,1] \to R$$ defined by $$f_n(x)=x^n$$. Now, lets consider the limits: for any $$x \in [0,1)$$, $$\lim_{n \to \infty} f_n(x) = 0$$, but $$\lim_{n \to \infty} f_n(1) = 1$$. Thus, the functions $$f_n$$ converge to the function $$f$$, where $$f(x)=0$$ when $$x \neq 1$$ and $$f(x)=1$$ when $$x=1$$. But because the limit of $$f_n(x)=f(x)$$ we say that $$f_n$$ specifically [converges pointwise](https://en.wikipedia.org/wiki/Pointwise_convergence) to $$f$$.

But, why doesn't the case we talked about exhibit uniform convergence? Because for any $$\varepsilon > 0$$, no single $$N$$ works for all $$x \in [0,1]$$. As $$x \to 1$$, $$f_n(x) = x^n$$ gets closer to 1, so you need larger and larger $$n$$ to make $$\lvert f_n(x) - f(x) \rvert < \varepsilon$$. No matter what $$N$$ you pick, you can always find some $$x$$ close enough to 1 where $$f_n(x)$$ hasn’t gotten close to 0 yet, so you can’t find a uniform $$N$$ that works for all $$x \in [0,1]$$. Hence, for the functions to exhibit uniform convergence they must meet all the criteria in the definition, and if they don't they can still exhibit pointwise convergence if they show convergence for each $$x$$ individually.

Basically, $$\textbf{uniform convergence}$$ can be simply explained as having all $$f_n$$'s lie completely inside an $$\varepsilon$$ tube around $$f$$. Uniform convergence is preferred compared to pointwise convergence because a sequence of functions that exhibits uniform convergence will have nicer properties:
- If all the converging sequences $$f_n$$ are continuous, then $$f$$ will also be continuous

Finally, lets connect the dots by relating it back to infinite series, we find that if $$\lvert f_n(x) \rvert \leq M_n$$ and that $$\sum_{n=1}^{\infty} M_n < \infty.$$ then $$\sum_{n=1}^{\infty} f_n(x).$$ converges. This is known as the [Weierstrass M-test](https://en.wikipedia.org/wiki/Weierstrass_M-test). We will prove this theorem later when we have the necessary tools to do so. Also, for any compact interval $$[a,b]$$ in $$R$$ and any continuous function $$f : [a,b] \to R$$, there exists a sequence $$p_1, p_2, \dots$$ of polynomials converging uniformly to $$f$$ on $$[a,b]$$. The proof of this statement is fairly rigorous but can be done using the Mean value theorem, which we explore later.



<div class="day-nav-wrapper">
  <a href="./day4.html" class="day-nav__link">Previous: #4</a>
  <a href="./day6.html" class="day-nav__link">Next: #6</a>
</div>