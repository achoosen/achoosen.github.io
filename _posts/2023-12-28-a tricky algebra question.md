---
layout: post
title:  "optimizing a trigonometric equation"
date: 2023-12-29 00:00 +0700
category: math
description: why am i doing a lot of trigonometry nowadays?
---
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

# The problem

A little of background. This problem appeared in *Universitas Indonesia*'s 2015 entrance test for 
'Mathematics for Natural Sciences'. This was Question 7.

Let $$\theta$$ be an angle such that

$$
\tan 4\theta=\dfrac{\cos\theta-\sin\theta}{\cos\theta+\sin\theta}
$$

Suppose $$\theta=x$$ (note x is in degrees) for some positive real number x, the smallest possible value of x is...

(A) 5
\\
(B) 9
\\
(C) 12.5
\\
(D) 14
\\
(E) 45
# My solution

The smallest possible value of x means we probably can just derive them, set it equal to 0, to find the minimum value.

$$
\tan 4x=\dfrac{\cos x-\sin x}{\cos x + \sin x}

\\ \dfrac{d}{dx}(\tan 4x=\dfrac{\cos x-\sin x}{\cos x + \sin x})

$$

LHS first.

$$
4\sec^2(4x)=0
\\ 4(\dfrac{1}{\cos^2 4x})=0
$$

So left hand side gives no solution.

We focus on the RHS now.

$$
\dfrac{d}{dx}(\dfrac{\cos x-\sin x}{\cos x + \sin x})
$$

Quotient rule states that $$f'(x)=\dfrac{u'v-uv'}{v^2}$$.

Let $$u=\cos x-\sin x$$ and $$v=\cos x + \sin x$$

$$
u' = -\sin x - \cos x
\\ v' = -\sin x + \cos x
$$

Applying quotient rule...


$$
f'(x)=\dfrac{(-\sin x - \cos x)(\cos x + \sin x)-(\cos x-\sin x)(-\sin x + \cos x)}{(\cos x + \sin x)^2}

\\ = \dfrac{-\sin^2 x - 2 \cos x \sin x - \sin^2 x - (\cos^2 x - 2 \sin x \cos x + \sin^2 x)}{(\cos x + \sin x)^2}

\\ = \dfrac{-2 \sin^2 x - 2 \cos^2 x}{(\cos x + \sin x)^2}
$$

Setting f'(x) = 0.

$$
0 = \dfrac{-2 \sin^2 x - 2 \cos^2 x}{(\cos x + \sin x)^2}

\\ 0 = -2 \sin^2 x - 2 \cos^2 x

\\ \sin^2 x = \cos^2 x

$$

Hmm I wonder what value of x that has both its sine and cosine equal?

Ez. 45 degrees.

$$
\sin 45= \dfrac{\sqrt{2}}{2}
\\ \cos 45 = \dfrac{\sqrt{2}}{2}
$$

Hence answer is E. You can actually verify this in the calculator too but remember that the exam doesn't allow you to have a calculator lol.



