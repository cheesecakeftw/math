---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 40

## [Fermat's Sandwich Theorem](https://mathworld.wolfram.com/FermatsSandwichTheorem.html)

Definition: If $x,y\in \mathbb{Z},$ $y^2=x^3-2$ has only $2$ sets of solutions.

Fermat shown that $26$ is the only number sandwiched between a perfect square number ($5^2=25$) and a perfect cubic one ($3^3=27$). It is easy to see that $(x,y)=(3,\pm 5)$ because $27-25=2$.
The funny thing is that while Fermat claimed that there are only 2 solutions he never bothered proving it, and left is as challenge to other french mathematicians.

The proof of this theorem is nontrivial but doable using the tools we have gone over. To solve this consider arithmetic in $\mathbb{Z}[\sqrt{-2}]$. To start we rewrite the equation in the ring $\mathbb{Z}[\sqrt{-2}]$ to get $(y+\sqrt{-2})(y-\sqrt{-2})=x^3$. We can show that the ring is Euclidean which implies that its a PID. But PIDs are UFDs, hence $\mathbb{Z}[\sqrt{-2}]$ is a UFD. The Norm function of this ring is $N(a+b\sqrt{-2})=a^2+2b^2$. Firstly, we notice that $y$ is odd. If $y$ were even then $4\mid x^3-2$ implies $ x^3\equiv 2\pmod{4}$. But cubes modulo $4$ can never be $2$, hence $y$ must be odd.

Now, consider an irreducible (can't be factored nontrivially) $p$ which divides both $(y+\sqrt{-2})$ and $(y-\sqrt{-2})$. Then it divides $2\sqrt{-2}=-(\sqrt{-2})^3$. Then $p$ must be $\sqrt{-2}$ since $\sqrt{-2}$ is an irreducible. Then, $\sqrt{-2}\mid y$, which is impossible since $y$ is odd. Hence, $(y+\sqrt{-2})$ and $(y-\sqrt{-2})$ are coprime, such that they have no irreducible factors. Since, their product is a cube, from their UPFs it isn't hard to see that they both must be cubes times units. Since, the only units in $\mathbb{Z}[\sqrt{-2}]$ are $\pm 1$, which are cubes, $(y+\sqrt{-2})$ and $(y-\sqrt{-2})$ are cubes.

Hence, for some $a+b\sqrt{-2}$, $y=(a+b\sqrt{-2})^3$. Expanding and equating coefficients we get that $y=a^3-6b^2a$ and $1=3a^2b-2b^3=b(3a^2-2b^2)$. From, the second one, $b=\pm 1$ and $(3a^2-2b^2)=\pm 1$. So, $3a^2=2\pm 1$, and since $3a^2=1$ is impossible, the only solution is $a=1$. From, that we get  $y=-5,5$. Plugging it into the original equation we get that $x=1$. Hence, the only two solutions are $(x,y)=(3,\pm 5)$!




<div class="day-nav-wrapper">
  <a href="./day39.html" class="day-nav__link">Previous: #39</a>
  <a href="./day41.html" class="day-nav__link">Next: #41</a>
</div>


