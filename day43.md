---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 43

## [Vector Spaces](https://en.wikipedia.org/wiki/Linear_algebra#Vector_spaces)

Definition: A vector space is a set of objects called vectors that you can add together and multiply by numbers (scalars), and the results are still vectors in the same set (Formally defined later).

Now that we have talked about structures such as fields, groups and rings, today we introduce a new algebraic structure which captures the structure of vectors. This structure is a vector space. Before we define the vector spaces formally, consider the well known dimensional space $\mathbb{R}^2$. Elements of the 2 dimensional space $\mathbb{R}^2$ are represented as pairs of real numbers: $(a,b)$. An element for any $n$ dimensional space is an $n$ tuple. Specifically, we can add elements: $(1,2)+(3,5)=(4,7)$. We can also scale an element: $2*(2,3)=(4,6)$. Addition and scalar multiplication of elements are operations that will be defined in a vector space.

Now let us define vector spaces. Consider a field $F$. Let $V$ be an abelian group of under addition which also allows the scalar multiplication operator, such that we can multiply an element of $F$ and $V$, to get another element of $V$. Note that elements of $F$ are called scalars, and elements of $V$ are called vectors. Then we say that an abelian group $V$ is a vector space over $F$ for $a,b\in F$ and $u,v\in V$ if:
- Distributivity of scalar multiplication: $a(u+v)=au+av$ and $(a+b)v=av+bv$.
- Associativity of scalar multiplication: $a(bv)=(ab)v$
- Identity element ($1\in F$) for scalar multiplication: $1v=v$

Using vector spaces we define another important idea: [Linear maps](https://en.wikipedia.org/wiki/Linear_map).Let $V,W$ be vector spaces over a field $F$. Then, we say that $f:V\to W$ is a linear map if $f(u+v)=f(u)+f(V)$ and $f(uv)=uf(v)$. A bijective linear map (each element in $V$ maps to exactly one element in $W$ and vice versa) is an [isomorphism](https://en.wikipedia.org/wiki/Isomorphism). Notice that this is really similar to homomorphisms in groups!


<div class="day-nav-wrapper">
  <a href="./day42.html" class="day-nav__link">Previous: #42</a>
  <a href="./day44.html" class="day-nav__link">Next: #44</a>
</div>


