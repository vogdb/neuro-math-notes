---
layout: post
title:  "Probability theory"
date:   2017-10-19 17:00:00 +0300
tags: Math
---

**Prerequisites** [Matt glossary]({{ site.baseurl }}{% post_url 2017-09-18-math-glossary %})

**Experiment.** Something that happens with an outcome. For example. An experiment is when we flip a coin once. An outcome then is either Heads(*H*) or Tails(*T*). Another experiment would be to flip the coin twice. An outcome then is a sequence of Heads and Tails. The result of one coin flip is not an outcome in such experiment. It is just a stage or intermediate result.

**Sample set.** Set of all possible outcomes. The experiment with one flip of a coin has a set *{H, T}*. Two flips is *{HH, TT, HT, TH}*. It must be: *mutually exclusive*, *collectively exhaustive*.

**Event.** A subset of the sample set.

**Cardinality of Set.** Size of Set.

\\(\binom{n}{k}\\) Over \\(n\\) choose \\(k\\).

**Venn diagram.**

{: .centered}
![Intersection of Sets]({{ site.url }}/assets/images/probability-theory/venn-intersection.svg){:height="300"}
*Intersection of Sets*

**Inclusion-Exclusion principle**
\\[|A \cup B| = |A| + |B| - |A \cap B|,\text{ where |A| number of elements in A}\\]

Intersection of elements is counted twice. Thus we need to extract it.

**Product of sets.** Set of ordered pairs where first item belongs to the first set and second item to the second set.

**Product Rule.** If there are **n** ways to perform action 1 and then by **m** ways to perform action
2, then there are \\(n \cdot m\\) ways to perform action 1 followed by action 2. You have **n** possibilities to pick the first item and **m** possibilities for the second.

**Permutations.** It is a set of elements in a particular order, e.g a list. For example, *{a, b, c}* has 6 permutations: *abc, acb, bac, bca, cab, cba*. Using *Product Rule* we can say that there are \\(k!\\) permutations of any set with \\(k\\) elements. Cause we have \\(k\\) possibilities to pick the first, \\(k-1\\) for the second and so on. In general for a set with \\(n\\) elements the number of permutations of \\(k\\) size is
\\[ \_{n}P_{k} = n(n-1)...(n-k+1)=\frac{n!}{(n-k)!} \\]

**Combinations.** Set of elements where order does not matter, e.g. sets. *abc* = *acb* = *cba*. When we have \\(k\\) elements, we can draw \\(k!\\) permutations from them. But as a combination it represents a single combination for \\(k!\\) of permutations. So in order to get the number of combinations we can divide the number of permutations by \\(k!\\).
\\[ \_{n}C_{k} = \frac{n!}{k!(n-k)!} \\]

**Conditional probability.** Probability of \\(A\\) given \\(B\\) occurred.

\\[ P(A \cap B) = P(B)P(A\|B) \implies P(A\|B) = \frac{P(A \cap B)}{P{B}}\\]
