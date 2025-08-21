---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 41

## [Pythagorean Triples](https://en.wikipedia.org/wiki/Pythagorean_triple)

Definition: A pythagorean triple consists of three positive integers $x,y,z$ such that $x^2+y^2=z^2$.

We are all aware of the pythagorean triple $(a,b,c)=(3,4,5)$ from physics. Maybe you can compute triplets such as $ (28, 45, 53) $ or $(120, 209, 241)$ too. But what if we had to find a formula that could generate all possible pythagorean triplets. It turns out a formula that can do that does exist (and is a cool trick)!

Let there be $a,b,c$ such that $a^2+b^2=c^2$. Factoring out $d=\gcd(a,b,c)$, we get coprime $x,y,z$ such that  $x^2+y^2=z^2$. Since, all of $x,y,z$ are coprime, $x$ and $y$ must be coprime too. So atleast one of $x$,$y$ is odd. Note that $y$ must be even because if it were odd $z$ would be $0$ modulo $4$, but $a^2+b^2$ would be $2$ modulo $4$, since odd squares are $1$ modulo $4$. Then, $z^2-x^2=(z-x)(z+x)=y^2$. Rearranging, $(x+z)/y=y/(z-x)$. Since both sides are rational we let $(x+z)/y=m/n$, in its lowest terms. Because its the reciprocal, $(z-x)/y=n/m$. Then $\frac{z}{y} +\frac{x}{y} =\frac{m}{n}$ and $\frac{z}{y}-\frac{x}{y}=\frac{n}{m}$. Solving, $\frac{z}{y}=\frac{m^2+n^2}{2mn}$ and $\frac{x}{y}=\frac{m^2-n^2}{2mn}$. 

Now, notice that since $m$,$n$ are reduced $\gcd(m,n)=1$. Also notice that if they were both odd, the numerator in $\frac{m^2-n^2}{2mn}$ would be $0$ modulo $4$ and the denominator would be $2$ at the least, contradicting our assumption that $x$ is odd. Hence, one of $m,n$ is even and one is odd. Hence, the numerators are odd and denominators even. Notice that $m,n$ cant divide the numerator hence the fractions are irreducible. Equating we get that $x=m^2-n^2$, $y=2mn$ and $z=m^2+n^2$ where $m,n$ have different parities. Then, substituting, $a=dx$, $b=dy$, $c=dz$ we get Euler's formula for all possible pythagorean triples!

Additionally, this might seem familiar to another famous theorem: [Fermat's Last Theorem](https://en.wikipedia.org/wiki/Fermat%27s_Last_Theorem). The theorem says that for any positive integers $x,y,z$ and $n>2$ there exist no integer solutions to $x^n+y^n=z^n$. We will NOT be proving the theorem because the [proof](https://www.mat.uniroma2.it/~eal/Wiles-Fermat.pdf) is way too long (109 pages)!



<div class="day-nav-wrapper">
  <a href="./day40.html" class="day-nav__link">Previous: #40</a>
  <a href="./day42.html" class="day-nav__link">Next: #42</a>
</div>


