---
layout: post
title:  "Math glossary and pronunciation"
date:   2017-09-18 21:00:00 +0300
tags: Math
---

### General

<!-- TODO Units, conversation of Units. Significant numbers, Системы счисления. Четные/нечетные/натуральные/действительные(rational, irrational), greek numbers.
-->
**0**. Zero, oh, naught.

**Order of magnitude**. The order of magnitude \\(b\\) of a number \\(N\\) is the smallest power of \\(10\\) required to represent that number. \\(N=a \cdot 10^b, 0.5 < a \leq 5\\). Example: \\(N=1324=1.324 \cdot 10^3, b=3\\), \\(N=0.001324=1.324 \cdot 10^{-3}, b=-3\\)

**Multiplication**. \\(a \cdot b\\). Multiplication or product of \\(a\\) and \\(b\\). \\(a\\) times \\(b\\). \\(a,b\\) are factors.

**Division**. \\(\frac{a}{b}\\) Quotient of \\(a\\) and \\(b\\). Ratio \\(a\\) to \\(b\\). \\(a\\) over \\(b\\). \\(a\\) is the numerator. \\(b\\) is the denominator.

**Fractions**. \\(\frac{2}{3}\\) two thirds, \\(\frac{4}{3}\\) four thirds.

**Reciprocal**. \\(a=\frac{1}{b}\\) \\(a\\) is reciprocal to \\(b\\) and vice versa.

**Factorization**. \\(k\*x + k\*y = k\*(x+y)\\). Decomposition into a product of multiple factors. Factor out the common factor \\(k\\).

**Exponentiation**. \\(a^n\\). \\(a\\) is the base, \\(n\\) is the exponent. \\(a\\) is raised to the \\(n\\)-th power. \\(a^2\\) \\(a\\) squared. \\(a^3\\) \\(a\\) cubed.

**Root**. \\(\sqrt[n]{a} = a^{\frac{1}{n}}\\). The \\(n\\)th root of \\(a\\). \\((\sqrt[n]{a})^n = a\\)

**Delta**. \\(\Delta x, \delta x\\): small difference of some value. Here the value is \\(x\\).

**Infinitesimal**. Infinitely small value.

**Closed interval**. \\([a,b] \implies a \leq x \leq b\\)

**Open interval**. \\((a,b) \text{ or } ]a, b[\implies a < x < b\\)

**Half-open/closed interval**. \\([a,b)\\) or \\((a,b]\\)

**Number \\(e\\)** .Euler's number. Constant. Defined as \\(\lim_{n \to \infty} (1 + \frac{1}{n})^n\\). See Exponent functions of [Derivative]({{ site.baseurl }}{% post_url 2017-09-14-derivative %}).

### Functions
**Definition**. \\(y=f(x)\\). \\(f\\) of \\(x\\). \\(x\\) is input. \\(y\\) is output. \\(f\\) is the function. \\(f\\) can only have one output, \\(y\\), for each unique input, \\(x\\).

**Domain of function**. The set of allowable input values.

**Range of function**. The set of all possible output values.

**Vertical line test**. If a vertical line intersects a curve on an xy-plane more than once then the curve is not a function.

**Explicit function**. When \\(f\\) is explicitly expressed by its arguments. Example \\(y=\pm\sqrt{x^2+25}\\)

**Implicit function** When \\(f\\) is implicitly given by an equation with its arguments. Example \\(y^2 + x^2 = 25\\)

**Inverse function**. When \\(f\\) undoes what \\(g\\) did then \\(f\\) is the inverse of \\(g\\) and vice versa. \\(y=f(x), x=g(y), x=g(f(x)), y=f(g(y)) \implies g=f^-1, f=g^-1\\). Not every function has its inverse. Graphically for two-dimension functions we swap \\(x\\) and \\(y\\), e.g. reflect over \\(y=x\\) line.

**Horizontal line test**. If a horizontal line intersects a function graph on an xy-plane more than once then the function does not have the complete inverse.

**One-to-one**. \\(\forall a \ne b, f(a) \ne f(b) \implies f \text{ is one-to-one}\\).

**Function composition** When \\(f\\) is a function of \\(x\\) and \\(x\\) is a function of \\(t\\) we have a composition of functions.
\\[f = g(x), x = h(t) \text{ or } f(t) = g(h(t)), \text{ h - inner, g - outer}\\]
For example. The temperature of a ship is a function of its distance to the sun. The distance is a function of time. So, in the end the temperature is the function of time.

**Exponential function**. Function where input is the exponent.

### Trigonometry
**Unit circle** A circle with the radius of \\(1\\)

**Circumference** The enclosing boundary of a curved geometric figure, especially a circle. For circle is \\(2\pi r\\).

**Number \\(\pi\\)** .Pronounce as *pie*. Constant. The ratio of circle's circumference to its diameter.

**Radians** Unit of angle measurement. We take a unit circle. The length of an arc is the radians measurement of the angle that it subtends. So the angle is one radian if the length of its arc is \\(1\\)

{: .centered}
![Radian]({{ site.url }}/assets/images/math-glossary/Circle_radians.gif){:height="200"}
*Radian*

**Sin, Cos, Tan**. Pronounce as *sign*, *cosign*, *tan or tangent*. Functions of angle. \\(cos=\frac{\text{adjacent}}{hypotenuse}\\), \\(sin=\frac{\text{opposite}}{hypotenuse}\\), \\(tan=\frac{sin}{cos}\\)

{: .centered}
![sin, cos]({{ site.url }}/assets/images/math-glossary/Unit_circle.svg){:height="200"}
*\\(sin, cos\\)*
