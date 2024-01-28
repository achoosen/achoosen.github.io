---
title: Derivation of the perpetuity formula
date: '2024-01-08'
layout: post
description: real life application of an infinite geometric series
---

So earlier, I was reading "The Cartoon Introduction to Economics Volume One: Microeconomics" and stumbled upon the formulas for the present value of annuity and the present value of perpetuity. The author noted in the comic strip that the formula of PV of perpetuity can be obtained by letting the PV of annuity formula sum to infinity. I became curious and wanted to try it out.

In the cartoon, the present value of annuity is defined by the formula,

$$

PV = x(\dfrac{1 - \dfrac{1}{(1+r)^n}}{r})

$$

where *r* represents interest rate, *n* represents time, and *x* represents future payments.

While the formula of PV of perpetuity is defined as $$PV= \dfrac{x}{r}$$.

So how do we get from annuity to perpetuity?

# The solution
All we have to do is rearrange the equation of annuity so it'll look like the equation below...

$$

PV = \dfrac{x}{r}(1- \dfrac{1}{(1+r)^n})

$$

Recall that $$\lim_{x\to\infty} \dfrac{1}{x} = 0 $$. This is also true for $$ \lim_{n\to\infty} \dfrac{1}{x^n} = 0 $$ where x is a constant. 

Therefore $$\lim_{n\to\infty} \dfrac{1}{(1+r)^n} = 0$$.

$$
\lim_{n\to\infty} PV = \lim_{n\to\infty} \dfrac{x}{r}(1- 0) =\lim_{n\to\infty} \dfrac{x}{r}

$$

And there you go, that's how I would (personally) show that the formula of perpetuity formula is $$\dfrac{x}{r}$$.