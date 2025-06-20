---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 22

## [Commutative Property](https://en.wikipedia.org/wiki/Commutative_property)

Definition: A set S is commutative if $$x \,\ast \, y = y \,\ast\, x$$ for all $x,y \in S$ where $\ast$ represents a binary operation.

After many days of analysis, today we switch to ring theory. We start with commutativity, a topic that is honestly quite obvious and is something that we have been taught in elementary math. Today we discuss how does this property extend to higher math!

Much of the commonly discussed operations are commutative: this includes addition and multiplication of numbers (most number systems), addition of matrices and vectors, union and intersection and even the "and" and "or" [logical operators](https://en.wikipedia.org/wiki/Logical_connective) that we use in coding. Note, that this property looks incredibly similar to another property: [associativity](https://en.wikipedia.org/wiki/Associative_property) which states: $$(x \ast y) \ast z = x \ast (y \ast z), \quad \forall x, y, z \in S$$

The proof of this property is quite rigorous and long so we won't be addressing it today, but isn't too hard to show using [induction](https://en.wikipedia.org/wiki/Mathematical_induction). While commutativity feels natural, in higher math it's actually rare: in fact, most interesting structures like matrix groups or quantum operators aren't commutative at all! Hence, a single operator might be commutative in some spaces but not for others!

However, we must also look at the cases where operations aren't commutative. Intuitively, we can see that subtraction and division are noncommutative operations through simple cases such as $0-1 \neq 1-0$ and $1/2 \neq 2/1$. Additionally functional composition isn't commutative either. Consider the functions $f(x)=2x$ and $g(x)=2x+1$. Note that $f(g(x))=4x+2$ and $g(f(x))=4x+1$, which shows that $f(g(x))\neq g(f(x))$. One counterintuitive example is that matrix multiplication of square matrices is a noncommutative operation (with the exception of 1x1 matrices obviously). For instance, $$\begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} 0 & 2 \\ 0 & 1 \end{bmatrix} $$ whereas $$\begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 0 & 1 \end{bmatrix}= \begin{bmatrix} 0 & 1 \\ 0 & 1 \end{bmatrix}$$ which are completely different results. Another intuitive example is exponentiation where $2^3 \neq 3^2$. Finally, the multiplication of [quaternions](https://en.wikipedia.org/wiki/Quaternion), which we use heavily in physics, isn't commutative either: $ij = k \ne ji = -k$.


<div class="day-nav-wrapper">
  <a href="./day21.html" class="day-nav__link">Previous: #21</a>
  <a href="./day23.html" class="day-nav__link">Next: #23</a>
</div>