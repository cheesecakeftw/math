---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 25

## [Inverse Element](https://en.wikipedia.org/wiki/Inverse_element)

Definition: Given a binary operation $\ast$ and an identity element $e$ if $x*y=e$ then $y$ is the inverse element and can be represented by $x^{-1}$.

Today we discuss a topic that we have learned in elementary school that extends all the way to higher mathematics. It is trivial to see that $$x + (-x)=0$$ and $$x$$ * $$(1/x)=1$$. Here, we call $$-x$$ the additive inverse and $$1/x$$ the multiplicative inverse. 

Similar to what we discussed yesterday certain elements may be the "left inverse" or the "right inverse" instead of being an inverse element: $x$ * $y$ = $y$ * $x$ = $e$. Now notice that similar to the identity element the inverse element is also unique. This can be proved by contradiction. For two inverses $x$ and $y$: $$x = x * e = x * (a * y) = (x * a) * y = e * y = y$$ which is only possible if $$y=x$$. Another trivial fact is that $$0$$ can't have a multiplicative inverse because we can't divide by 0. 

Let's extend that to how [groups](https://en.wikipedia.org/wiki/Group_(mathematics)) work. A group is a set with an associative operation that has an identity element, and every element has an inverse. Recall that a set with an associative operation is called a monoid. Hence, a monoid in which every element has an inverse is a group. Here the inverse $$f^{-1}$$ of a group element $$f$$ defines a transformation that undoes the transformation done by $$f$$: $$f^{-1}$$ is the inverse of $$f$$. One example of a group is the monoid of real numbers under addition which each have an inverse element. Also, note that contradictory to what you would expect none of the max, gcd, union functions have inverses. However, matrices do have inverses and are widely used in mathematics. Note, that groups are absolutely crucial to ring theory and mathematics in general!

For example, groups of functions, where $X$ is a set with [bijections](https://en.wikipedia.org/wiki/Bijection) $$X\to X$$ forms a group under function composition. Note, that a function has an inverse element iff it is a bijection. Also note that a function has a right inverse for function composition iff it is [injective](https://en.wikipedia.org/wiki/Injective) and a right inverse for function composition iff it is [surjective](https://en.wikipedia.org/wiki/Surjective). Finally, we introduce a new group: an abelian group. Under addition, a ring is an abelian group, which basically means that it is commutative and associative!



<div class="day-nav-wrapper">
  <a href="./day24.html" class="day-nav__link">Previous: #24</a>
  <a href="./day26.html" class="day-nav__link">Next: #26</a>
</div>