---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 37

## [Wilson's Theorem](https://en.wikipedia.org/wiki/Wilson%27s_theorem)

Definition: A natural number $n>1$ is a prime if and only if $(n-1)!\equiv -1\pmod{n}$.

This theorem is an elementary number theory result that is quite well known and helps us build to some really important parts of number theory. Note that this is a biconditional statement so we must prove both sides. 

Let us begin with the forwards direction. Let $p$ be a prime. The result is trivial for $p=2$, so let p be an odd prime. Since, $\mathbb{Z}_p$ is a field, because every element in it is coprime to $p$ each element has a unique inverse in the field. By Euclid's lemma we know that the only values with $a\equiv a^{-1}\pmod{p}$ are $a=1,-1$. Hence, with the exception of those numbers, every other element of $(p-1)!$ can be arranged in pairs such that the product of each pair is congruent to $1$. Multiplying the factors out we get, $(p-1)!\equiv-1\pmod{p}$, completing the proof.

Now we prove the reverse direction. Assume for the sake of contradiction that $n$ is composite. Then some prime $q<n$ exists such that $q\mid n$ and $k\in \mathbb{Z}$ such that $n=qk$. Then, $(n-1)!=mn-1=q(km)-1$ for some integer $m$ by rewriting $(n-1)!\equiv -1\pmod{n}$. Then, $(n-1)$ must be one less than a multiple of $q$. But, since $q\leq n-1$, one of the factors in the expanded product of $(n-1)!$ must be $q$. Hence, $(n-1)!\equiv 0 \pmod{q}$, which gives us a contradiction. Hence, $n$ must be prime.

This theorem could also be proved by considering the polynomial $f(x)=x^p-1$ which has $p-1$ roots, $1,2,\ldots,p-1$ by Fermat's Little Theorem. We will go over this proof later because this requires Lagrange's Theorem. A common application of this theorem is to show that for any odd prime $p\equiv 1 \pmod{4}$, there exists $x^2\equiv -1\pmod{p}$. We know that $(p-1)!\equiv -1\pmod{p}$. Pairing each $x=1,\ldots,(p-1)/2$ in the expansion with $(p-x)=-x$ we get that $(p-1)!\equiv\prod_{x=1}^{(p-1)/2} (-x)^2= (-1)^{\frac{p-1}{2}}((\frac{p-1}{2})!)^2$ Since, $p\equiv 1 \pmod{4}$, $(p-1)/2$ is even. Hence, $((\frac{p-1}{2})!)^2\equiv-1 \pmod{p}$. There's a lot more to what just happened, and we will explore this later!


<div class="day-nav-wrapper">
  <a href="./day36.html" class="day-nav__link">Previous: #36</a>
  <a href="./day38.html" class="day-nav__link">Next: #38</a>
</div>


