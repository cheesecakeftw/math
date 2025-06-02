---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 2

## Heine Borel Theorem

Definition: A set $$ X \subseteq \mathbb{C} $$ is compact if and only if it is closed and bounded. It can also be called compact when every open cover of $$\displaystyle X$$ has a finite subcover.

Intuitively it is easy to see that each function will have a maximum in a closed interval. But how can we prove it? Firstly, we must prove the Heine Borel Theorem. We can prove this theorem by dividing the square into 4 subsquares and then attempt to show that at least one of the four subsquares must not be covered by any finite subcover. Repeating this process leads to a sequence of smaller squares whose intersection is approaching a single point, which ends up lying entirely inside some open set from the cover, giving a contradiction and proving the existence of a finite subcover. The converse of this theorem also holds true and is a fairly straightforward proof using construction.

This property ties back to topology where we define certain vector spaces as Heine–Borel, iff every closed and bounded subset in $$X$$ is compact. Also, notice that this theorem is very similar to the previously discussed $$\textbf{Bolzano–Weierstrass theorem}$$ with the only difference being that according to the Bolzano–Weierstrass theorem every closed, bounded set is sequentially compact in $$R^n$$ whereas according to the Heine–Borel theorem every closed, bounded set is compact in $$R^n$$. We can prove the Heine–Borel theorem using the Bolzano–Weierstrass theorem and vice versa. Here, a sequentially compact space means that for every sequence in the set $$X$$ there is a convergent subsequence converging to a point in $$X$$.

A really interesting property of this theorem is that if $$X \subseteq R$$ is a compact set and $$U$$ an open set containing $$X$$, and $$f : U \to R$$ is a continuous function, then $$f(X)$$ is also compact. Another extremely important corollary is the [Extreme Value Theorem](https://en.wikipedia.org/wiki/Extreme_value_theorem) which is widely used throughout mathematics. The theorem states that if $$X \subseteq R$$ be a nonempty compact set, and $$f : X \longrightarrow R$$ is a continuous function, then there exists some $$y \in X$$ such that, for all $$x \in X$$, $$f(x) \le f(y).$$ This theorem is again based on compact sets and can be proved using the property defined above using the upper bound of the function.

<div class="day-nav-wrapper">
  <a href="./day1.html" class="day-nav__link">Previous: #1</a>
  <a href="./day3.html" class="day-nav__link">Next: #3</a>
</div>
