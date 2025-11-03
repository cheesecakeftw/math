---
layout: default
title: Math Every Day
description: A brief guide to Fun Higher Math
---
# Day 48

## [Dot Product](https://en.wikipedia.org/wiki/Dot_product)

Definition: The dot product is a function that takes two vectors of the same dimension and returns a single number.

In the previous section, we saw that a vector can act as a map that produces a scalar. The dot product elevates this idea to a pair of vectors! Let $$u=(u_1,u_2,\ldots,u_n)$$ and $$v=(v_1,v_2,\ldots,v_n)$$ be vectors in $$\mathbb{R}^n$$. Then the dot product is defined as $$u\cdot v=u_1v_1+u_2v_2+\ldots+u_nv_n.$$ For example, if $$u=(2,3)$$ and $$v=(4,-1)$$, then $$u\cdot v=2(4)+3(-1)=5.$$ Keep in mind that this function can be defined as $$\mathbb{R}^n \times \mathbb{R}^n\to \mathbb{R}^n$$. It distributes over addition, so $$(u+w)\cdot v=u\cdot v+w\cdot v,$$ and also $$v\cdot (u+w)=v\cdot u+v\cdot w,$$, showing that the dot product distributes over addition. Additionally, $$(cu)\cdot v=c(u\cdot v).$$  which shows that the dot product is linear and that it works out with scalar multiplication.

If $$V$$ is a vector space over a field $$F$$, any function $$f:V\times V\to F$$  is called a [bilinear form](https://en.wikipedia.org/wiki/Bilinear_form) on $V$ if it satisfies those two properties. For example, the dot products one of them! When such a form is evaluated at $$u,v\in V$$, we often denote it as $$\langle u,v\rangle.$$ here, $$\langle u,v\rangle.$$ may not be equal to $$\langle v,u\rangle.$$ 

Additionally, we can rewrite the dot product as a matrix product. Here, the row vector represents an element of the dual space $$V^*$$, while the column vector represents an element of $$V$$. The dot product can then be interpreted as applying a linear functional to a vector, just like we discussed for the dual space yesterday such that its a composition of linear maps $$\mathbb{R} \to \mathbb{R}^n$$ and $$\mathbb{R}^n \to \mathbb{R}$$. to give $$\mathbb{R} \to \mathbb{R}$$. But clearly $$\mathbb{R} \to \mathbb{R}^n$$ is pretty much a vector in $$\mathbb{R}^n$$. So, $$\operatorname{Hom}(\mathbb{R},\mathbb{R}^n)\equiv \mathbb{R}^n$$. So, if $$T:\mathbb{R}^n\to (\mathbb{R}^n)^{*}$$, is the isomorphism then $T(u_1,\ldots,u_n)=[u_1,\ldots,u_n],$ then $u\cdot v$ is $T(u)(v)$.

So basically given a linear map $$T:V\to V^*$$, we can define one of the bilinear form by $$\langle u,v\rangle=T(u)(v).$$ Similarly, a bilinear form determines such a map $$T:V\to V^*$$. Hence, the bilinear forms on $V$ match with the linear maps $$V\to V^*$$. The dot product is one such case where $$T$$ is the identity map!

<div class="day-nav-wrapper">
  <a href="./day47.html" class="day-nav__link">Previous: #47</a>
  <a href="./day49.html" class="day-nav__link">Next: #49</a>
</div>
