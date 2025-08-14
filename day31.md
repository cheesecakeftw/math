---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 31

## [The Division Algorithm](https://en.wikipedia.org/wiki/Euclidean_division)

Definition: Given $a,b\in \mathbb{Z}$, with $b\neq 0$, there exist unique integers $q,r$ such that $a=bq+r$ and $0\leq r< \lvert b\rvert$.

Your first thought might be this seems awfully familiar to the [Euclidean Space excerpt](./day27.html). That intuition would be correct! But, this isn't a general statement and is specifically meant to show that $\mathbb{Z}$ is a euclidean space. This algorithm might seem intuitive, but has applications extended in a significant amount of number theory (even when you wouldn't expect it).

Let us prove the existence of the algorithm using what we discussed yesterday. Note, that first we consider the case $b>0$. Consider the set $S=${$a-bq: q\in \mathbb{Z} \text{ and } a-bq\geq 0$}. Now consider $q=-a$, then $x=a-b(-a)\geq 0$. Hence, $x\in S\implies $$S \neq \varnothing$. By WOP, let $r$ be the least element of $S$. We know that there exists $q$ such that $r=a-bq$ where $r\geq 0$ by the definition of $S$. For the sake of contradiction, let $b \leq r$. Then $r-b=a-b(q+1)\geq 0$. Hence, $r-b\in S$, but $r-b<r$, contradicting the minimality of $r$. Hence, $0\leq r<b$. Now, we consider the case where $b<0$. Writing, $\lvert b\rvert=-b$ and applying the same argument and flipping the sign of $q$ at the end we see that the argument still holds.

Finally, we prove the uniqueness of the integers $q,r$ such that $a=bq+r$. Assume $q,r$ aren't unique. Then there exist distinct $q',r'$ such that $a=bq'+r'$. Then, $0\leq r< \lvert b\rvert$ and $0\leq r'< \lvert b\rvert$. Subtracting both definitions of $a$, $b(q-q')=r-r'$. Then, $b$ must be a divisor of $r-r'$ which implies $\lvert r'-r\rvert<\lvert b\rvert$. Hence, $r'-r=0$ by our earlier inequalities which implies $b(q-q')=0$. Since, $b\neq 0$, and $\mathbb{Z}$ is an integral domain, $q-q'=0$. So we get that $q=q'$ and $r=r'$ which gives us a contradiction and implying $q,r$ are distinct. We are now done proving the algorithm!





<div class="day-nav-wrapper">
  <a href="./day30.html" class="day-nav__link">Previous: #30</a>
  <a href="./day32.html" class="day-nav__link">Next: #32</a>
</div>