---
layout: post
title:  "Derivative"
date:   2017-09-14 21:23:00 +0300
tags: Math Derivative
---

**Prerequisites** [Limits]({{ site.baseurl }}{% post_url 2017-09-02-limits %}), [Matt glossary]({{ site.baseurl }}{% post_url 2017-09-18-math-glossary %})

### Rate of change of function.

Let \\(f\\) be a function of \\(t\\). At \\(t=4, f(t)=10\\). At \\(t=7, f(t)=28\\). The **Average value** of \\(f\\) at the interval \\([4, 7]\\) is \\((10 + 28)/2 = 19\\). But the **Average rate of change** of \\(f\\), e.g. how fast/slow it has been changing on the interval, is \\(\frac{f(7) - f(4)}{7 - 4} = 18/3 = 6\\).
It means that function's value has been increasing at a rate \\(6\\) units of \\(f\\) per unit of \\(t\\). Of course this rate can be negative. The Average rate of change on an interval is the slope of the Secant line that crosses the function at the interval's boundaries.
\\[\text{Average rate of change} = Slope_{secant} = \frac{f(a) - f(b)}{a - b}\\]

{: .centered}
![The Average rate of change]({{ site.url }}/assets/images/derivative/average-rate-change.svg){:height="300"}
*The Average rate of change*

### Derivative definition

The Average rate of change gives the interval's rate. The rate of change in a point is called **the instantaneous rate of change** and it is the **Derivative** of function in that point. The **Derivative** of function \\(f\\) of argument \\(x\\) in point \\(a\\) is the instantaneous rate of change of this function in \\(a\\). It is denoted as "\\(f\\) prime of \\(a\\)":
\\[f\'(a) = Slope_{tangent} = \lim_{x \to a} \frac{f(a) - f(x)}{a - x} = \lim_{\Delta x \to 0} \frac{f(a + \Delta x) - f(a)}{\Delta x} \\]
As you can see we get the derivative when we start calculating the Average rate of change on less and less intervals. Mathematically it means the limit of average rates of \\(f\\) in point \\(a\\). Graphically it is the slope of the tangent line in \\(a\\). The Tangent line is a line (linear function) that approximates function in the point. For a linear function the tangent is the function itself.

{: .centered}
![Derivative]({{ site.url }}/assets/images/derivative/derivative.svg){:height="300"}

### Derivative graphs

<p class="centered">
  <span class="half-width">
    <img src="{{ site.url }}/assets/images/derivative/build-derivative-graph-1.svg" alt="function graph">
    <em>Function graph</em>
  </span>
  <span class="half-width" style="vertical-align: top">
    <img src="{{ site.url }}/assets/images/derivative/build-derivative-graph-2.svg" alt="Sketch of derivative graph">
    <em>Sketch of function's derivative graph</em>
  </span>
</p>

{: .centered}
[![graph Derivative function](https://img.youtube.com/vi/Gbtma_UQpro/0.jpg)](https://www.youtube.com/watch?v=Gbtma_UQpro)
*How to graph Derivative function*

### Derivative calculation
**By definition** for example \\(x^2\\)
\\[ \\forall a, f\'(a) = \lim_{x \to a} \frac{f(x) - f(a)}{x - a} = \lim_{x \to a} \frac{x^2 - a^2}{x - a} = \lim_{x \to a} x + a = 2a \\]
**Linear combinations**
\\[f\'(x) = g\'(x) + h\'(x), f(x) = g(x) + h(x) \\]
\\[f\'(x) = Kg\'(x), f(x) = Kg(x) \\]
**General power rule** If \\(n\\) is any fixed number and \\(f(x) = x^n\\). Easy to prove by definition. Some factorization is required.
\\[f\'(x) = nx^{n-1}\\]
