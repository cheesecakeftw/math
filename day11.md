---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 11

## [Singularities](https://en.wikipedia.org/wiki/Singularity_(mathematics))

Definition: $$\varepsilon > 0,\ B_\varepsilon(z_0) \setminus \{z_0\} \subseteq U$$. Then $$z_0$$ can be called an isolated singularity.

Today we talk about one of the coolest topics in complex analysis and introduce a new type of series! If $$f$$ is only defined in a deleted neighborhood of $$z_0$$, then it might still be possible to express $$f$$ as a series of the form $$\sum_{n=-\infty}^{\infty} a_n (z-z_0)^n$$. This series is called a [Laurent Series](https://en.wikipedia.org/wiki/Laurent_series). Before, we talk about how a Laurent Series relates to singularities specifically, lets talk about what is a singularity. Suppose that $z_0 \in \mathbb{C}$, and $U \subseteq \mathbb{C}$ is some open subset such that $z_0 \notin U$, but $U$ contains some deleted neighborhood of $z_0$: i.e. $B(z_0, \varepsilon) = \{ z \in \mathbb{C} : 0 < \lvert z - z_0 \rvert < \varepsilon \} = \{ z \in \mathbb{C} : \lvert z - z_0 \rvert < \varepsilon \} \setminus $ {$$ z_0 $$}.Then for an analytic function $f : U \to \mathbb{C}$ we call $$z_0$$ an isolated singularity. 

Furthermore, there are 3 types of behaviors that these singularities can exhibit:
- If there is a continuous function $g : U \cup \{ z_0 \} \to \mathbb{C}$ such that $g(z) = f(z)$ for any $z \in U$, then we say that $z_0$ is a **removable singularity** of $f$.
- If $\lim_{z \to z_0} f(z) = \infty$, then we say that $z_0$ is a **pole** of $f$.
- If $\lim_{z \to z_0} f(z)$ does not exist and is not $\infty$, then we say that $z_0$ is an **essential singularity** of $f$

Now lets go over an example. Consider $f : \mathbb{C} \setminus $ {$$ -1 $$} $ \to \mathbb{C}$ which is defined by $f(z) = \frac{z^2 - 1}{z + 1}$. Then $-1$ is a removable singularity, since defining $f(-1) = -2$ extends $f$ to a continuous function on $\mathbb{C}$. The singularity only rose when we defined the function wrong. (Similarly, consider $$\frac{\sin(z)}{z}$$ and try to use series!). Now lets consider $$f(z)=e^{\frac{1}{z}}$$ on $$ C \setminus$$ {$$ 0 $$} where we claim that $$z=0$$ is an essential singularity. To see this, approach $z = 0$ along the negative real axis: $z = -c$ for small positive $c$, giving $f = e^{-1/c} \to 0$ as $c \to 0$. Similarly, the limit along the positive real axis, the limit is $\infty$. Similarly, try finding the poles of $$f(z)=\frac{z^2+1}{z^2-z}$$! Now, lets consider a really cool special case, $$f(z)=\log z$$. Then $z = 0$ seems like an isolated singularity of $f(z)$, but it is not. Since $\log z$ is multivalued, we define a branch by removing the negative real axis and $0$. However, every neighborhood of $0$ contains points on the negative real axis. Thus, we don't have a function defined in a neighborhood of 0.

Finally, lets go back to how does the Laurent Series relate to Singularities. It turns out we can detect types of singularities from Laurent expansions! Suppose $f$ is holomorphic in a deleted neighborhood of $z_0$ and has a Laurent series expansion
$$
\sum_{n=-\infty}^{\infty} a_n (z - z_0)^n
$$
centered at $z_0$. Then if $a_n = 0$ for all $n < 0$, then $f$ has a removable singularity at $z_0$. If there is some $n < 0$ with $a_n \ne 0$, but only finitely many such terms, then $f$ has a pole at $z_0$.Finally, if there are infinitely many $n < 0$ with $a_n \ne 0$, then $f$ has an essential singularity at $z_0$. While we won't prove this because the proof is lengthy, it is a fairly simple proof using integrals. 

Additionally, there are some shocking theorems that are directly related to singularities! One of them is the [Casorati–Weierstrass](https://en.wikipedia.org/wiki/Casorati%E2%80%93Weierstrass_theorem) theorem, which states that for any essential singularity $z_0$ of $f$, and for every deleted neighborhood $V$ of $z_0$, $f(V)$ is dense in $\mathbb{C}$; that is, for every $w \in \mathbb{C}$ and every $\varepsilon > 0$, there exists $z \in V$ such that $\lvert f(z) - w \rvert < \varepsilon$. This theorem's stronger and much more difficult version is widely used and known as [Picard's Great Theorem](https://en.wikipedia.org/wiki/Picard_theorem), which we will discuss later. The proofs of both of these theorem's require tools we haven't discussed yet, so we won't be going over them as of now.

<div class="day-nav-wrapper">
  <a href="./day10.html" class="day-nav__link">Previous: #10</a>
  <a href="./day12.html" class="day-nav__link">Next: #12</a>
</div>