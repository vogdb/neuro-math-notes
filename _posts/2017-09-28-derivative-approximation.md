---
layout: post
title:  "Derivative Approximation"
date:   2017-09-28 20:10:00 +0300
tags: Math Derivative
---

**Prerequisites** [Derivative]({{ site.baseurl }}{% post_url 2017-09-14-derivative %})

### Linear approximation

When function is approximated by a linear function it is a linear approximation. Linear derivative approximation is when we use the derivative of the function at some point to get its linear approximation at the vicinity \\(\Delta x\\) of the point. The second derivative of function gives us concavity and hence whether the function is located below or above its linear approximation.

{: .centered}
![Linear approximation]({{ site.url }}/assets/images/derivative-approximation/linear-approximation.jpg){:height="300"}
*Linear approximation*

Mathematically (\\(x\\) is the derivative point):
\\[\Delta f = Slope_{tangent} \Delta x = f\'(x)\Delta x\\]
\\[f(x + \Delta x) = f\'(x)\Delta x + f(x)\\]
