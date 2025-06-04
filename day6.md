---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 6

## [Mean Value Theorem](https://en.wikipedia.org/wiki/Mean_value_theorem)

Definition: Let $$f : [a,b] \to R$$ be a continuous function on the closed interval $$[a,b]$$, and differentiable on the open interval $$(a,b)$$, where $$a < b$$. Then there exists some $$c \in (a,b)$$ such that:
$$
f'(c) = \frac{f(b) - f(a)}{b - a}.
$$

As promised yesterday, where we discussed that the mean value theorem can be used to prove the [Weierstrass M-test](https://en.wikipedia.org/wiki/Weierstrass_M-test), we will now go over it. First, we will address a more specialized case of the Mean Value Theorem, that you will know if you know basic calculus, called [Rolle's theorem](https://en.wikipedia.org/wiki/Rolle%27s_theorem). Rolle's theorem assumes that $$f(a)=f(b)$$, which would result in some $$c$$ where $$f'(c)=0$$. This can be proved using the Extreme Value Theorem, which we talked about earlier. We notice that $$f'(c)=0$$ at a minimum or maximum of $$f(x)$$, and according to the Extreme Value theorem there has to be minimum and maximum in the interval $$[a,b]$$. But, what if $$a$$ or $$b$$ are where $$f(x)$$ attains the minimum and maximum. Then note that the function would be constant, and that $$c \in (a,b)$$, because the slope remains $$0$$ everywhere. Hence, we know that $$f(x)$$ will attain a maximum at $$x=c$$ for some $$c \in (a,b)$$. If $$f'(c) > 0$$, that is, $$\lim_{h \to 0} \frac{f(c+h) - f(c)}{h} > 0$$, there must exist some $$h > 0$$ such that $$c + h < b$$ and $$\frac{f(c+h) - f(c)}{h} > 0$$, that is, $$f(c+h) > f(c)$$. But $$f(c)$$ is the *maximum*, contradiction. Similarly, if $$f'(c) < 0$$, we also derive a contradiction.
$$\square$$        

To prove the Mean Value Theorem using Rolle's Theorem let $$g(x)=f(x)-\frac{f(b)-f(a)}{b-a}x$$. Since, $$g(a)=g(b)$$ (by construction), $$g'(c)=0$$ and also by differentiating $$g'(c)=f'(x)-\frac{f(b)-f(a)}{b-a}$$. Hence, by equating, $$f'(c)=\frac{f(b)-f(a)}{b-a}$$, which proves the Mean Value theorem. $$\square$$    

The Mean Value theorem also has some very nice implications:
- If the derivative of $$f$$ exists and is 0 at every point, then $$f$$ is constant on the interval.
- If $$f'(x) = g'(x)$$ for all $$x$$ in an interval $$(a,b)$$ of the domain of these functions, then $$f - g$$ is constant. This can be proved by defining $$h(x)=f(x)-g(x)$$ and then differentiating and using the Mean Value theorem.




<div class="day-nav-wrapper">
  <a href="./day5.html" class="day-nav__link">Previous: #5</a>
  <a href="./day7.html" class="day-nav__link">Next: #7</a>
</div>