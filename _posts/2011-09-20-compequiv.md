---
title: The hierarchy of equivalence relations on the natural numbers under computable reducibility
permalink: /compequiv
category: publication
tags: computability
---

With Joel Hamkins and Russell Miller. *Computability*, 2012.  ([ar&chi;iv](http://arxiv.org/abs/1109.3375) \| [journal](http://dx.doi.org/10.3233/COM-2012-004))<!--more-->

*Abstract*: The notion of computable reducibility between equivalence relations on the natural numbers provides a natural computable analogue of Borel reducibility.  We investigate the computable reducibility hierarchy, comparing and contrasting it with the Borel reducibility hierarchy from descriptive set theory.  Meanwhile, the notion of computable reducibility appears well suited for an analysis of equivalence relations on the c.e. sets, and more specifically, on various classes of c.e. structures.  This is a rich context with many natural examples, such as the isomorphism relation on c.e. graphs or on computably presented groups.  Here, our exposition extends earlier work in the literature concerning the classification of computable structures.  An abundance of open questions remains.

*Further notes*: My background lies in an area called Borel equivalence relations.  I'll say a lot more about this subject later, but for now let me motivate this post by briefly describing the importance of equivalence relations in mathematics.  The point is that every classification problem gives rise to an equivalence relation.  For instance, the isomorphism problem for countable graphs boils down to studying the isomorphism equivalence relation on the space $\mathcal P(\mathbb N\times\mathbb N)$.  The key notion in the subject is *Borel reducibility*, which gives us a way to compare the difficulty of two classification problems:

If $E,F$ are equivalence relations on (reasonable) spaces of mathematical structures $X,Y$, then we say $E$ is *Borel reducible* to $F$ if there is a Borel function $f\from X\into Y$ satisfying $x\mathrel{E}x'\iff f(x)\mathrel{F}f(x')$.

Here, "Borel" is a technical stand-in for "reasonably explicit or definable".

In this present project, we wanted to find an analogous theory for equivalence relations on the natural numbers.  Unfortunately, since all functions on $\mathbb N$ are Borel (in fact all countable objects are trivially Borel) there is no use in looking at Borel reducibility in this case.  Thus, for reasons which are both practical and aesthetic, we wanted the class of reduction functions to be those which are *computable* by a Turing machine.

The notion of reducibility of equivalence relations on $\mathbb N$ turns out to be a generalization of the more traditional notion of reducibility of *subsets* of $\mathbb N$.  Indeed, a subset $A\subset\mathbb N$ can more or less be represented in the hierarchy of equivalence relations by $E_A$, where $x\mathrel{E_A}x'\iff x,x'\in A$ or $x=x'$.  Thus in the paper, we spend a few sections laying out the very elementary theory of reductions between equivalence relations.

On the other hand, the notion of reducibility of equivalence relations on $\mathbb N$ also turns out to be a kind of specialization of the study of equivalence relations on $\mathcal P(\mathbb N)$ (or any of the broad class of spaces considered in the Borel theory).  This is because all of the most important elements of $\mathcal P(\mathbb N)$ are for instance c.e., that is, enumerable by a Turing machine!

Now, we can regard any equivalence relation on the c.e. sets as an equivalence relation on $\mathbb N$ as follows.  First let $W_n\subset\mathbb N$ be the subset enumerated by the $n$th Turing machine, according to some reasonable indexing of all of the Turing machines.  Then, given any equivalence relation $E$ on $\mathcal P(\mathbb N)$, we can consider its "c.e. version" $E^{ce}$ by specifying $n\mathrel{E}^{ce}n'$ iff $W_n\mathrel{E}W_{n'}$.  It's as simple as that.

This leads naturally to a rather extensive program: how does the theory of equivalence relations on $\mathcal P(\mathbb N)$ with respect to Borel reducibility compare with the theory of equivalence relations on c.e. subsets of $\mathbb N$ with respect to computable reducibility?  Do they agree or disagree in the case of basic examples?  Do classical definitions and theorems have reasonable analogs in the computable scenario?  We begin to answer these questions, and I may give some of our findings in a future post.  But for now I'll leave it there, and note that there is much more to be done.
