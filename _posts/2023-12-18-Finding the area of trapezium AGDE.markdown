---
layout: post
title:  "Finding the area of trapezium AGDE"
date: 2023-12-18 16:16:27 +0700
category: math
description: A geometry question from SIMAK UI 2019, Universitas Indonesia's entrance exam.
---
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

## The problem

This was an entrance exam question for *Universitas Indonesia* in 2019. If you are interested, you may access the [page](https://bimbinganalumniui.com/edukasi/pelajaran/topik/590).

![the math problem](/assets/images/uigeometryproblem.png)

# in English
Given ABC are equilateral, BC = 2CD, line DEF is perpendicular to AB, and AG is parallel to AG, as shown in the diagram. If the area of BDF is $$\dfrac{81}{2}\sqrt{3}$$, the area of trapezium AGDE is...

## The solution
<details>
<summary>View answer</summary>
Let us understand the givens in the problem.

$$ AB = BC = AC = 2CD 
\\ BD = 3CD
\\ DF = AG 
$$

My attempt to attack this problem is to find the area of triangle AFE so we can subtract the whole area by the sum of area BFD and AFE. 

To accomplish this, for starters, we need to know the value of AF.

$$
AB = 2CD
\\ BF = 2CD - x
\\ AF = x
$$

We'll have to set up two equations to find this value of $$x$$. Notice that our BF and AF produces a right triangle with side AG. We can use the Phytagoras Theorem.

$$
(BD)^2 = (BF)^2 + (AG)^2
\\(3CD)^2 = (2CD-x)^2 + (AG)^2
$$

This can be simplified to,

$$
eq. 1: (AG)^2 = (3CD)^2 - (2CD - x)^2
$$

For the second equation,
$$
(AD)^2 = (AF)^2 + (AG)^2
$$

However we'll require the value of AD first.

Notice that the midpoint of BC which we will call Y. AY-YD-DA forms a right triangle. So it's simply just applying the Phytagoras Theorem to find the value of AD.

$$
AY = \sqrt{3}CD, YD = 2CD
\\ AD = \sqrt{3(CD)^2 + 4(CD)^2}
\\ AD = \sqrt{7}CD
$$

Now we can solve the second equation.

$$
(AD)^2 = (AF)^2 + (AG)^2
\\ (\sqrt{7}CD)^2 = x^2 + (AG)^2
\\ eq. 2: (AG)^2 = 7(CD)^2 - x^2
$$

Equating the two expressions of AG,

$$
(3CD)^2 - (2CD - x)^2 = 7(CD)^2 - x^2
\\ 9(CD)^2 - (4(CD)^2 - 4CDx + x^2) = 7(CD)^2 - x^2
\\ 9(CD)^2 - 4(CD)^2 + 4CDx - x^2 + x^2 - 7(CD)^2 = 0
\\ -2(CD)^2 + 4CDx = 0
\\ 4CDx = 2(CD)^2
\\ x = \dfrac{2(CD)^2}{4CD}
\\ x = \dfrac{1}{2}CD
\\ AF = \dfrac{1}{2}CD
$$

which means $$BF = \dfrac{3}{2}CD$$.

Then we can find AG using any of the Phytagoras equation we used earlier.

$$
(AG)^2 = 7(CD)^2 - (AF)^2
\\ (AG)^2 = 7(CD)^2 - (\dfrac{1}{2}CD)^2
\\ (AG)^2 = 7(CD)^2 - \dfrac{1}{4}(CD)^2
\\ (AG)^2 = \dfrac{27}{4}(CD)^2
\\ AG = \dfrac{3\sqrt{3}}{2}CD
$$

This is great. We can know figure out the value of CD.

$$
A_{BDF} = \dfrac{81}{2}\sqrt{3}
\\ \dfrac{1}{2}(BF)(DF) = \dfrac{81}{2}\sqrt{3}
\\ \dfrac{1}{2}(\dfrac{3}{2}CD)(\dfrac{3\sqrt{3}}{2}CD) = \dfrac{81}{2}\sqrt{3}
$$

By inspection, we can cancel $$\sqrt{3}$$, 81, 3 and 2. Leaving us with,

$$
(CD)^2 = 36
\\ CD = 6
$$

A mystery unlocked.

Now we just need the value of EF. Notice that if we have a line, EB. We would be producing a right triangle. 
A right triangle of lines AB, BE, and EA. 

Consequentially, we can also create a similar right triangle expression.

"In a right triangle, if the altitude drawn from the right angle to the hypotenuse divides the hypotenuse into two segments, then the length of the altitude is the geometric mean of the lengths of the two segments." ([Source](https://calcworkshop.com/triangle-trig/similar-right-triangles))

Let $$ EF = a $$ 

$$
\dfrac{AF}{EF} = \dfrac{EF}{BF}
\\ AF = 3, BF = 9
\\ \dfrac{3}{a} = \dfrac{a}{9}
\\ a^2 = 27
\\ EF = a = 3\sqrt{3} 
$$

The area of right triangle AFE is,

$$
A_{AFE} = \dfrac{1}{2}(AF)(EF)
\\ = \dfrac{1}{2}(3)(3\sqrt{3})
\\ = \dfrac{9}{2}\sqrt{3}
$$

The area of the rectangle AGDF is,

$$
A_{AGDF} = (AF)(AG)
\\ = 3(9\sqrt{3})
\\ = 27\sqrt{3}
$$

And we have finally reached the end. 

The area of the polygon AGDB is,

$$
A_{AGDB} = A_{AGDF} + A_{BDF}
\\ = 27\sqrt{3} + \dfrac{81}{2}\sqrt{3}
\\ = \dfrac{135}{2}\sqrt{3}
$$

While the area of the polygons without the trapezium is,

$$
A_{AFE} + A_{BDF} = \dfrac{9}{2}\sqrt{3} + \dfrac{81}{2}\sqrt{3}
\\ = \dfrac{90}{2}\sqrt{3}
$$

And therefore...

$$
A_{AGDE} = \dfrac{135}{2}\sqrt{3} - \dfrac{90}{2}\sqrt{3}
\\ = \dfrac{45}{2}\sqrt{3}

$$

</details>