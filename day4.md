---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 4

## [Derivative](https://en.wikipedia.org/wiki/Derivative)

Definition: We say that a function $$f: R \longrightarrow R$$ is differentiable at $$x_0$$ if $$\lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$ exists. 

Yes, these are those derivatives which would be trivial to all who know calculus. We can use a derivative to linearly approximate $$f(x+h)$$ for some $$f(x)$$ for some small $$c$$ and to find the rate of change at the instantaneous point $$x$$. This also relates to the fundamental theorem of calculus where we find k such that for $$x \approx c$$ we find $$ f(x) \approx f(c)+k(x-c)$$. If the limit in the definition exists everywhere in the function we say that $$f$$ is $$\textbf{differentiable}$$, which can be denoted by $$f'$$ and if f is differentiable at some $$x_0$$ we say that $$f$$ is differentiable at $$x_0$$, which can be denoted by $$f'(x_0)$$. We also write $$\frac{df}{dx}$$ sometimes.

There are some really interesting rules that two functions $$f$$ and $$g$$ and their derivatives follow:
- Product rule: $$(f*g)'=f'*g+f*g'$$
- Quotient rule: $$(f/g)'=(f'*g-f*g')/{g^2}$$
- $$(c*f)'=c*f'$$ and $$(f+g)'=f'+g'$$, where $$c$$ is a constant. These suggest homomorphism based properties in these functions, which we will explore in more depth later.
- Chain rule: $$(f \circ g)' = (f' \circ g) * g'$$
- Power rule: For some $$f(x)=x^n$$, we have that $$f(x)=n*x^{n-1}$$, which holds for every nonzero real number. This can be proved quite easily by using exponential properties. 


Derivatives also have some really cool properties. If $$f$$ is differentiable everywhere than it is a continuous function. However, the vice versa isn't true. For example, the absolute value function $$f(x) = \lvert x \rvert$$ is continuous at every point but it doesn't have a derivative at $$x=0$$. This can be proved using the limit derivation defined earlier of a derivative. Additionally, a differentiable function is critical to the complex plane because it establishes a property known as [holomorphism](https://en.wikipedia.org/wiki/Holomorphic_function), which we discuss further later. 

Side‑note for Power rule (defining $$ x^r$$ for all real $$r $$):
For $$ x > 0 $$, let $$ x^k = \sup \{ y > 0 : y^k < x \}, \,  x^{p/q} = (x^q)^p \quad \left( \frac{p}{q} \in Q \right), \, x^r = \sup \{ x^s : s \in Q,\, s < r \}.$$

<div class="day-nav-wrapper">
  <a href="./day3.html" class="day-nav__link">Previous: #3</a>
  <a href="./day5.html" class="day-nav__link">Next: #5</a>
</div>