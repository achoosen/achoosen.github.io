---
layout: post
category: math
title: "infinite area of isosceles triangle in a circle = area of a circle"
description: an investigation problem i encountered in my math textbook
date: '2023-10-02 00:00:00 +0000'
---
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

*This was written when I was still using WordPress*

First of all, this was overdue in a longg time. I have written this last year and left it on drafts and never ended up bothering to write the mathematical equations although the idea is there.

Suppose we have a circle with point O as origin and radius r within the circle are n congruent isosceles triangles.

Know that the formula for an area of isosceles triangle is

$$
A = \dfrac{1}{2}ab\sin(c)
$$

where a and b represent the sides. In this case, r for radius, will represent the two sides of the isosceles triangle and $$\theta$$ represents the angle between those two sides..

In this case, we can arrange the formula as,

$$
A = \dfrac{1}{2}r*r\sin(\theta)
\\ A = \dfrac{1}{2}r^2\sin(\theta)

$$

Multiplying with $$n$$ amount of isosceles triangle we have, we get

$$
\\ An = \dfrac{n}{2}r^2\sin(\theta)

$$

A full circle is known to be represented in 360 degrees or in radians, $$2\pi$$. Because we are using $$n$$ which represents a number that we don’t know. However what we do know is that it will allow us to converge to a whole, one circle. Therefore by intuition, the value of $$\theta$$ is $$\dfrac{2\pi}{n}$$ because we want to know the angle (radians) for 1 isosceles triangle within $$n$$ amount of isosceles triangles.

Since it is a circle we can let

$$
\lim_{x\to\infty}\dfrac{n}{2}r^2\sin(\dfrac{2\pi}{n})

$$

Simplifying further the expression by cancelling out n and 2. We end up with,

$$
\lim_{x\to\infty}\pi*r^2
$$

The limit of a constant as it approaches an infinity is always the constant itself. And hence we see that the area of a circle is our favorite $$\pi$$ and its radius squared through the use of infinite amount of isosceles triangles.