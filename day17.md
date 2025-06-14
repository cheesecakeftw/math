---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 17

## [Analytic Continuation](https://en.wikipedia.org/wiki/Analytic_continuation)

Definition: Suppose $f$ is an analytic function defined on a non-empty open subset $U$ of the complex plane $\mathbb{C}$. If $V$ is a larger open subset of $\mathbb{C}$ containing $U$, and $g$ is an analytic function defined on $V$ such that $$g(z) = f(z) \quad \forall z \in U,$$ then $g$ is called an analytic continuation of $f$.

Today, we go over a topic we need to know to understand branch points and branch cuts which we will go over next. In simple terms analytic continuation means $$g$$ is the unique extension of f to $$V$$: the only holomorphic function on $$V$$ that agrees with $$f$$ on $$U$$. Let us suppose $f$ is holomorphic near $z_0$ and not zero, then its power series is $f(z)=a_0+a_1(z-z_0)+a_2(z-z_0)^2+...$, and clearly its order is $n$ where $n$ is the smallest integer such that $a_n \neq 0$. Then we write $f(z)=(z-z_0)^ng(z)$, where $g(z)$ is holomorphic in the neighborhood of $z_0$ and $g(z) \neq 0$. THen, there is some r such that $g(z)\neq 0$ when $\lvert z-z_0\rvert<r$. Thus, $f$ has no zeroes other than $z_0$ with $\lvert z-z_0\rvert<r$. It follows, that zeroes of holomorphic functions don't have limit points. 

Now suppose we have two holomorphic functions $$f$$ and $$g$$, on a connected open set $$U \subseteq C$$ and suppose that $f$ and $g$ agree on some set $S$ containing a limit point, such as a curve or tiny open set. Then $$f(z)=g(z)$$ for all $$z \in S$$, so $$f(z)-g(z)=0$$ for all $$z \in S$$. By the argument above, $f(z)-g(z)=0$ on $U$. Because $f-g$ is holomorphic and zero on a set $S$ with a limit point, the argument above shows that its zeros can't be isolated unless it's identically zero. This property is unique to holomorphic functions (Check out the smooth real function $g(z)$ which is $e^{\frac{-1}{x}}$ for $x>0$ and 0 for $x<0$). This behavior can be explained by the [Identity theorem](https://en.wikipedia.org/wiki/Identity_theorem).


Lets try out an example! Let $f : B_1(0) \to \mathbb{C}$ be defined by $$f(z) = \sum_{n=0}^{\infty} z^n,$$ and let $g : \mathbb{C} \setminus {1} \to \mathbb{C}$ be defined by $$g(z) = \frac{1}{1 - z}.$$ Now, note that $f(z)=g(z)$ for all $z \in B_1(0)$ and both are holomorphic functions, but $g$ is the one defined on a larger domain. Thus, $g$ is the analytic continuation of $f$ on $\mathbb{C} \setminus {1}$. Now consider the [Reimann zeta function](https://en.wikipedia.org/wiki/Riemann_zeta_function) (which converges for $Re(s)>1$) and the Dirichlet function $$\eta(s) = \sum_{n=1}^{\infty} \frac{(-1)^{n-1}}{n^s}$$(which converges for $Re(s)>0$). We can relate, them to get $$\zeta(s) = \frac{1}{1 - 2^{1 - s}} \eta(s)$$. This allows us to extend $\zeta(s)$ to $Re(s)>0$, except with the pole at $s=1$. In fact, $\zeta(s)$ can be continued analytically to $\mathbb{C} \setminus {1}$, where it has a simple pole at $s = 1$, using $$
\zeta(s) = \frac{s}{s - 1} - \sum_{n=1}^{\infty} \left( \zeta(s + n) - 1 \right) \frac{s(s + 1)(s + 2) \cdots (s + n - 1)}{(n + 1)!}$$. It might also be possible that we can't extend $f$ on $U$ at all to a holomorphic function on $V$. An example, is $f(z)=\frac{1}{z}$ on $$\mathbb{C} \setminus {0}$$ which won't extend to a holomorphic $C$, because there is a pole at 0. It can still be the case that we can extend $f$ to a point on $V$, but not to all of $V$ simultaneously. Try to figure out such a case (Hint: involves [branch-cuts](https://en.wikipedia.org/wiki/Branch_point))!






<div class="day-nav-wrapper">
  <a href="./day16.html" class="day-nav__link">Previous: #16</a>
  <a href="./day18.html" class="day-nav__link">Next: #18</a>
</div>