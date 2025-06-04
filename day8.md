---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 8

## [Cauchy-Riemann Equations](https://en.wikipedia.org/wiki/Cauchy%E2%80%93Riemann_equations)

Definition: In order for $$f$$ to be diﬀerentiable in the complex plane, it is necessary that $$
\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \\
\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}.
$$ where $$u$$ and $$v$$ are respectively the real and imaginary parts of a complex valued function. These equations are known as the Cauchy Riemann Equations.

Now that we have talked about Real analysis for so many days, lets have a change of topic. Before I get into what these equations mean, lets talk about complex numbers. A complex number is any number that is written in the form of $$z=x+iy$$. When we extend this to complex functions, $$f(z)=f(x+iy)=u(x,y)+ iv(x,y)$$ where $$u$$ and $$v$$ are real differentiable functions and z is a single complex variable.

In order for $$f'(z_0)$$ to exist, the limit $$ \frac{\Delta w}{\Delta z} = \frac{f(z_0 + \Delta z) - f(z_0)}{\Delta z}$$, where $$ \Delta z = \Delta x + i \Delta y$$, and $$ \Delta w = f(z_0 + \Delta z) - f(z_0),$$ must be the same whether we take $$\Delta y = 0$$ (so $$\frac{\Delta w}{\Delta z} \to u_x + i v_x$$) or $$\Delta x = 0$$ (so $$\frac{\Delta w}{\Delta z} \to -i u_y + v_y$$). Equating $$u_x + i v_x = -i u_y + v_y$$ and matching real and imaginary parts gives $$ u_x = v_y, u_y = -v_x,$$, the Cauchy–Riemann equations. This is a gist of the complete proof, which is much longer.

Now, you might be wondering why do we need these equations in the first place? It is possible that:
- A complex function can be diﬀerentiable at a point, but not at any other point in a neighborhood, such as is the case for $$f(z) = \lvert z\rvert^2$$.
- There exist complex functions $$f(x+ iy) = u(x,y) + iv(x,y)$$ such that u and v have continuous partial derivatives of all orders, yet f is not diﬀerentiable, such as is the case for $$f(z)=\bar z$$.
- Continuity and diﬀerentiability of the real and imaginary parts do not imply diﬀerentiability of the function. Again, this is so for $$f(z) = \bar z$$.
All of these examples can be verified by using the limit definition of a derivative, which is not too hard. Hence, to make sure that a complex function is differentiable we use the Cauchy Riemann equations, which are easier to use than checking the derivative. 

Intuitively, we can figure out that $$f(z)=e^z$$ will be differentiable at every point, based on how the derivative acts in the real plane. But do they satisfy the Cauchy-Riemann Equations?
We have
$$
\frac{\partial u}{\partial x} = e^x \cos y, \quad \frac{\partial u}{\partial y} = -e^x \sin y,
$$
$$
\frac{\partial v}{\partial x} = e^x \sin y, \quad \frac{\partial v}{\partial y} = e^x \cos y.
$$ Hence, the Cauchy-Riemann equations are satisfied, supporting our intuition, so $$e^z$$ is differentiable everywhere. Try to use the equations on the cases above to show that they hold when $$f(z)$$ won't be differentiable! Understanding how differentiation works in the complex plane is crucial and allows us to understand one of the most used classes of functions ([holomorphic functions](https://en.wikipedia.org/wiki/Holomorphic_function)) in complex analysis.










<div class="day-nav-wrapper">
  <a href="./day7.html" class="day-nav__link">Previous: #7</a>
  <a href="./day9.html" class="day-nav__link">Next: #9</a>
</div>