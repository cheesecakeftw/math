---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 29

## [Modular Arithmetic](https://en.wikipedia.org/wiki/Modular_arithmetic)

Definition: For $a,b,m\in \mathbb{Z}, \quad$ $m\mid a-b \implies a \equiv b\pmod{m}$

Most of us are familiar with modular arithmetic whether you realize it or not. Notice that 1:00 and 13:00 are denoted as 1:00 on a 12-hour clock. This is because $13\equiv 1 \pmod{12}$. this is read as 13 is congruent to 1 modulo 12 which is the same as 12 divides 13-1. 

Before we get into modular arithmetic, let us see what [divisibility](https://en.wikipedia.org/wiki/Divisibility_(ring_theory)) actually means. Consider $a,b\in \mathbb{Z}$. We say that $a$ divides $b$ (denoted as $a\mid b$) if there exists $k\in \mathbb{Z}$ such that $a=bk$. For example, $2\mid 12$ and $12=2\ast 6$. This definition holds in any commutative ring. It is important to note that divisibility is transitive:
$a\mid b, \,b\mid c \implies a \mid c$. This is easy to prove by using the definition of divisibility. There are various other properties that we will reference in the future.

Coming back to modular arithmetic, let us go over what the [congruence relation](https://en.wikipedia.org/wiki/Congruence_relation) is! There are 3 properties that a congruence relation follows. You may notice that these are similar to equality. The properties are:
- Reflexivity: For $a\in \mathbb{Z},\quad$$a\equiv a \pmod{m}$.
- Symmetry: For $a,b\in \mathbb{Z},$ if $a\equiv b \pmod{m}$ then $b\equiv a \pmod{m}$.
- Transitivity:  For $a,b,c\in \mathbb{Z},$ if $a\equiv b \pmod{m}$ and $b\equiv c \pmod{m}$, then $a\equiv c \pmod{m}$.
A relation satisfying these properties is called an equivalence relation: Congruence and equality are equivalence relations.

Note that the congruence class modulo $m$ of an integer $a$ is the set of all integers that are congruent to $a$ modulo $m$. This allows us to split all integers into various congruence classes for some arbitrary mod $m$. The congruence class for integers congruent to $a$ modulo $m$ is defined as $[a]$ and contains all integers of form $a+mk$ for some $k\in \mathbb{Z}$. For example for $m=3$ we have $[5]=[2]$.

The set of all congruence classes modulo $m$ is called the ring of integers modulo $m$. This is denoted by $\mathbb{Z}/m\mathbb{Z}$ or $\mathbb{Z}_m$. For $m>0$, $\mathbb{Z}/m\mathbb{Z}=${$0,1,2,\ldots m-1$}. This set is also called the least residue system modulo $m$ and represents the least positive integer of each residue class mod $m$. Note that residue classes and congruence classes are the same thing! We can also multiply and add residue classes. This is verifiable by showing that if $a \equiv b \pmod{m}$ and $c \equiv d \pmod{m}$, then $a + c \equiv b + d \pmod{m}$, which isn't too hard to do using the definition of congruences!.



<div class="day-nav-wrapper">
  <a href="./day28.html" class="day-nav__link">Previous: #28</a>
  <a href="./day30.html" class="day-nav__link">Next: #30</a>
</div>