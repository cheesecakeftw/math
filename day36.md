---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 36

## [Chinese Remainder Theorem](https://en.wikipedia.org/wiki/Chinese_remainder_theorem)

Definition: For two congruences: for any $m_1,m_2$ such that $\gcd(m_1,m_2)=1$, where we have the system of congruences $x\equiv a_1\pmod{m_1}$ $x\equiv a_2\pmod{m_2}$ the system has a solution. In other words we can determine the congruence class of $x$ modulo $m_1m_2$.

I think we can all agree that the congruence $x\equiv 2\pmod{9}$ is easy to solve. But what about $7x\equiv 4\pmod{143}$ and $15x\equiv 23\pmod{135}$? You could check each value in $\mathbb{Z}_m$ for some modulo $m$ but that is incredibly inefficient. In fact one of the equations doesn't even have a solution. The Chinese Remainder Theorem (CRT) will make it much easier to solve and determine if a congruence has a solution or not.

Firstly, lets prove the $2$ moduli case. Since, $\gcd(m_1,m_2)=1$ by Bezout's there exist $n_1,n_2\in \mathbb{Z}$ such that $m_1n_1+m_2n_2=1$. Note that we can perform the euclidean algorithm and then substitute backwards to find those integers. A solution is $x =a_{1} m_{2} n_{2} + a_{2} m_{1} n_{1}.$ Rewording, $x=a_1(1-m_1n_1)+a_2m_1n_1 = a_1+(a_2-a_1)m_1n_1.$ This implies that $x\equiv a_1\pmod{m_1}$. The second congruence is proved by switching the subscripts 1 and 2, completing our proof by construction. Similarly, we prove the general case for $x\equiv a_1\pmod{m_1},\ldots, x\equiv a_k\pmod{m_k}$ where all moduli are coprime by iterating the process.

Lets evaluate an example we mentioned earlier. Consider $7x\equiv 4\pmod{143}$. For this equation to have solutions, $7x\equiv 4 \pmod{11}$ and $7x\equiv 4 \pmod{13}$ must have solutions. It isn't too hard to solve these and we see that $x\equiv 10 \pmod{11}$ and $x\equiv 8 \pmod{13}$. Letting $x=10+11k$ for $k\in \mathbb{Z}$ and substituting it into the other equation we get that $k\equiv 1\pmod{13}$ which implies that $k=1+13t$ for $t\in \mathbb{Z}$. Substituting, $x=10+11(1+13t)=21+143t$. Hence, $x\equiv 21\pmod{143}$. If the congruences didn't hold when we broke the modulo into its prime factors there would be no solution. Similarly, we can solve many other congruences by breaking the modulo into its prime factors and checking if the equation still holds.



<div class="day-nav-wrapper">
  <a href="./day35.html" class="day-nav__link">Previous: #35</a>
  <a href="./day37.html" class="day-nav__link">Next: #37</a>
</div>


