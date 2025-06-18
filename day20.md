---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 20

## [Infinite Products](https://en.wikipedia.org/wiki/Infinite_product)

Definition: The infinite product of complex numbers $z_1, z_2, \ldots$ is denoted as $$\prod_{n=1}^\infty z_n$$ to be the limit of the finite products, $$\prod_{n=1}^N z_n$$ if
this limit exists, and is nonzero.

Today we take a step back from all those complicated theorems and discuss something more intuitive and fun. Before we get into how these products relate to complex analysis specificifically lets go over the situation with zero. For a product to equal to 0 one of the terms has to be 0, which is problematic, because like series, we want convergence of a product only to depend on the tail of the sequence, but not the product. So we can say that the product converges iff finite $z_n$ are 0 and some nonzero subsequence converges in the above sense. Hence, it is clear that if a product converges, then $\lim_{n \to \infty} z_n=1$; the converse, of course, fails. 

Now that we know that an infinite product must tend to 1 in order to have some hope of converging, it makes sense to write $z_n=1+a_n$ and consequently consider the product $\prod_{n=1}^\infty (1+a_n)$. Now, one logical thing we can do is to take the logarithm of the product to convert it to a sum by choosing a branch cut that doesn't go through the $z_n$'s. Hence, $$\log\prod_{n=1}^\infty (1 + a_n) = \sum_{n=1}^\infty \log(1 + a_n)$$. Now, the product converges iff the sum converges. But when does the sum converge? Let us get rid of the logarithms first. Recall that $log(1+z)=z-\frac{z^2}{2}+\frac{z^3}{3}-\ldots$ from its expansion. If $\lvert z \rvert$ is very small, $\log(1+z) \approx z$, so that $\lim_{a\to 0}\frac{log(1+a)}{a}=1$. Now, according to the [Limit Comparison test](https://en.wikipedia.org/wiki/Limit_comparison_test), for two sequences $a_n$ and $b_n$ if $\lim_{n\to \infty} \frac{a_n}{b_n} =1$, then either both the series converge or neither one does. It follows that $$\sum_{n=1}^{\infty} \log(1+\lvert a_n \rvert)$$ and  $$\sum_{n=1}^{\infty} \log(\lvert a_n \rvert)$$ either both converge or diverge. Hence, an infinite product $$\prod_{n=1}^\infty (1 + a_n)$$ [converges absolutely](https://en.wikipedia.org/wiki/Absolute_convergence) if $$\prod_{n=1}^\infty (1 + \lvert a_n\rvert)$$ converges. Hence, for the absolute converge of the product the converge of $$\sum_{n=1}^\infty (\lvert a_n \rvert)$$ is absolutely crucial.

A really important property of absolutely convergent series and products is that we can freely rearrange the terms, which is not the case in conditionally convergent series. Note that infinite products can be used to for famous expansions such as the constant $\pi$ which is given through the [ Wallis product](https://en.wikipedia.org/wiki/Wallis_product): $$
\frac{\pi}{2} = \prod_{n=1}^\infty \frac{4n^2}{4n^2 - 1} = \left( \frac{2}{1} \cdot \frac{2}{3} \cdot \frac{4}{3} \cdot \frac{4}{5} \cdot \frac{6}{5} \cdot \frac{6}{7} \cdots \right)$$. While we won't prove it here (mostly because the proof is too long) infinite products are crucial to understanding and proving the [Weierstrass factorization theorem](https://en.wikipedia.org/wiki/Weierstrass_factorization_theorem). The theorem states that if $a_n$ is a sequence sorted by absolute value, so that $a_n \to \infty$ as $n \to \infty$, then $$ f(z) = z^m \prod_{n=1}^\infty \left(1 - \frac{z}{a_n}\right) e^{p_n(z/a_n)}$$ is an entire function that vanishes at 0 (if $m > 0$) and the $a_j$’s and nowhere else, so that the order of the zero at $a$ is equal to the number of occurrences of $a$ in the sequence. This theorem is used quite frequently in complex analysis and allows us to prove other important theorems such as the one we discuss tomorrow!



<div class="day-nav-wrapper">
  <a href="./day19.html" class="day-nav__link">Previous: #19</a>
  <a href="./day21.html" class="day-nav__link">Next: #21</a>
</div>