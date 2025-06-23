---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 23

## [Associative Property](https://en.wikipedia.org/wiki/Associative_property)

Definition: A set $$S$$ is associative if for all $$x,y,z \in S$$ any a binary operator *, $$(x\ast y)\ast z=x\ast (y\ast z)$$. The set $S$ can also be called a [semigroup](https://en.wikipedia.org/wiki/Semigroup).

Today we discuss a property that ties back really closely to what we discussed yesterday: commutativity. Yesterday, we saw that a property as simple as commutativity was really important in higher mathematics. Similarly, associativity a property that looks so trivial, turns out to be the roots of lots of higher mathematics. You may recognize this property because we learn a version of it in primary school based on multiplication: (x * y) * z = x * (y * z).

Now that we know that multiplication is associative, what about addition or composition? It turns out that addition is also associative, which isn't too hard too see. Additionally, the gcd and lcm functions also act associatively, i.e. $$\gcd(\gcd(x, y), z) = \gcd(x, \gcd(y, z)) = \gcd(x, y, z)$$. Similar to the commutative property the intersection and union of sets is again associative. To our surprise, the operation of function composition is associative! For some functions $$f,g,h$$ on one set or multiple sets $$(f \circ g) \circ h = f \circ (g \circ h) = f \circ g \circ h$$. Lets try out a quick example: Let $f(x)=2x$, $g(x)=x^2$, $h(x)=2x+1$. It is quite easy to compute and see that function composition is associative here. Contrary to the commutative property matrices are also associative, which is easy to conclude based on the properties of matrices. Additionally, even the maximum of numbers, often used in *competitive programming* is associative: i.e. $$\max(\max(x, y), z) = \max(x, \max(y, z))$$.

We won't go into the proof because this fact is again quite rigorous despite this being an intuitive property. Similar to the commutative property subtraction and division aren't associative either, but exponentiation which is commutative isn't associative. We can try a simple case to see it: $$2^{(1^2)} \ne (2^1)^2$$. One of the most important results of this property is that we can omit parenthesis, which makes the expression easier to use.

Note that in general associative operations aren't commutative. But there are exceptions: every continuous, associative operator on an interval of the real number line that is injective and strictly increasing in each argument is commutative. A really cool application of this property is the [telescoping series](https://en.wikipedia.org/wiki/Telescoping_series), where we use addition's associativity for cancelling terms in the infinite series!



<div class="day-nav-wrapper">
  <a href="./day22.html" class="day-nav__link">Previous: #22</a>
  <a href="./day24.html" class="day-nav__link">Next: #24</a>
</div>