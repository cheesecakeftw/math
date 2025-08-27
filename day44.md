---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 44

## [Linear Subspaces](https://en.wikipedia.org/wiki/Linear_subspace) (and [Linear Independence](https://en.wikipedia.org/wiki/Linear_independence))

Definition:  Linear subspaces are subsets of vector spaces, that are vector spaces themselves.

Before we discuss Linear independence, let's formally define linear subspaces. A linear subspace of a vector space $V$ over a field $F$ is a subset $W$ of $V$ such that $u+v\in W$ and $cu\in W$ for every $u,v\in W$, and every $c\in F$, making $W$ a vector subspace. 

One way of forming a subspace is to consider a set of linear combinations of a set $S$ of vectors. For example, we consider the sum $c_1v_1+c_2v_2+\ldots c_kv_k$ where $v_1,\ldots \in S$ and $c_1,\ldots \in F$ which forms a linear subspace defined as the span of $S$. The image $f(V)$ of a linear map $f:V\to W$ is always a subspace, since linear maps preserve addition and multiplication. Similarly, we define the [span](https://en.wikipedia.org/wiki/Linear_span) of a set as all the linear combinations of those vectors which is the smallest subspace that could possibly contain $S$. It can also be said that its an intersection of all linear subspaces containing $S$.

We say that a set of vectors is linearly independent if none is in the span of the others. A set is linearly independent if and only if the only way to represent a $0$ vector is to have $c_i=0$ for all $i$. Similarly, a sequence of vectors can also be dependent. This is when there exists some $c_1,c_2,\ldots$ that are not all $0$ such that $\sum_{i=0}^{n}c_iv_i=0$, where 0 is the 0 vector in $V$. Now consider the example $v_1=(2,4)$ and $v_2=(1,2)$. Since, $a(2,4)+b(1,2)=0$ has solutions $a=1,b=-2$, this set of vectors is linearly dependent. On the other hand, consider $u=(1,0)$ and $v=(0,1)$. If $$a(1,0)+b(0,1)=0,$$  then $a=0$ and $b=0$ are the only solutions. Hence, this set is linearly independent.


Linear independence can be extended to infinity too! An infinite set of vectors is said to be linearly independent if every subset is linearly independent too. This definition supports the fact that subsets of a linearly independent set are independent too. We define an infinite set that is linearly dependent similarly.


<div class="day-nav-wrapper">
  <a href="./day43.html" class="day-nav__link">Previous: #43</a>
  <a href="./day45.html" class="day-nav__link">Next: #45</a>
</div>


