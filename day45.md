---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 45

## [Dimension (of a Vector Space)](https://en.wikipedia.org/wiki/Dimension_(vector_space))

Definition: The dimension of a vector space $V$ is said to be the size of the basis of $V$.

That is a lot of words that we haven't covered! Recall that before we defined the vector space $\mathbb{R}^2$ as $2$ dimensional and $\mathbb{R}^n$ as $n$ dimensional. But why? Let's consider the $\mathbb{R}^2$ case as an example again. Each possible vector $(x,y)$=$x(1,0)+y(0,1)$. Notice that each vector $(x,y)$ is a unique linear combination of $(1,0),(0,1)$. To put it precisely, vectors in $\mathbb{R}^2$ need $2$ parameters to be uniquely defined, which is why we call that space $2$ dimensional.

Before, we formally define the dimension of a vector space, we define a few other ideas. For any vector space $V$ over $F$ let $v_1,v_2,\ldots \in V$ be a set of vectors. We call that set the spanning set of $V$ when every $u\in V$ is a linear combination of $v_i$. If a spanning set is linearly independent, then we say that it is the basis of $V$. This means that every $u\in V$ is a unique combination of $v_i$. In $\mathbb{R}^2$, the vectors $(1,0),(0,1)$ form a basis, and are denoted by $e_1,e_2$.

Now, we specifically consider vector spaces that have a finite spanning set (even though the infinite case holds), defined as finite-dimensional spaces. Then we define the dimension of a finite-dimensional space $V$ over $F$ to be the cardinality  of the basis of $V$. Hence, the dimension of $\mathbb{R}^2$ is $2$ and $\mathbb{R}^n$ is $n$. Furthermore, while we won't prove it, it isn't too hard to see that each vector space $V$ must have a basis with the same size. Formally, this is called the dimension theorem for vector spaces. On the other hand noticing that every vector space $V$ must have a basis is not trivial at all!

Additionally, we have a few more interesting properties in finite-dimensional spaces. If $U$ is a subspace of $V$, then $\dim{U}\leq\dim{V}$. If $V$ is finite-dimensional, $\dim{U}=\dim{V}\implies U=V$. For subspaces $W_1,W_2$ of $V$, $\dim{W_1+W_2}=\dim{W_1}+\dim{W_2}-\dim{W_1\cap W_2}$, where $W_1+W_2$ is the span of $W_1\cup W_2$. For non finite-dimensional spaces such as $\mathbb{R}$ over $\mathbb{Q}$, they still have a basis, but things look very different and are surprisingly isomorphic. We will discuss why later!


<div class="day-nav-wrapper">
  <a href="./day44.html" class="day-nav__link">Previous: #44</a>
  <a href="./day46.html" class="day-nav__link">Next: #46</a>
</div>


