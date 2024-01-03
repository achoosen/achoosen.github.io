---
layout: post
title:  "a tricky algebra question"
date: 2023-12-28 00:00 +0700
category: math
description: trigonometry ahhhhhhhhhh
---

# The problem

If $$\sin \theta - \cos \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2}$$, $$0 \le \theta \le \dfrac{\pi}{2}$$, then the value of $$\sin^3 \theta - \cos^3 \theta =$$...

(A) $$\dfrac{1}{2}\sqrt{2}$$
\\
(B) $$\dfrac{1}{2}\sqrt{3}$$
\\
(C) $$\sqrt{2}$$
\\
(D) $$2$$
\\
(E) $$12$$

A little of background. This problem appeared in *Universitas Indonesia*'s 2015 entrance test for 
'Mathematics for Natural Sciences'. 

# My solution

A very useful identity for solving this problem is $$\sin^2 \theta+\cos^2 \theta = 1$$.

With the above identity, we at least can get an idea of what $$\sin^3 \theta - \cos^3 \theta$$ looks like for now.

$$
(\sin \theta - \cos \theta)(\sin^2 \theta+\cos^2 \theta) = (\dfrac{\sqrt{6}-\sqrt{2}}{2})(1)
\\ (\sin^3 \theta + \sin \theta \cos^2 \theta - \sin^2 \theta \cos \theta - \cos^3\theta) = \dfrac{\sqrt{6}-\sqrt{2}}{2}
$$

Simplifying further...

$$
\sin^3 \theta - \cos^3 \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2} + \sin \theta \cos \theta (\sin \theta - \cos \theta)

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2} + \sin \theta \cos \theta (\dfrac{\sqrt{6}-\sqrt{2}}{2})

$$

Great. Now we just need to find $$\sin \theta \cos\theta$$.

We recognize that

$$
(\sin \theta - \cos \theta)^2 = \sin^2\theta - 2\sin\theta\cos\theta + \cos^2\theta
$$

You see where I'm going?

$$
\sin^2\theta - 2\sin\theta\cos\theta + \cos^2\theta =(\dfrac{\sqrt{6}-\sqrt{2}}{2})^2

\\ \sin^2\theta - 2\sin\theta\cos\theta + \cos^2\theta = 2 - \sqrt{3}

\\ - 2\sin\theta\cos\theta + \sin^2\theta + \cos^2\theta = 2 - \sqrt{3}

\\ - 2\sin\theta\cos\theta + 1 = 2 - \sqrt{3}

\\ \sin\theta\cos\theta = \dfrac{\sqrt{3}-1}{2}
$$

dOpE. We go back to our known identity of $$\sin^3 \theta - \cos^3 \theta$$.

$$
\sin^3 \theta - \cos^3 \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2} + \sin \theta \cos \theta (\dfrac{\sqrt{6}-\sqrt{2}}{2})

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2} + (\dfrac{\sqrt{3}-1}{2}) (\dfrac{\sqrt{6}-\sqrt{2}}{2})

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2} + (\dfrac{\sqrt{6}}{2})(\dfrac{\sqrt{3}-1}{2}) - (\dfrac{\sqrt{2}}{2})(\dfrac{\sqrt{3}-1}{2})

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{\sqrt{6}-\sqrt{2}}{2} + \dfrac{\sqrt{18}}{4}-\dfrac{\sqrt{6}}{4} - \dfrac{\sqrt{6}}{4}+\dfrac{\sqrt{2}}{4}

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{2\sqrt{6}}{4}-\dfrac{2\sqrt{2}}{4} + \dfrac{\sqrt{18}}{4}-\dfrac{\sqrt{6}}{4} - \dfrac{\sqrt{6}}{4}+\dfrac{\sqrt{2}}{4}

\\ \sin^3 \theta - \cos^3 \theta = -\dfrac{\sqrt{2}}{4} + \dfrac{\sqrt{18}}{4}

\\ \sin^3 \theta - \cos^3 \theta = -\dfrac{\sqrt{2}}{4} + \dfrac{3\sqrt{2}}{4}

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{2\sqrt{2}}{4}

\\ \sin^3 \theta - \cos^3 \theta = \dfrac{1}{2}\sqrt{2}
$$

Hence answer is A. 

