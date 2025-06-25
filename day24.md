---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 24

## [Identity Element](https://en.wikipedia.org/wiki/Identity_element)

Definition: An element $e$ in a set $S$ is called the identity element if $e \ast s=s$ for all $s\in S$.

Today we discuss one of the most trivial seeming theorems that is absolutely crucial to mathematics. To be precise, an element is called the identity element iff  $e * s=s * e=s$ for all $s\in S$. Note that based on the order a right identity and a left identity could exist. Additionally, only one unique identity element can exist in a set. IF $a$ and $b$ are identity elements then, $a=a*b=b$.

You are probably familiar with the multiplicative identity which is the number 1 because multiplying any number by one gives that number back. Similarly, the additive identity is 0: $a+0=a$. Like everything we discussed in the last 2 days sometimes this identity works out and sometimes it doesn't. For example, over a subset of some set of real numbers, the union and the intersection have an identity element: $$X \cup \emptyset$$ and $$X \cap X =X$$. The [identity matrix](https://en.wikipedia.org/wiki/Identity_matrix) is the identity element for matrix multiplication. For the functions on a set $$f :X \to X$$ there exists an [identity function](https://en.wikipedia.org/wiki/Identity_function), denoted by id such that $$f \circ id=f$$. One of the most useful identity elements are for the maximum and minimum function for a set of extended real numbers which are $-\infty$ and $\infty$ respectively: $$\max(-\infty, x)=x$$ for all $x$ in $X$. This is again used extremely frequently in programming by using the max/min values of *datatypes*. If we aren't using the extended real numbers set then the situation varies and there might not be an identity element for the set.

Note that there also exist sets where no identity elements exist. Consider the cross product of vectors, where there is no identity element because the direction of any nonzero cross product will always be orthogonal to any element multiplied. Also, consider the semigroup of positive natural numbers which wont have an identity element because we need 0, but it isn't a natural number.

Now we define an important term that we will use quite often. A set that demonstrates the associative binary operation and an identity element is called a [monoid](https://en.wikipedia.org/wiki/Monoid). For example, nonnegative integers form a monoid, where the identity element is 0. Note that monoids are a branch of semigroups and are used in various branches of mathematics. Additionally, similar to something we discussed earlier, commutative monoids also exist. As expected their operations are commutative!



<div class="day-nav-wrapper">
  <a href="./day23.html" class="day-nav__link">Previous: #23</a>
  <a href="./day25.html" class="day-nav__link">Next: #25</a>
</div>