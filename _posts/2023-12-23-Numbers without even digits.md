---
layout: post
title:  "Numbers without even digits"
date: 2023-12-23 15:00 +0700
category: math
description: im actually bad at counting???
---
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

# The problem

What percentage of the first 100 positive integers contains no even digits?

# My attempt

I decided to count the even digits first.

Easy. The first 10 digits only has 4 even digits. 2, 4, 6, 8.

We also know that 20, 40, 60, 80, all of its consecutive numbers are even digits.

$$
4*10 = 40
$$

Then the numbers that starts with odd digits (10's, 30's, 50's, 70's, 90's), there are 5 of them.

Within those numbers, there are 5 even digit numbers (we include 0)

So $$5*5=25$$

And lastly the number 100 is even because it contains a 0.

Summing all the even digit numbers...

$$
4+40+25+1=70
$$

So the percentage of numbers without even digits are...

$$
\dfrac{100-70}{100}=\dfrac{30}{100}
$$

Yes it is 30%.

But I soon realized there is a more efficient way of dealing with this problem.

# The answer from community post

We immediately count all the non-even digits. The counting is splitted into three parts: one digit numbers, two digit numbers, and three digit numbers.

For the one digit numbers,
easy it is all the odd digits such as 1,3,5,7,9. We have 5.

For the two digit numbers,
we can arrange non-even digit numbers by using the 5 odd digit numbers. This will be $$5*5=25$$

For the three digit number, 100, it is an even digit number.

So there you have it, $$25+5=30$$ or $$\dfrac{25+5}{100}=\dfrac{30}{100}$$.

# Conclusion
I still have a lot to practice for combinatorics & permutations problems.....

This result is also interesting because 30% of numbers without even digits is kinda mindblowing. There are just a lot of numbers with even digits then.