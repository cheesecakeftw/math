---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 39

## [Euler's Criterion](https://en.wikipedia.org/wiki/Euler's_criterion)

Definition: For an odd prime $p$ and coprime integer $a$, $a^{\frac{p-1}{2}}$ is $1\pmod{p}$ if there exists an integer such that $x^2\equiv a\pmod{p}$, or $a^{\frac{p-1}{2}}$ is $-1\pmod{p}$ if there exists no such integer.

Before we dive into why this could possibly hold true, let us define a term: an integer $a$ is a [quadratic residue](https://en.wikipedia.org/wiki/Quadratic_residue) modulo $n$ if there exists an integer $x$ such that $x^2\equiv a\pmod{p}$. For example, $3^2\equiv 2\pmod{7}$ implies $2$ is a quadratic residue modulo $n$. Similarly, squaring $1,\ldots,6$ because those are the only integers modulo $7$ we get that $1,2,4$ are quadratic residues. Here, it isn't too hard to see that the only residues will be found squaring $1,...(p-1)/2$ since $(p-x)^2\equiv x^2\pmod{p}$ by expanding the square. Also, from Lagrange's theorem we know that $x^2$ can have at most $2$ solutions for each $a$. This implies that there are atleast $(p-1)/2$ distinct quadratic residues. So, for any integer $p$ there are exactly $(p-1)/2$ distinct quadratic residues modulo $p$.

Let us prove the existence of the criterion now. By FLT, $a^{p-1}\equiv \pmod{p}$. Then, $(a^{\frac{p-1}{2}}-1)(a^{\frac{p-1}{2}}+1)\equiv 0\pmod{p}$. Since, the domain is integral, one of the factors must be $0$. Now, if $a$ is a quadratic residue $a^{\frac{p-1}{2}}\equiv (x^2)^{\frac{p-1}{2}}\equiv x^{p-1}\equiv 1$. So, every quadratic residue makes the first factor $0$. Applying Lagrange's, there can't be more than $(p-1)/2$ values of $a$ that make the first factor 0. But, since theres only that many distinct residues, the other $(p-1)/2$ residue classes have to be nonresidues making the other factor $0$. This completes the proof of Euler's Criterion.

We represent Euler's Criterion using the [Legendre Symbol](https://en.wikipedia.org/wiki/Legendre_symbol): $\left(\tfrac{a}{p}\right)$. Your first thought might be that that's a fraction. But NO! The notation just happens to be defined like that but isn't a fraction (Thank Legendre for that). The symbol is $1$ if $a$ is a quadratic residue modulo $p$, $-1$ if $a$ is quadratic nonresidue modulo $p$ and $0$ if $p$ divides $a$. By definition, $\left(\tfrac{a}{p}\right)\equiv a^{\frac{p-1}{2}}\pmod{p}$ by Euler's Criterion. The most important property of this symbol has to be quadratic reciprocity: For odd primes $p$ and $q$ $\left( \tfrac{q}{p} \right)\left( \tfrac{p}{q} \right) = (-1)^{\tfrac{p-1}{2}\,\tfrac{q-1}{2}}$. We won't be proving this theorem here because it is too long. There are many other properties that this symbol follows other than this too such as: $\left(\tfrac{a}{p}\right)\equiv \left(\tfrac{a\pmod{p}}{p}\right)$. These properties make evaluating the symbol for any $a,p$ very efficient!





<div class="day-nav-wrapper">
  <a href="./day38.html" class="day-nav__link">Previous: #38</a>
  <a href="./day40.html" class="day-nav__link">Next: #40</a>
</div>


