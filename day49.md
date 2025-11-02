---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 49

## [Field Extension](https://en.wikipedia.org/wiki/Field_extension)

Definition: A field extension is a pair of fields $$ K \subseteq L$$ such that the operations of $$K$$ are those of $$L$$ restricted to $$K$$.

Today we start something pretty new: [Galois Theory](https://en.wikipedia.org/wiki/Galois_theory)! Before we get into what a field extension really is, let us define a few terms. An algebraic number is any complex number $c$ such that if $f(c)=0$ for some polynomial $f\in \mathbb{Q}[x]$. Note that any algebraic number is the root of infinitely many polynomials, and that we call the unique monic polynomial of the lowest degree with $c$ as a root the minimal polynomial. To prove it consider two such polynomials $f$ and $g$. Then $f-g$ would have a lower degree, giving us a contradiction. Additionally, the minimal polynomial is always irreducible: if $f=pq$, and $c$ is a root of either then one must be a constant. For example, the minimal polynomial of $\sqrt{2}$ is $x^2-2$.

So, now we can define a field $\mathbb{Q}(a)$ as the set of all $f(a)$ for all polynomials $f\in\mathbb{Q}[x]$ for some algebraic number $a$. Intuitively is isn't too hard to see that those numbers must be algebraic too. But, why? For example, if $a=\sqrt[3]{3}$, what polynomial has $b=1+\sqrt[3]{3}+\sqrt[3]{9}$ as a root? Firstly, we calculate $b^2=7+5\sqrt[3]{3}+3\sqrt[3]{9}$ and that $b^3=31+21\sqrt[3]{3}+18\sqrt[3]{9}$. Now, expressing powers of $b$ in terms of $1,\sqrt[3]{3},\sqrt[3]{9}$, we solve for $xb^3+yb^2+zb+c=0$. Solving we get $2b^3-3b^2-27b-14=0$. Notice that the constant $\sqrt[3]{9}$ and $\sqrt[3]{3}$ terms don't interact with each other when adding: Hence, they form an independent basis over $\mathbb{Q}$. Basically, the field $\mathbb{Q}(\sqrt[3]{3})$ can be treated as three dimensional vector space over $\mathbb{Q}$ with basis $1,\sqrt[3]{3},\sqrt[3]{9}$.

So basically, $\mathbb{Q}(a)$ is an n-dimensional vector space over $\mathbb{Q} $ where: if the minimal polynomial of an algebraic number $a$ has degree $n$, we say that $a$ has degree $n$ too. The basis are $1,a,\ldots,a^{n-1}$. So, if $b\in \mathbb{Q}(a)$, then $1,b,\ldots,b^n$ are linearly dependent, because any $n+1$ elements in an $n$ dimensional space have to be linearly dependent.

Now we formally define field extensions: For a field $L$ with subfield $$ K \subseteq L$$, there is a field extension $L/K$. Don't confuse this with a quotient ring! If $L$ is finite dimensional over $K$, then $L/K$ is a finite dimensional. Note that we denote the degree of the extension where the larger field $L$ is a $K$ vector space as $[L:K]$. Here, $[\mathbb{Q}(a):\mathbb{Q}]$ is the degree of $a$. Additionally, if we consider two finite dimension extensions $M/L$ with degree $n$ and $L/F$ as an $m$ dimensional vector space, then $M$ is also a vector space over $F$, such that the dimension is $mn$. This means $[M:F]=[M:L][L:F]$. For any $b\in \mathbb{Q}(a)$ we have that the degree of $b$ divides the degree of $a$. Try to denote it in the degree notation to see why!
<div class="day-nav-wrapper">
  <a href="./day48.html" class="day-nav__link">Previous: #48</a>
  <a href="./day50.html" class="day-nav__link">Next: #50</a>
</div>
