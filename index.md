---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---

Hi! This is the website for Math Every Day. This page will cover one theorem or mathematical idea every day. We will be addressing subjects from game theory all the way through analysis and number theory. Each entry offers a brief overview of the idea and, where relevant, goes over a problem or application.

This guide is NOT a comprehensive reference and is meant only as a quick and fun introduction. **Click the day or topic that you want to read about!**

## Days: 
### [1](./day1.html) [2](./day2.html) [3](./day3.html) [4](./day4.html) [5](./day5.html) [6](./day6.html) [7](./day7.html)
### [8](./day8.html) [9](./day9.html) [10](./day10.html) [11](./day11.html) [12](./day12.html) [13](./day13.html) [14](./day14.html)
### [15](./day15.html) [16](./day16.html) [17](./day17.html)  [18](./day18.html) [19](./day19.html) [20](./day20.html) [21](./day21.html)
### [22](./day22.html) [23](./day23.html) [24](./day24.html) [25](./day25.html) [26](./day26.html) [27](./day27.html) [28](./day28.html)
### [29](./day29.html) [30](./day30.html) [31](./day31.html) [32](./day32.html) [33](./day33.html) [34](./day34.html) [35](./day35.html)
### [36](./day36.html) [37](./day37.html) [38](./day38.html) [39](./day39.html) [40](./day40.html)


1 - 7: Real Analysis

8 - 21: Complex Analysis

22 - 28: Ring Theory

29 - 42: Number Theory




### [Day 1: Cauchy Sequences](./day1.html)

$$\forall \varepsilon > 0, \ \exists N \in \mathbb{N} \ \text{such that} \ \forall m,n > N, \ |x_m - x_n| < \varepsilon$$

### [Day 2: Heine Borel Theorem](./day2.html)

$$
\text{A set } X \subseteq \mathbb{R} \text{ is compact if and only if it is closed and bounded.}
$$

### [Day 3: Limits in functions and sequences](./day3.html)

$$\lim_{n \to \infty} f_n(x) = f(x)$$

### [Day 4: Derivative](./day4.html)

$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

### [Day 5: Uniform and Pointwise Convergence](./day5.html)

$$\forall \varepsilon > 0, \ \exists N \ \text{such that} \ \forall n > N, \ \forall x \in U, \ \lvert f_n(x) - f(x) \rvert < \varepsilon$$

### [Day 6: Mean Value Theorem](./day6.html)

$$\exists c \in (a,b) \ \text{such that} \ f'(c) = \frac{f(b)-f(a)}{b-a}$$

### [Day 7: Arzelà–Ascoli theorem](./day7.html)

$$(F \subset R(X),\ \text{bounded and equicontinuous}) \implies \exists \{f_{n_k}\} \to f \text{ uniformly}.$$

### [Day 8: Cauchy-Riemann Equations](./day8.html)

$$
\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \\
\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}.
$$

### [Day 9: Liouville's Theorem](./day9.html)

$$
\text{A bounded entire function } f : \mathbb{C} \to \mathbb{C} \text{ is constant.}
$$

### [Day 10: Taylor Series](./day10.html)

$$
f(z) = \sum_{n=0}^{\infty}
a_n(z - z_0)^n, \,\, \,\ a_n=\frac{f^{(n)}(z_0)}{n!}
$$

### [Day 11: Singularities](./day11.html)

$$
\varepsilon > 0,\ B_\varepsilon(z_0) \setminus \{z_0\} \subseteq U \implies z_0 \text{ is an isolated singularity.}
$$

### [Day 12: Contour Integration](./day12.html)

$$\int_\Gamma f(z)\,dz = \int_a^b f\bigl(\gamma(t)\bigr)\,\gamma'(t)\,dt$$

### [Day 13: The Cauchy Integral Theorem](./day13.html)

$$\int_\Gamma f(z)\,dz =0$$

### [Day 14: Cauchy Integral Formula](./day14.html)

$$f(z_0) = \frac{1}{2\pi i} \int_{\Gamma} \frac{f(z)}{z - z_0}\, dz$$

### [Day 15: Maximum Modulus Principle](./day15.html)

$$ \text{Holomorphic } f \text{ on connected open } U,\ \lvert f(z_0) \rvert \geq \lvert f(z) \rvert\ \forall z \in U \Rightarrow f \text{ constant.}$$ 

### [Day 16: The Residue Theorem](./day16.html)

$$ \int_{\Gamma} f(z)\,dz = 2\pi i \sum_{k=1}^{n} \operatorname{Res}(f; z_k)$$ 

### [Day 17: Analytic Continuation](./day17.html)

$$
f : U \to \mathbb{C}, \quad g : V \to \mathbb{C}, \quad U \subset V \subset \mathbb{C}, \quad f = g|_U \Rightarrow g \text{ is analytic continuation of } f
$$

### [Day 18: Branch Point](./day18.html)

$$
z_0 \in \mathbb{C} \text{ is a branch point } \Leftrightarrow f(z_0 + \varepsilon e^{2\pi i t}) \text{ not single-valued on } t \in [0,1]
$$

### [Day 19: Branch Cuts](./day19.html)

$$\text{curves removed to make a multivalued function single valued on the remaining domain.}$$

### [Day 20: Infinite Products](./day20.html)

$$\prod_{n=1}^{\infty} a_n=a_1a_2a_3\ldots$$

### [Day 21: Hadamard Factorization Theorem](./day21.html)

$$f(z) = e^{g(z)} z^m \prod_{n=1}^\infty \left(1 - \frac{z}{a_n}\right) e_{p_\kappa}\left(\frac{z}{a_n}\right)$$

### [Day 22: Commutative Property](./day22.html)

$$x \,\ast \, y = y \,\ast\, x \,, \quad \forall x,y \in S$$ 

### [Day 23: Associative Property](./day23.html)

$$(x \ast y) \ast z = x \ast (y \ast z), \quad \forall x, y, z \in S$$

### [Day 24: Identity Element](./day24.html)

$$s \ast 1=s, \quad \forall s \in S$$ 

### [Day 25: Inverse Element](./day25.html)

$$s \ast s^{-1} = 1, \quad \forall s \in S$$

### [Day 26: Distributive Property](./day26.html)

$$x\ast (y+z)=x\ast y + y\ast z,  \quad \forall x,y,z \in S$$

### [Day 27: Euclidean Domain](./day27.html)

$$
\forall\,a,b\in R\;,\exists\,q,r\in R\;\text{ s.t. }\;a=bq+r \text{ where }f(r)<f(b).
$$

### [Day 28: Ideal](./day28.html)

$$
I\subseteq R\ \text{is an ideal} \iff \forall\,a,b\in I,\ r\in R:\ a+b\in I,\ ra\in I.
$$

### [Day 29: Modular Arithmetic](./day29.html)

$$m\mid a-b \iff a \equiv b\pmod{m}$$

### [Day 30: Well Ordering Principle](./day30.html)

$$
S \subseteq \mathbb{N},\ S \neq \varnothing \ \Rightarrow\ \exists\,m \in S, \text{such that $m$ is the least element in $S$}
$$

### [Day 31: The Division Algorithm](./day31.html)

$$
a,b\in\mathbb{Z},\ b\ne0\ \Rightarrow\ \exists!\,q,r\in\mathbb{Z}\text{ such that } a=bq+r,\ 0\le r<|b|.
$$

### [Day 32: Bezout's Identity](./day32.html)

$$
a,b\in\mathbb{Z},\ \gcd(a,b)=d\ \Rightarrow\ \exists\,x,y\in\mathbb{Z} \text{ such that } ax+by=d.
$$

### [Day 33: Unique Prime Factorization](./day33.html)

$$
n>1\in\mathbb{Z}\ \Rightarrow\ n=p_1\cdots p_k,\text{ for primes } p_i.
$$

### [Day 34: Unit Group](./day34.html)

$$
U_n = \{\,a \in \mathbb{Z}_n \mid \gcd(a,n) = 1\,\}.
$$

### [Day 35: Fermat's Little Theorem](./day35.html)

$$
p\ \text{prime},\ a\in\mathbb{Z},\ \implies\ a^{p-1}\equiv 1 \pmod{p}.
$$

### [Day 36: Chinese Remainder Theorem](./day36.html)

$$
x \equiv a_1\pmod{m_1}, x \equiv a_2 \pmod{m_2},\ \gcd(m_1,m_2)=1 \ \implies \text{ there exists } x \pmod{m_1m_2}.
$$

### [Day 37: Wilson's Theorem](./day37.html)

$$
p\ \text{prime} \ \iff\ (p-1)! \equiv -1 \pmod{p}.
$$

### [Day 38: Lagrange's Theorem](./day38.html)

$$
f(x)\in\mathbb{Z}_p[x],\ \deg f = n\implies\ f \text{ has at most }n \text{ roots in } \mathbb{Z}_p.
$$

### [Day 39: Euler's Criterion](./day39.html)

$$
a^{\tfrac{p-1}{2}}\equiv\left(\tfrac{a}{p}\right)\pmod{p},\quad p\ \text{ odd prime },\ a\in\mathbb{Z}.
$$

### [Day 40: Fermat's Sandwich Theorem](./day40.html)

$$
y^2 = x^3 - 2 \ \implies\ (x,y) = (3,\pm 5).
$$