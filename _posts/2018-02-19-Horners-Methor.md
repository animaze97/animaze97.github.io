---
layout: post
title: Introduction to Horner’s Method
tags: [Mathematics, Polynomials, Programming, Horner]
---
![](/img/horner_method_1.jpeg)


In this post I would be discussing Horner’s method which made my life a hell lot of easier dealing with scary-looking polynomials. It’s basically a method that can be used for approximating the roots of a polynomial fairly quickly. Once you have this in your arsenal, you can factorize higher degree polynomials within seconds and without any effort.

For explaining this method, I will be using the polynomial:

F(x) = 2x⁴–20x³+70x²–100x+48

And from our previous knowledge about polynomials we know that the constant term is equal to the product of the roots of the polynomial (assuming you know this, if you paid attention to the blabbering of your math teacher).

Step 1) Take the constant term in the polynomial and find its factors (both positive and negative). In our case, its 48, so we would have ±1, ±2, ±3, ±4, ±6, ±8, ±12, ±16, ±24 ±48.

Step 2) Write the coefficients of the polynomial starting from the highest degree (4 in our case) to the lowest degree (0 — constant term), and put 0 if any degree coefficient is missing in the given polynomial (For example, If the polynomial is of the form x²+1, then coefficient of degree 1 is missing, so we would have 1 0 1). So, for F(x) we would have something like: 2 -20 70 -100 48.

Step 3) Take any factor of 48 (suppose we take -1) and do the following:


As we can see in the above image that the remainder (final entry) is not 0 (it’s 240), so we can say that -1 is not a root of the polynomial.

Step 4) Now take the next factor of 48 (suppose we take +1) and repeat the same process.


In this case, the remainder (final entry) came out to be 0, so we know that +1 is a factor of the polynomial or (x-1) divides F(x). The remaining entries in the final row (in the above image) are: 2 -18 52 48.

These entries represent the coefficients of the polynomial

G(x) = F(x)/(x-1) = 2x³–18x²+52x+48.

Now repeat the above steps with G(x) to find the remaining roots. At first, you might think it is an overkill to use this method to factorize polynomials, but believe me with a bit of practice you can find all the roots fairly quickly as compared to any other method.

As for the given polynomial (F(x)), its roots are: 1, 2, 3, 4. Solve yourself and match your answer to get the hang of it.
