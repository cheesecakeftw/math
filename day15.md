---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 15

## [Maximum Modulus Principle](https://en.wikipedia.org/wiki/Maximum_modulus_principle)

Definition: Suppose that $U \subseteq \mathbb{C}$ is a connected open set and $f : U \to \mathbb{C}$ is holomorphic. If there exists some $z_0$ so that
$$\lvert f(z_0) \rvert \geq \lvert f(z) \rvert \text{for all } z \in U,$$
then $f$ is constant.

Today, we talk about one of the coolest complex analysis theorems and address how this is an application of the Cauchy Integral Formula. Keep in mind that, connected means "in one piece". If $U$, consisted of say two disjoint open sets, then $f$ could be 0 on one of the sets and 1 on the other, because either set isn't aware of the value of the other set: holomorphicity is a local property. Before, we get into the proof lets go over the Gauss Mean Value theorem, which is a direct consequence of the Cauchy Integral formula and gives a direct proof of the Maximum Modulus Principle. According to the[ Gauss Mean value theorem](https://planetmath.org/proofofgaussmeanvaluetheorem) we have that if $f$ is holomorphic in $$\overline{B_\rho(z_0)}$$ (an open ball centered at $z_0$), then $$ f(z_0) = \frac{1}{2\pi} \int_0^{2\pi} f(z_0 + \rho e^{i\theta})\, d\theta. $$ The proof of this theorem is very straightforward and directly uses the Cauchy Integral formula along the contour $\lvert z-z_0\rvert=\rho$, parameterized by $\gamma(\theta)=z_0+\rho e^{i\theta}$ for $0 \leq \theta \leq 2\pi$.

Now, lets move on to the proof of this theorem! Suppose that $z_0$ is a maximum with $\lvert f(z_0)\rvert \geq \lvert f(z) \rvert$ and choose $\rho > 0$ so that $\overline{B_\rho(z_0)} \subset U$. By Gauss’s formula, $$f(z_0)=\frac{1}{2\pi}\int_0^{2\pi}f(z_0+\rho e^{i\theta}),d\theta,$$ and the ML inequality forces $\lvert f(z)\rvert = \lvert f(z_0)\rvert$ for all $z$ with $\lvert z - z_0\rvert = \rho$. On that circle set $g(z)=f(z)+f(z_0)$, where $z_0$ is again the maximum and using the ML inequality and Gauss' theorem we show that $\lvert g(z_0)\rvert = \lvert g(z) \rvert$ . A second mean value argument gives $\lvert g(z)\rvert=2\lvert f(z_0)\rvert$, so by $$\lvert g(z)\rvert \le \lvert f(z)\rvert + \lvert f(z_0)\rvert = 2\lvert f(z_0)\rvert$$ we conclude $f(z)=f(z_0)$ whenever $\lvert z - z_0 \rvert = \rho$. Choose any point $z_1 \in U$ and a path $\gamma\colon[0,1]\to U$ from $\gamma(0)=z_0$ to $\gamma(1)=z_1$. We then find a sequence of disks centered at points along $\gamma$ contained in $U$. Using the argument above on each disk in succession shows that $f$ remains equal to $f(z_0)$ throughout, hence $f(z_1)=f(z_0)$. Thus, for any arbitrary point $z \in U$, $f(z)=f(z_0)$, so that $f$ is constant. $\blacksquare$

Note, that on a compact set, the story is completely different! We know that, the image of a compact set under a continuous function is compact, so $\lvert f(z) \rvert$ has a maximum on any compact set. Thus, if U is a nonempty bounded open subset of $C$ and $f$ is holomorphic, then $\lvert f\rvert$ has no maximum on $U$ but it does have one on $\lvert U \rvert$. This means that the maximum must lie on the boundary $\partial U$. Also, note that there is a [Minimum Modulus Principle](https://en.wikipedia.org/wiki/Maximum_modulus_principle#cite_note-1) too! It states that if $f$ is a holomorphic function on a connected open set $U \subseteq \mathbb{C}$ and there exists $z_0 \in U$ such that $$0 < \lvert f(z_0) \rvert \leq \lvert f(z) \rvert$$ for all $z$ in some neighborhood of $$z_0,$$ then $f$ is constant on $U$. Finally, there's another stronger related result known as the [Open Mapping Theorem](https://en.wikipedia.org/wiki/Open_mapping_theorem). The theorem states that if $f$ is a nonconstant holomorphic function on an open set $U \subseteq \mathbb{C}$, then $f(U)$ is an open subset of $\mathbb{C}$. We will be using this theorem quite frequently in the future!


<div class="day-nav-wrapper">
  <a href="./day14.html" class="day-nav__link">Previous: #14</a>
  <a href="./day16.html" class="day-nav__link">Next: #16</a>
</div>