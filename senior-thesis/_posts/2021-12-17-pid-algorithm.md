---
title: The PID controller algorithm
tags: combinatorics
---

A senior thesis by Ryan Amidan, Fall 2021<!--more-->

*Abstract*: The PID algorithm is a closed loop correction mechanism which stands for Proportional, Integral, Derivative. The Purpose of the PID algorithm is to make adjustments to a variable $Y$ that is not meeting it's target value $Y\_t$. The PID algorithm will adjust an input variable $x$ in order to move $Y$ towards $Y\_t$ without any user input, within a certain error tolerance. Depending on the values of the constants $P$, $I$ and $D$ the adjustments made to reach $Y\_t$ can become quicker and more accurate.