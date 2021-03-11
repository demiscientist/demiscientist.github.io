---
layout: post
title: Once Normalized, Always Normalized
---

{{ page.title }}
================

<p class="meta">30 July 2015 - New Delhi</p>

Quantum mechanics’ approach to solve a problem involves looking for the particle’s (the body under consideration) wave function, $$\Psi(x,t)$$, and we get it by solving the Schrödinger equation: 
\begin{equation}
i\hbar\frac{\partial \Psi}{\partial t} = -\frac{\hbar^2}{2m} \frac{\partial^2 \Psi}{\partial x^2} + V\Psi
\end{equation}

The Schrödinger equation plays a role logically analogous to Newton’s second Law, i.e., given suitable initial conditions $$\Psi(x,0)$$, the Schrödinger equation determines $$\Psi(x,t)$$ for all future time, just as in classical mechanics.

To know what exactly is this “wave function”, and what is its utility? As we already know, a particle, by virtue of its nature, is localized at a point, whereas the wave function is spread out in space. This fact is in itself confusing, how can such an object represent a particle?
The answer is provided by Born’s statistical interpretation of the wave function, which says that $$\left |\Psi(x,t)\right |^2$$ gives the probability of finding the particle at point x, at time t. Probability is the area under the graph of \left |\Psi^2\right |. It follows from the properties of discrete distributions that,

{\displaystyle \int_{-\infty}^{+\infty}\left |\Psi(x,t)\right |^2\,dx =1}

However, it’d be delinquent on our part if we do not check the consistency of both the Schrödinger equation and the Born’s statistical interpretation.

Well, a glance at Schrödinger equation reveals that if {\displaystyle \Psi(x,t)} is a solution, so too is {\displaystyle A\Psi(x,t)}, where A is any (complex) constant. We must pick this undetermined multiplicative factor so as to ensure that statistical interpretation is satisfied. This process is called the normalizing the wave function. One should keep in mind that non-normalizable solutions cannot represent particles, and must be rejected. Physically realizable states correspond to the square-integrable solutions to Schrödinger’s equation.

However, the more important question is if we’ve a normalized wave function at time t=0, how do we know that it’ll stay normalized, as time goes on, and \Psi evolves?
Fortunately, the Schrödinger equation has the remarkable property that it automatically preserves the normalization of the wave function—without this crucial feature the Schrödinger equation would be incompatible with the statistical interpretation, and the whole theory would crumble.

To check time evolution of normalization,
