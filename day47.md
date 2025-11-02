---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 47

## [Dual Space](https://en.wikipedia.org/wiki/Dual_space)

Definition: The dual space of a vector space $$V$$ over a field $$F$$ is the set of all linear maps from $$V$$ to $$F$$. These maps are called linear functionals. The dual space is denoted by $$V^*$$.

To understand what this means, let us go over an example. Take a vector in $$\mathbb{R}^2$$, say $$(3, -5)$$. This can be written as a $$2\times1$$ column matrix:
$$
\begin{bmatrix}
3 \\
-5
\end{bmatrix}
$$
or as a $$1\times2$$ row matrix $$[3\ -5]$$.  

The column vector can be thought of as a map $$f:\mathbb{R}^2\to\mathbb{R}$$ defined by $$f(x,y)=3x-5y$$. The row vector can be seen as a map $$g:\mathbb{R}\to\mathbb{R}^2$$ defined by $$g(t)=t(3,-5)$$. So, while one map takes a vector and gives a number, the other takes a number and gives a vector. Both represent the same thing, but are viewed in opposite directions.

Now let $$V$$ and $$W$$ be finite dimensional vector spaces over a field $$F$$. The set of all linear maps from $$V$$ to $$W$$ is denoted as $$\operatorname{Hom}(V,W)$$. This set is itself a vector space, because we can add and scale maps such that $(f+g)(v)=f(v)+g(v)$ and $(cf)(v)=c*f(v)$. In particular, $$\operatorname{Hom}(F,V)$$ corresponds to all column matrices, and is naturally [isomorphic](https://en.wikipedia.org/wiki/Isomorphism) to $$V$$. Each vector $$v\in V$$ can be identified with a map that sends $$c\in F$$ to $$cv$$.

Next, consider $$\operatorname{Hom}(V,F)$$, which consists of all linear maps from $$V$$ to the field $$F$$. This is what we call the dual space of $$V$$, denoted as $$V^*$$. Each element of $$V^*$$ is a functional that takes a vector and returns a scalar. Note that $V$ is also isomorphic to $$V^*$$. If $$V$$ has basis vectors $$v_1,v_2,\ldots,v_n$$, then the dual space has a corresponding dual basis $$v_1^*,v_2^*,\ldots,v_n^*$$, where $$v_i^*(v_j)=\delta_{ij}$$. Any functional in $$V^*$$ can be denoted as $$c_1v_1^*+c_2v_2^*+\ldots+c_nv_n^*$$, similar to how a vector in $$V$$ is denoted as a combination of $$v_1,v_2,\ldots,v_n$$. If we chose a different basis of $v$, then we get a completely different isomorphism.

Finally, we can take the dual of the dual space, denoted by $$V^{**}$$. Each vector $$v\in V$$ defines a map $$\Phi(v):V^*\to F$$ by $$\Phi(v)(\varphi)=\varphi(v)$$. This gives the map $$\Phi:V\to V^{**}$$. When $$V$$ is finite dimensional, and this map is an isomorphism, meaning $$V$$ and $$V^{**}$$ can be found. Hence, surprisingly, taking the dual space twice brings us back to the original vector space!



<div class="day-nav-wrapper">
  <a href="./day46.html" class="day-nav__link">Previous: #46</a>
  <a href="./day48.html" class="day-nav__link">Next: #48</a>
</div>
