---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 12

## [Contour Integration](https://en.wikipedia.org/wiki/Contour_integration)

Definition: For an open set $$U\subset\mathbb{C}$$, a contour $$\Gamma\subset U$$ with smooth parametrization $$\gamma:[a,b]\to\Gamma$$, and a function $$f:U\to\mathbb{C}$$, the contour integral of $$f$$ along $$\Gamma$$ is defined by $$\int_\Gamma f(z)\,dz = \int_a^b f\bigl(\gamma(t)\bigr)\,\gamma'(t)\,dt$$ and is called a contour integral.

Today we discuss one of the most important topics in complex analysis that allows us to do things we can't with just basic calculus. Before we get into what contour integration is, lets quickly define [integration](https://en.wikipedia.org/wiki/Integral) in $$R$$. Firstly, for $$f:[a,b] \to R$$, subdivide the interval $$[a,b]$$ into many subintervals. let $$x_0=a$$ and $$x_n=b$$ and let $$P=[[x_0,x_1],\ldots,[x_n-1,x_n]]$$. For each interval $$[x_{k-1},x_k]$$, let $$x_k ^{*}$$ be a point in the interval. Then we define the [Reimann sum](https://en.wikipedia.org/wiki/Riemann_sum) as $$R_P(f) = \sum_{k=1}^{n} f(x_k^{*})(x_k-x_{k-1})$$. For a partition $$P$$, let $\lvert P\rvert =\max \[ x_k-x_{k-1} \]$. Then we define the integral $$\int_{a}^{b}f(x)dx$$ to be the limit $$\int_{a}^{b}f(x)dx = \lim_{\lvert P \rvert \to 0} R_P(f)$$. This is fairly standard definition of integrals that most people who take calculus are familiar with. A really important consequence of integration that is fairly intuitive is the [ML inequality](https://en.wikipedia.org/wiki/Estimation_lemma) which says that if $$f$$ is integrable and has a maximum M on $$[a,b]$$, then $$\int_{a}^{b}f(x)dx \leq M(b-a)$$. This basically means that the integral is bounded by the maximum of the function times the length of the interval.
'
But what if the function we want to integrate is defined on $$C$$. Intuitively, it seems 2 sided, so should it be a double integral? It turns out that we don't usually do that. Instead we integrate over curves in $$C$$. Here, a parameterized curve is a continuous function $\gamma :[0,1] \to C$. We usually write $$\Gamma$$ for an image of $$\gamma$$. An important note is that non-differentiable curves can be extremely bad. An example where we can't define an integral would be the [Dragon curve](https://en.wikipedia.org/wiki/Dragon_curve) which goes through every point in $$C$$. For now lets avoid those and try to define the complex integral by Reimann sums. To do this we take points $t_k^* \in [t_{k-1},t_k]$ in a partition like we defined before, getting $$R_P(f) = \sum_{k=1}^{n} f(\gamma(t_k^{*}))_1(\gamma(t_k-x_{t-1})_1)$$ for $dx$. Here, $\gamma(t_k^{*})_1$ represents the x-coordinate, similarly we can do one for the y-coordinate or $dy$ instead too. 

Using the Reimann sum definition introduced above we can prove important properties such as $$\int_\Gamma \left( f(z) + g(z) \right) dz = \int_\Gamma f(z) dz + \int_\Gamma g(z) dz$$ and $$\int_{\Gamma_1 + \Gamma_2} f(z)\, dz = \int_{\Gamma_1} f(z)\, dz + \int_{\Gamma_2} f(z)\, dz$$ and If $\tilde{\gamma}(t) = \gamma(1 - t)$ (i.e. $\tilde{\gamma}$ traverses the same path, but backward), then $$ \int_{\tilde{\Gamma}} f(z)\, dz = - \int_{\Gamma} f(z)\, dz$$. You can also break down $$\Gamma$$ into $$ \gamma_1 +\ldots \gamma_2 $$ similarly.You may also be wondering if the ML-inequlity extends to the complex plane. It doe and is very important in complex analysis! If $\gamma$ has length $L$ and $\lvert f(z) \rvert \leq M$, then $$\left\lvert \int_{\Gamma} f(z)\, dz \right\rvert \leq \int_{\Gamma} \lvert f(z) \rvert\, \lvert dz \rvert \leq ML.$$ While we won't go into examples of contour integration today, a simple problem worth trying is integrating $$z^n$$ along the circle $$\Gamma :\lvert z\rvert =1$$, parameterized by $\gamma(t)=e^{2\pi i t}$!

Finally, lets see how does the anti-derivative factor into all of this. Let $U \subseteq \mathbb{C}$ be an open set, and let $f : U \to \mathbb{C}$ be a continuous function. An antiderivative of $f$ is a holomorphic function $F : U \to \mathbb{C}$ such that $F'(z) = f(z)$ for all $z \in U$. This gives us a really important theorem: If $f$ has an antiderivative $F$ on $U$, then for any differentiable curve $\gamma : U \to \mathbb{C}$ with $\gamma(0) = z_1$ and $\gamma(1) = z_2$, we have
$$
\int_{\Gamma} f(z)\, dz = F(z_2) - F(z_1).
$$
By definition, $\int_{\Gamma} f(z)\, dz = \int_0^1 f(\gamma(t)) \gamma'(t)\, dt$. Since $F$ is an anti-derivative of $f$, this equals $\int_0^1 \frac{d}{dt} F(\gamma(t))\, dt = F(\gamma(1)) - F(\gamma(0)) = F(z_2) - F(z_1)$.$\square$ This has the consequence that if $$f$$ has an anti-derivative then the integral of $$f$$ along a closed contour is 0. Another consequence is that the integral only depends on the endpoints. We will later extend on these consequences which will give us one of the most important theorems in complex analysis! Also, note that not all functions have anti-derivatives. Try to show why $$f(z)=\log z$$ doesn't have an anti-derivative in $$C$$, but does in $$R$$.




<div class="day-nav-wrapper">
  <a href="./day11.html" class="day-nav__link">Previous: #11</a>
  <a href="./day13.html" class="day-nav__link">Next: #13</a>
</div>