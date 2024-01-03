---
layout: post
category: math
title: "quadratic patterns: 1, 3, 6, 10, 15, …"
description: a sequence I stumbled upon while observing the pascal's triangle.
date: '2023-03-31 00:00:00 +0000'
---

i stumbled upon this sequence while observing the pascal’s triangle,

I became curious, how would you solve for a_n on this sequence?

1, 3, 6, 10, 15…

Give it a try if you’d like or you can just immediately click to see its solution

.

# TL:DR

Listing the terms....

$$
a_1 = 1

\\ a_2 = 1+2

\\ a_3 = 1+2+3

\\ a_n = 1+...+n

$$

We represent the terms in the pattern from 1 to n with $$b$$

$$
b_1 = 1
\\ d = 1
$$

Using the arithmetic sequence formula,

$$
b_n = a_1+(n-1)d
\\ b_n = 1+(n-1)1
\\ b_n = n
$$

So the value of $$a_n$$ can be represented by the sum of the $$b_n$$ terms.

$$
a_n = \dfrac{n}{2}(1+n)
\\ a_n = \dfrac{n^2+n}{2}
$$

# Dumb me overcomplicating it.

We can start by understanding the common difference.

| m   | n | 1st difference  | 2nd difference |
| --- |---| --------------- | ---------------|
| 1   | 1 |  1  |  1 |
| 2   | 3 |  2 | 1 |
| 3   | 6 | 3 | 1|
| 4   | 10 | 4 | 1 |
| 5   | 15 | 5 | 1|

As you can see the numbers increase from the first difference. However that first difference also increases because there is the second difference. The second difference here remains as constant (sweet).

You will recognize that this is basically a quadratic sequence. Although there are available resources, I wanted to challenge myself.

I start by listing the terms,

$$
a_1 = 1

\\ a_2 = 1+2

\\ a_3 = 1+2+3

\\ a_4 = 1+2+3+4

$$

Notice that the numbers appear to be a sum of its consecutive numbers following the value of n. 
I decided to focus on $$a_2$$ first.

So the value of $$a_{n+1}$$ can be expressed in

$$
= \dfrac{n}{2}(2+n+1)
\\ = \dfrac{n}{2}(n+3)
$$

with n starting by 1.
(yeah i know it doesnt make sense LOL)

Back to the pattern, let’s try with what we have so far.

$$
a_2 = 1+[\dfrac{n}{2}(n+3)]

\\ a_2 = 1+\dfrac{1}{2}(4) = 3

\\ a_3 = 1+\dfrac{3}{6} = 1+\dfrac{1}{2}
$$

Yep that is wrong.

What went wrong? Well, we have to make $$n = n-1$$ in this case because we need to decrease n by 1 for the sum of n+1 pattern inside the formula. 

For example, if I’m working on $$a_n = 3$$, our original expression would get the sum of first 3 when we actually need the sum of the first 2.

Thus the final formula is

$$
a_n = 1 + \dfrac{n-1}{2}(n-1+3)

\\ a_n = 1+[\dfrac{n-1}{2}(n+2)

$$

Simplifying it even further becomes

$$
a_n = \dfrac{n^2+n}{2}
$$

As you can see this is not the right way to problem-solve things. Rather than solving it immediately for all values, I worked out the problem in an inefficient manner although I ended up with the right answer.