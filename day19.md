---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 19

## [Branch Cut](https://en.wikipedia.org/wiki/Branch_point)

Definition: A branch cut is a curve in the complex plane such that it is possible to define a single analytic branch of a multi-valued function on the plane minus that curve.

We talked about what branch points are yesterday, but how exactly do we define a holomorphic square root function? We know that it can only be done on some domain that doesn't contain a loop around 0. We can choose a simple path from 0 to $\infty$ which is called a branch cut, and define the holomorphic square root function on the complement of the branch cut. A popular choice is the nonpositive real axis, but any path from 0 to $\infty$ does work, even if its a spiral or something complicated like that.

But, what happens when there are more branch points? Let us consider $f(z)=\sqrt{z^3-z}$. We have a branch point when $z^3-z=0$. Notice that when we take $\sqrt{z}$ at $z=0$, we run into the same problem that we discussed yesterday where it looks like $\sqrt{-z}$ making it a branch point. Notice that $\sqrt{z^3-z}=\sqrt{z}\sqrt{z-1}\sqrt{z+1}$. Now that we have extra branch points, can we define $f$ on the circle $\lvert z-1/2 \rvert=3/4$ which circles $z=0$ and $z=1$, but not $z=-1$? On the circle $\sqrt{z+1}$ is a well defined because we aren't circling -1. Now the other parts of $f$ have a branch point in the circle which gets multiplied by -1. But, these contributions cancel out so we can define a holomorphic $f$ as we circle around two of the branch points, not just around one. If we want to define it on a maximal domain of $C$, we need to connect the branch points and connect the third one to $\infty$ via a path not intersecting the other path. We can then define a holomorphic $f$ on the complement of this branch cut.

What about other such complicated types of branch cuts? What about $$f(z) = \sqrt[3]{z^3 - z}$$? We can't define this $f$ on a region that circles one or two branch points. But we can define it on a region that circles the three of them. A typical domain is $$\mathbb{C} \setminus [-1, 1]$$. But, note that there is a difference between functions like $\sqrt{z}$ and $\sqrt{z^2-1}$. $\sqrt{z^2-1}$ has a cut from -1 to 1 but $\sqrt{z}$ has a cut from 0 to $\infty$. Why exactly does it need to go to $\infty$? It turns out that $\infty$ is a branch point for only $\sqrt{z}$! To check if $\infty$ is a branch point of a function $f(z)$, we let $g(z) = \frac{1}{f(1/z)}$ and check if $0$ is a branch point of $g(z)$. For $\sqrt{z}$, this gives $g(z) = \sqrt{1/z} = \frac{1}{\sqrt{z}}$, which has a branch point at $0$, so $\infty$ is a branch point of $\sqrt{z}$. But for $\sqrt{z^2 - 1}$, $g(z) = \sqrt{1 - z^2}$ has no branch point at $0$, so $\infty$ is not a branch point of $\sqrt{z^2 - 1}$, which makes intuitive sense, because in a neighborhood of $\infty$, $\sqrt{z^2-1}$ looks very much like $z$.

Now lets consider another important function: the [logarithmic function](https://en.wikipedia.org/wiki/Logarithm). It has branch points at 0 and $\infty$. Let us check if 0 is a branch point. Let $$\varepsilon > 0$$ be arbitrary. Then, as in the definition of a branch point, let $$f_1(z)$$ be defined on a region containing $$U_1$$ such that $$f_1\left(\tfrac{\varepsilon}{2} e^{i\theta}\right) = \log \tfrac{\varepsilon}{2} + i\theta$$ for $$0 \leq \theta \leq \pi$$, and let $$f_2(z)$$ be defined on a region containing $$U_2$$ by $$f_2\left(\tfrac{\varepsilon}{2} e^{i\theta}\right) = \log \tfrac{\varepsilon}{2} + i\theta$$ for $$-\pi \leq \theta \leq 0$$. Then we have $$f_1\left(-\tfrac{\varepsilon}{2}\right) = \log \tfrac{\varepsilon}{2} + i\pi$$, whereas $$f_2\left(-\tfrac{\varepsilon}{2}\right) = \log \tfrac{\varepsilon}{2} - i\pi$$. One can similarly check that $$\infty$$ is a branch point. To check that every other point in $C$ isn't a branch point, find a [power series](https://en.wikipedia.org/wiki/Power_series) expansion for $\log z$ in the neighborhood of any nonzero point $z_0$. THis is enough because, it implies that $\log z$ is a analytic in a neighborhood of $z_0$. We can define the power series using elementary calculus.



<div class="day-nav-wrapper">
  <a href="./day18.html" class="day-nav__link">Previous: #18</a>
  <a href="./day20.html" class="day-nav__link">Next: #20</a>
</div>