---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 3

## Limits in functions and sequences

Definition: Let $$f(x)$$ be a function of real numbers. We say that $$L$$ is the limit of the sequence if, for any $$\varepsilon > 0$$ and $$\delta>0$$, there is some $$\lvert x - c\rvert < \delta$$, then $$\lvert f(x) - L\rvert < \varepsilon$$. When this happens, we write $$\lim_{x \to c} f(x)=L$$. 

After all of that complicated math, lets take a step back and discuss what are limits! Yes, limits are intuitive to you if you know calculus. But there's more. Let's say I want to the value of the function $$f(x)=\frac{x^2-4}{x-2}$$ at $$x=2$$. Most likely your first instinct would be to evaluate $$f(2)$$. But here $$f(2)=\frac{0}{0}$$ which is undefined. However, the function is just $$(x+2)$$ everywhere else after cancelling out, which allows us to say that $$f(x)$$ approaches 4 as $$x$$ approaches 2.

This definition above is known as the epsilon-delta definition of a limit and is used in formal mathematics. The definition means that we can make $$f(x)$$ arbitrarily close to L, if $$x$$ is taken to be sufficiently close to $$c$$. For example, lets apply this definition to the question earlier which we found had a limit of 4. For any $$\varepsilon>0$$ we let $$\delta=\varepsilon$$, so that if $$\lvert x - 2\rvert < \delta$$, then $$\lvert f(x) - 4\rvert = \lvert x - 2\rvert  < \varepsilon$$. Hence, the definition held true! 

In the case that the limit exists for every $$x$$ and is equal to $$ f(x)$$ we call that function continuous. For example, $$f(x)=x$$ is continuous. A function can also be continuous at a point. Now lets address some cases where there is no limit and the definition wont hold true. When we choose a piecewise function such that for $$x<0$$, $$f(x)=1$$ and for $$x>=0$$, $$f(x)=2$$. Then the limit doesn't exist at 0 because if we pick $$\varepsilon=0.01$$ then for any $$\delta$$ and any $$L$$ we wont be able to get $$\lvert f(x) - L\rvert<0.01$$, because the function has a different limit from each side. Also, there are cases where the limit wont be $$f(c)$$ for $$x=c$$ because of a jump discontinuity. 

A really cool connection is that the epsilon-delta definition can be extended to sequences: Let $$x_1, x_2, \ldots$$ be a sequence of real numbers. We say that $$L$$ is the limit of the sequence if, for any $$\varepsilon > 0$$, there is some $$N > 0$$ so that, if $$n > N$$, then $$\lvert x_n - L\rvert < \varepsilon$$. When this happens, we write $ $L = \lim_{n \to\infty} x_n$$. This can also be shown to hold true intuitively using examples.




<div class="day-nav-wrapper">
  <a href="./day2.html" class="day-nav__link">Previous: #2</a>
  <a href="./day4.html" class="day-nav__link">Next: #4</a>
</div>