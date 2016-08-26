---
layout: post
title: Equivalence relations and infinite-time computable reductions
category: presentation
tags: ittm
---

Effective Mathematics of the Uncountable, New York, August 2008<!--more-->

*Abstract*: Many classification problems can be thought of as an equivalence relations on $2^\omega$. For instance, any countable linear ordering on $\omega$ can be coded as an element of $2^\omega$, and the classification problem for countable linear orders can be identified with the isomorphism equivalence relation on these codes. If $E,F$ are equivalence relations on $2^\omega$, then a *reduction* from $E$ to $F$ is a function $f\colon2^\omega\to2^\omega$ such that $x\mathrel{E}x'\iff f(x)\mathrel{F}f(x')$.

If the reduction function is reasonably explicit, then we say that the classification problem up to $E$ is no more complicated than that up to $F$.

In the study of Borel equivalence relations one defines that $E\leq_BF$ iff there exists a Borel reduction from $E$ to $F$. In this talk, we instead consider infinite-time Turing computable reductions. Such reductions are more powerful than Borel reductions; indeed any Borel function is infinite-time computable from a real parameter. It is then possible to use infinite-time computable reductions to analyze very natural equivalence relations which are beyond Borel in complexity.
