---
layout: post
title: The fundamental theorem on symmetric polynomials
permalink: /symmetric
category: publication
tags: galois algebra
---

History's first whiff of Galois theory.  With Ben Blum-Smith. *College mathematics journal*, 2017. ([ar&chi;iv](http://arxiv.org/abs/1301.7116) \| [journal](http://dx.doi.org/10.4169/college.math.j.48.1.18))<!--more-->

*Abstract*: We describe the fundamental theorem on symmetric polynomials (FTSP), exposit a classical proof, and offer a novel proof that arose out of an informal course on group theory. The paper develops this proof in tandem with the pedagogical context that led to it. We also discuss the role of the FTSP both as a lemma in the original historical development of Galois theory and as an early example of the connection between symmetry and expressibility that is described by the theory.

*Additional summary*: This expository and pedagogical article was initiated by Ben Blum-Smith, and is based on some discussions that came out of an abstract algebra class he gave for teachers in New York.

The fundamental theorem on symmetric polynomials states that if a polynomial in $n$ variables is *symmetric* (meaning it is invariant under permutations of the variables), then it can be expressed in terms of the *elementary symmetric polynomials*:
\[\begin{array}{c}x_1+\cdots+x_n\\
x_1x_2+\cdots+x_{n-1}x_n\\
\vdots\\
x_1\cdots x_n\end{array}
\]
This elementary result played a key role in Galois' work.  The standard proof is an inductive one, and is based on a monomial order such as the lexicographic ordering on the terms of the given polynomial $f$.

This argument, while standard among the experienced, is not easy to arrive at from a naive perspective.  In this article we present another proof which arose out of our inquiry-based discussions in which the terms of $f$ are dealt with based on a natural notion of how "spread out" their exponents are.
