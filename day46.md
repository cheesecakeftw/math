---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 46

## [Matrix](https://en.wikipedia.org/wiki/Matrix_(mathematics))

Definition: A matrix is a rectangular array of numbers (or other mathematical objects). Not the movie!

Before we define what a matrix is formally, let us understand what it is. Consider the map $f:\mathbb{R}^3\to \mathbb{R}^3$ to be some linear map. Notice how it isn't efficient to write down such a map for each point. We would have to say $f(x,y,z)=(2x + y - z,\; 3y + z,\; x - 4z)$. Here's where matrices come in. They are a much more efficient way of writing the map down.

Let $F^n$ be a finite dimensional vector space over a field $F$ and we have a linear map $f:F^n\to F^m$. Using the $n$ basis vectors $v_1=(1,0,\ldots,0),v_2=(0,1,\ldots,0),\ldots v_n=(0,0,\ldots,1)$ we are able to define the outputs of $F^n$. Similarly, by specifying each of the $m$ coordinates we are able to define the outputs of $F^m$. For example, the $i$-th entry where $1\leq i \leq n$ we have that $f(v_j)$ is $a_{i,j}$. This is much more convenient then writing $f(x_1, x_2, \ldots, x_n) = \left(\sum_{j=1}^n a_{1,j}x_j,\; \ldots,\; \sum_{j=1}^n a_{m,j}x_j\right)$. Then, we define $f$ to be the $m \times n$ matrix of numbers with $m$ rows and $n$ columns:

$$
\begin{bmatrix}
a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
\vdots  & \vdots  & \ddots & \vdots  \\
a_{m,1} & a_{m,2} & \cdots & a_{m,n}
\end{bmatrix}
$$

Now let us define the operations we can use on this $m \times n$ matrix. Let the $m \times n$ matrix be $X$ and let it represent the map $f:F^n\to F^m$ and let $Y$ be an $n\times k$ matrix on the map $g:F^k\to F^n$. Define the matrix $Z$ to be $f\circ g:F^k\to F^m$. Let $x_{i,j}$ be the entries in $X$, $y_{i,j}$ be the entries in $Y$ and $z_{i,j}$ be the entries in $Z$. Then $z_{i,a}$ is the $i$-th coordinate of $f(g(v_a))=f(y_{1,a},y_{2,a}\ldots y_{m,a})$. Then $z_{i,a}=x_{i,1}y_{2,a}+x_{i,2}y_{1,a}+\ldots x_{i,m}y_{m,a}$. Notice that this formula is really similar to the well known matrix multiplication formula. Hence, $XY=Z$ where $f\circ g$ (composition of matrices) is represented by the matrix $XY$.

Similarly, we extend this logic to general vector spaces $V,W$ with dimensions $n,m$ respectively, where we can have $V=F^n$ and $W=F^m$, allowing us to represent a linear map of $f$ from $V$ to $W$ as an $m\times n$ matrix. To put it simply, any linear map between vector spaces can be captured by a matrix, and changing the bases just changes how that matrix looks, without changing the map itself!



<div class="day-nav-wrapper">
  <a href="./day45.html" class="day-nav__link">Previous: #45</a>
  <a href="./day47.html" class="day-nav__link">Next: #47</a>
</div>


