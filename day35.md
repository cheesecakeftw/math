---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 35

## [Fermat's Little Theorem](https://en.wikipedia.org/wiki/Fermat%27s_little_theorem)

Definition: For any integer $a$ and a prime $p$ such that $\gcd(a,p)=1$ we have $a^{p-1}=1\pmod{p}$.

This is one of the most well known theorems in number theory that we have probably come across even if we aren't aware of the proof. It is widely used in olympiad mathematics and is really cool looking. Note that this theorem's generalization which we prove below gives us the [order](https://en.wikipedia.org/wiki/Order_(group_theory)) of the cyclic group $U_n$ with a primitive root as $\phi(n)$.

Before we discuss the proof of the theorem we prove the [cancellation property](https://en.wikipedia.org/wiki/Cancellation_property) of congruences. Consider $au\equiv bu \pmod{p}$ with $\gcd(u,p)=1$ where $a,b\in \mathbb{Z}$. We can rewrite the congruence as $p\mid u(a-b)$. Since $\gcd(u,p)=1$, by euclid's lemma: $p\mid a-b \implies a\equiv b \pmod{p}$.

Now we prove Fermat's little theorem. Consider the set $S=${$1,2,\cdots,p-1$} which represents the residues modulo $p$ where $p$ is a prime. Consider $a\in \mathbb{Z}$ such that $\gcd(a,p)=1$. Then, the set $T=$ {$a,2a,\cdots,(p-1)a$} is also a set of residues modulo $p$ since each integer is coprime. Let us prove that these are distinct residues. Assume for the sake of contradiction $ax_i\equiv ax_j\pmod{p}$ where $x\in S$ and $i\neq j$. By the cancellation property then $x_i\equiv x_j\pmod{p}$ when clearly all elements in $S$ are distinct giving us a contradiction. Hence, each $r\in T$ is a set of distinct residues modulo $p$ which means that $T$ is a permutation of $S$. Hence, $a^{p-1}(p-1)!\equiv (p-1)!\pmod{p}$. Since $\gcd((p-1)!,p)=1$, by the cancellation property, $a^{p-1}\equiv 1\pmod{p}$, completing the proof.

A stronger result this theorem, [Euler's Theorem](https://en.wikipedia.org/wiki/Euler%27s_theorem), which says that if $\gcd(a,n)=1$, then $a^{\phi(n)}\equiv\pmod{1}$. Consider the unit group $U_n$ which has $\phi(n)$ elements and multiply all the elements by an arbitrary $u\in U_n$ since $a$ is just some $u$ in $U_n$. The proof follows from above after this and shouldn't be too hard to complete!


<div class="day-nav-wrapper">
  <a href="./day34.html" class="day-nav__link">Previous: #34</a>
  <a href="./day36.html" class="day-nav__link">Next: #36</a>
</div>


