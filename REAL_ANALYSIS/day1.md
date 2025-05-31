---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 1

## Cauchy Sequences

$$\forall \varepsilon > 0,\ \exists N \in \mathbb{N}, \,\ \forall m,n > N,\left| x_m - x_n \right|<\varepsilon$$

Definition: Let $$x_1,x_2,\ldots$$ be a sequence of rational numbers. Then we can call this sequence a Cauchy sequence if for every $$
\varepsilon>0$$, there is some $$N>0$$ so that whenever $$m,n>N$$, then $$\left| x_m - x_n \right|<\varepsilon$$

To start this math series lets discuss one of the cornerstones of analysis, a theorem which explains how to approximate a real number without taking the ratio! One really interesting property that shows if a sequence is Cauchy is that it always converges. The converse, that if a sequence has a limit, then it is Cauchy, is also true. A sequence converging just means that as the sequence progresses it is getting closer and closer to a particular number. It could also be said that the distance between the n-th term and the number the sequence converges to is reducing.

A really cool example of this idea would be the expansion of $$\sqrt{2}$$. The sequence defined as 
$$x_0 = 1, x_1 = \frac{3}{2}, x_2 = \frac{17}{12}, x_3 = \frac{577}{408}, \ldots$$ 
where $$x_{n+1} = \frac{1}{2} \left(x_n + \frac{2}{x_n} \right)$$
would want to converge to $$\sqrt{2}$$. For this sequence, for any given $\varepsilon>0$, we can always find some $m,n > N$ such that $\lvert x_m - x_n\rvert < \varepsilon$ because the difference between $$x_n$$ and $$x_m$$ is increased by a decimal place, making it smaller: the numbers get arbitrarily closer as the sequence goes on, allowing us to fulfill the criteria for any  $\varepsilon>0$ by choosing $m$ and $n$ appropriately.

Note that Cauchy Sequences do not converge in every space. In the previous example our sequence was converging to $$\sqrt{2}$$ but $$\sqrt{2}\notin \mathbb{Q}$$. A space where all Cauchy sequences converge is called a **complete space**. Also, if we have two Cauchy sequences $$(a_n)$$ and $$(b_n)$$, then $$(a_n+b_n)$$ and $$(a_n \cdot b_n)$$ are also Cauchy sequences. We do however need to prove that these operations are well defined based on the spaces of the sequences (which is quite rigorous).

Another important property is that, in any space, a Cauchy sequence is bounded. This is because if $d$ is the farthest any earlier term is from $x_N$, then every term is within $d + 1$ of $x_N$, so the sequence is bounded. Also note that if $$f : M \to N$$ is a uniformly continuous map between the metric spaces $$M$$ and $$N$$ and $$(a_n)$$ is a Cauchy sequence in $$M$$, then $$(f(a_n))$$ is also a Cauchy sequence in $$N$$. These properties allow us to derive the [Bolzano–Weierstrass theorem](https://en.wikipedia.org/wiki/Bolzano%E2%80%93Weierstrass_theorem), which states that every bounded sequence has a convergent subsequence. This theorem can be applied to all Cauchy sequences in $$\mathbf{R}$$.

<div class="day-nav-wrapper">
  <a href="./day2.html" class="day-nav__link">Next: #2</a>
</div>
