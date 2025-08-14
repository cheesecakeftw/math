---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 33

## [Unique Prime Factorization](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic)

Definition: Any integer $n>1$ is either a prime or can be represented as a product of primes.

We have seen earlier that the ring $\mathbb{Z}[\sqrt{-5}]$ doesn't have UPF whereas based on our daily observations it isn't too unreasonable to conclude that $\mathbb{Z}$ does. But why? Why is it better to assume that $1$ isn't a prime? THe reason for all this is the Fundamental Theorem of Arithmetic or UPF which tells us that every integer more than $1$ can be represented uniquely as a product of prime numbers. If $1$ were a prime consider $4=2\ast 2=2\ast 2\ast 1$, which contradicts FTA. 

Before, we prove FTA let us prove [Euclid's lemma](https://en.wikipedia.org/wiki/Euclid%27s_lemma) which states that if a prime $p$ divides $ab$ where $a,b\in \mathbb{Z}$, $p\mid a$ or $p\mid b$. For arbitrary $a,b\in \mathbb{Z}$ where $p\mid ab$ with $\gcd(p,b)=1$ by Bezout's identity there exist $x,y\in \mathbb{Z}$ such that $px+by=1$.Multiplying by $a$, $apx+aby=a$. Since,  $p\mid ab \implies pk=ab$ for $k\in \mathbb{Z}$ we have $apx+pky=a$. Since, $p(ax+ky)=a$, $p\mid a$. Similarly, if $\gcd(p,a)=1$, $p\mid b$, completing the proof.

Now we prove that every integer greater than 1 is either a prime or a product of primes. The base case holds true for $n=2$ since $2$ is a prime. Then, for $n>2$ assume that by strong induction, this holds true for all numbers greater than $1$ and less than $n$. Now there are 2 cases. If $n$ is prime we are done. Otherwise there exist $x,y\in \mathbb{Z}$ such that $n=xy$ with $1<x\leq y <n$. By the induction hypothesis $a,b$ are products of primes such that $a=p_1p_2\ldots p_j$ and $b=q_1q_2\ldots q_m$. Then, $n=p_1p_2\ldots p_jq_1q_2\ldots q_m$ which is a product of primes completing the proof.

Finally, we prove that every integer $n>1$ has a unique prime factorization. Assume that there exists some integer $d$ which has two distinct prime factorizations. Consider the set $S$ of integers $>1$ which have two distinct prime factorizations. Since, $d\in S$, let $n$ be the least element in $S$ by WOP. Then, $n=p_1p_2\ldots p_j= q_1q_2\ldots q_m$, where each $p_i,q_i$ are primes. Since, $p_1$ divides $q_1q_2\ldots q_m$, $p_1$ must divide some $q_i$ by euclid's lemma. Since, $p_1$ and $q_i$ are both primes it isn't hard to see that $p_1=q_i$. Cancelling these two factors from the factorizations we get $p_2\ldots p_j= q_1q_2\ldots q_{m-1}$ where WLOG $q_1q_2\ldots q_{m-1}$ are primes. But, these products are two distinct prime factorization of some integer smaller than $n$, contradicting the minimality of $n$. Hence, every integer greater than $1$ has a unique prime factorization.

Note that any integral domain where every nonzero non unit element can be written as a product of irreducible elements is called a [Unique Factorization Domain](https://en.wikipedia.org/wiki/Unique_factorization_domain)! [Irreducible elements](https://en.wikipedia.org/wiki/Irreducible_element) are elements that can't be products of two non-unit elements. Units are elements $u,v\in R$ s.t. $uv=1$ for some ring $R$. Hence, $\mathbb{Z}$ is a UFD because $1$ is a unit in $\mathbb{Z}$ whereas  $\mathbb{Z}[\sqrt{-5}]$  isn't a UFD.  Can you come up with more examples of UFDs?









<div class="day-nav-wrapper">
  <a href="./day32.html" class="day-nav__link">Previous: #32</a>
  <a href="./day34.html" class="day-nav__link">Next: #34</a>
</div>