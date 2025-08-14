---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 30

## [Well Ordering Principle ](https://en.wikipedia.org/wiki/Well-ordering_principle)

Definition: Every non-empty subset of non-negative integers $\mathbb{N}$ consists of a least element.

WOP is one of the most intuitively trivial things, but also one of the most useful (especially when we are building up from the basics). This theorem can be used to prove the existence of the division algorithm, the termination of the euclidean algorithm and is widely used in number theory, as we will see shortly. Note that we can prove induction using WOP and WOP using induction implying an equivalence relation.

First lets prove WOP using [induction](https://en.wikipedia.org/wiki/Mathematical_induction). Consider a nonempty subset $S$ of positive integers with no least element. $1 \notin S$ or else it would be the least element. Define the complementary set X: $1\in X$. Then suppose every integer $\leq n$ is in $X$. Then if $n+1$ is in $S$ it would be the least element since every smaller element is in $X$. Hence, $n+1\in X$. By strong induction it is easy to see that every element must lie in $T$. So, $S$ is an empty set, giving us a contradiction.

Now lets prove induction using WOP. Suppose $P$ is some function such that $P(1)$ is true and $P(n)$ being true implies $P(n+1)$ is true. Let $S$ be the set of $k$  s.t. $P(k)$ is false. Suppose $S$ is nonempty and by WOP let $d$ be the least element. Since, $P(1)$ is true, $1\notin S$, so $d\neq 1$, so $d-1$ is positive, and by minimality $d-1 \notin S$. So $P(d-1)$ is true, but but then by property of $P$, $P(d)$ is true. So $d\notin S$, giving us a contradiction. So $S$ is empty and $P(k)$ is true for all $k$.

Now, lets prove something so trivial one wouldn't even think of this: there is no integer between $0$ and $1$! We will use the [minimal criminal](https://en.wikipedia.org/wiki/Minimal_counterexample) method to prove this. Assume for the sake of contradiction there exists $n\in \mathbb{N}$ s.t. $0<n<1$. Consider the set of integers $S = ${$ k \in \mathbb{Z} \mid 0 < k < 1 $}. Since, $n\in S$, $S\neq \varnothing$. By WOP, we know there exists $x\in S$ which is the least element. Since $0<x<1$, and $x>0$ multiplying by $x$ gives $0<x^2<x$. If $x$ is an integer than $x^2$ is also an integer and by transitivity of inequalities $x^2\in S$ which contradicts the minimality of $x$. Hence, there is no integer between 0 and 1!

<div class="day-nav-wrapper">
  <a href="./day29.html" class="day-nav__link">Previous: #29</a>
  <a href="./day31.html" class="day-nav__link">Next: #31</a>
</div>