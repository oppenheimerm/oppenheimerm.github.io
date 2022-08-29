---
layout: post
description: Intermediate results with the walrus operator.
tags: python maths
---

Intermediate results with the walrus operator

Sometime we'll have a complex condition where we want to preserve an expensive intermediate result for later use.  Imagine a condition that involves a complex calculation; the cost of computing is high measured in time, or input-output, or memory, or network resource use.  Resource use defines the cost of computation.

This is an example where it cane be helpful to assign a name to the value or an expression.  We'll look at how to use the "assignment expression" or "walrus" operator.  It's called the walrus because the assignment expression operator, `:=`, looks lie the face of a walrus to some people.

\\[ x = {-b \pm \sqrt{b^2-4ac} \over 2a} \\]



Row-Echelon Form and Back-Subsitution

The method of elimination can be applied to a system of linear equations in more than two variables.  In fact, this method easily adapts to computer use for solving linear systems with dozens of variables.  

When elimination is used to solve a system of linear equations, the goal is to rewrite the system in a form to which back-substitution can be applies.  To see how this works, consider the following two systems of linear equations.


$$\begin{cases} 
x & - & 2y & + & 3z & = & 9\\\ 
& & y & + & 3z & = & 5\\\ 
& & & & z & = & 2 
\end{cases}$$

The second system is said to be in ***row-echelon form***, which means that it has a "stair-step" pattern with leading coefficients of 1.  After comparing the two systems, it should be clear that it is easier to solve the second system.

<p class="post-footer">Thanks for reading! <img src="/assets/images/assets/mo-144x144-white.png" alt="MO"></p>