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
The answer is provided by Born’s statistical interpretation of the wave function, which says that $$\left |\Psi(x,t)\right |^2$$ gives the probability of finding the particle at point $$x$$, at time $$t$$. Probability is the area under the graph of $$\left |\Psi^2\right |$$. It follows from the properties of discrete distributions that,

\begin{equation}
\int_{-\infty}^{+\infty}\left |\Psi(x,t)\right |^2\,dx =1
\end{equation}

However, it would be delinquent on our part if we do not check the consistency of both the Schrödinger equation and the Born’s statistical interpretation.

Well, a glance at Schrödinger equation reveals that if $$\Psi(x,t)$$ is a solution, so too is $$A\Psi(x,t)$$, where $$A$$ is any (complex) constant. We must pick this undetermined multiplicative factor so as to ensure that statistical interpretation is satisfied. This process is called the normalizing the wave function. One should keep in mind that non-normalizable solutions cannot represent particles, and must be rejected. Physically realizable states correspond to the square-integrable solutions to Schrödinger’s equation.

However, the more important question is if we’ve a normalized wave function at time $$t=0$$, how do we know that it will stay normalized, as time goes on, and $$\Psi$$ evolves?
Fortunately, the Schrödinger equation has the remarkable property that it automatically preserves the normalization of the wave function—without this crucial feature the Schrödinger equation would be incompatible with the statistical interpretation, and the whole theory would crumble.

To check time evolution of normalization,

\begin{equation}
\frac{d}{dt}\int_{-\infty}^{+\infty}\left |\Psi(x,t)\right |^2 dx = \int_{-\infty}^{+\infty}\frac{\partial}{\partial t}\left |\Psi(x,t)\right |^2 dx
\end{equation}

Writing Schrödinger equation as:

\begin{equation}
\frac{\partial \Psi}{\partial t} = \frac{i\hbar}{2m} \frac{\partial^2 \Psi}{\partial x^2} - \frac{i}{\hbar}V\Psi
\end{equation}

Similarly,

\begin{equation}
\frac{\partial \Psi^{\ast}}{\partial t} = -\frac{i\hbar}{2m} \frac{\partial^2 \Psi^{\ast}}{\partial x^2} + \frac{i}{\hbar}V\Psi
\end{equation}

Since $$V$$ and $$\Psi$$ are real.

Substituting in the first equation and rearranging, we get;

\begin{equation}
\Rightarrow \frac{\partial \left |\Psi\right |^2}{\partial t} = \frac{i\hbar}{2m} \Big( \Psi^{\ast}\frac{\partial^2 \Psi}{\partial x^2} - \Psi\frac{\partial^2 \Psi^{\ast}}{\partial x^2}\Big ) = \frac{\partial}{\partial x}\Big { \frac{i\hbar}{2m}\Big(\Psi^{\ast}\frac{\partial \Psi}{\partial x} - \Psi\frac{\partial \Psi^{\ast}}{\partial x}\Big )\Big}
\end{equation}

\begin{equation}
\therefore, \frac{d}{dt}\int_{-\infty}^{+\infty}\left |\Psi(x,t)\right |^2 dx = \frac{i\hbar}{2m}\Big (\Psi^{\ast}\frac{\partial \Psi}{\partial x} - \Psi\frac{\partial \Psi^{\ast}}{\partial x}\Big )_{-\infty}^{+\infty}
\end{equation}

Since, \Psi(x,t)\rightarrow 0 as x\rightarrow \infty for \Psi(x,t) to be non-normalizable.

It follows,

{\displaystyle \frac{d}{dt}\int_{-\infty}^{+\infty}\left |\Psi(x,t)\right |^2 dx = 0.}

and hence, integral is a constant (independent of time); if \Psi is normalized at t=0, it stays normalized for all future time.

Q.E.D.

Hence, we can conclude that wave function once normalized is always normalized.

Though we’ve discussed the normalization and the time evolution of the wave function but it’d be sin on my part if I don’t argue on the plausibility of Schrödinger equation itself. Hence, I’d like to add little plausibility argument leading to Schrödinger equation—

We know very well that wave equation for a stretched string can be derived from Newton’s law, and the electromagnetic wave equation can be derived from Maxwell’s equations; but we cannot expect to be able to derive the quantum mechanical wave equation from any of the equations of classical physics. However, we can expect to receive some help from the de Broglie-Einstein postulates,

{\displaystyle \lambda = \frac{h}{p}}           and           {\displaystyle \nu = \frac{E}{h}}

which connect, for the case of essentially constant p and E, the wavelength \lambda of the wave function with the linear momentum p of the associated particle, and also connect the frequency \nu of the wave function with the total energy E of the particle. The above equation plus others that we shall have reason to accept, will be woven into an argument that is designed to make the quantum mechanical wave equation seem more plausible, but I’d like to emphasize that this plausibility argument will not constitute a derivation. In the final analysis, the quantum mechanical wave equation will be obtained by a postulate, whose justification is not that it has been deduced entirely from information already known experimentally, but that it correctly predicts results which can be verified experimentally.

We begin our plausibility argument by listing four reasonable assumptions concerning the properties of the desired quantum mechanical wave equation:

It must be consistent with the de Broglie-Einstein postulates,
{\displaystyle \lambda = \frac{h}{p}} and {\displaystyle \nu = \frac{E}{h}}
It must be consistent with the total energy equation,
{\displaystyle E = \frac{p^2}{2m} + V}
It must be linear in \Psi(x,t). That is, if \Psi_1(x,t) and \Psi_2(x,t) are two different solutions to the equations for a given potential energy V, then arbitrary linear combination of these solutions, \Psi(x,t) = c_1\Psi_1(x,t) + c_2\Psi_2(x,t), is also a solution. This linearity requirement ensures that we shall be able to add together wave functions to produce the constructive and destructive interferences that are so characteristic of waves.
The potential energy V is generally a function of x, and possibly even t.
Wave associated with a particle—
Using wave equation,

{\displaystyle \triangledown^2\Psi = \frac{1}{v^2}\frac{\partial^2 \Psi}{\partial t^2}}

where, \Psi = \Phi(x,y,z)T(t)

where, \Phi(x,y,z) is the function of space.

We’re going to strictly consider V to be a function of just x, and not x and t.

Since we’re looking for harmonic solutions (following Schrödinger’s brilliant insight, we choose to express the phase of a plane wave in the superfluid vacuum as a complex phase factor via \Psi = Ae^{i(k.r-\omega t)}.), we’ve;

     {\displaystyle T(t) = e^{-i\omega t}}

{\displaystyle \therefore, T(t) = e^{-i\frac{2\pi}{h}t}}

where \omega = 2\pi \nu  and \nu = \frac{E}{h}

Now,

{\displaystyle \Psi = \Phi(x) e^{-i\frac{E}{\hbar}t}}

Substituting in the wave equation,

{\displaystyle \triangledown^2\Phi(x)e^{-i\frac{E}{\hbar}t} = \frac{1}{v^2}\frac{\partial^2 \Psi}{\partial t^2}}

{\displaystyle \Rightarrow \triangledown^2 \Phi(x) = -\frac{1}{v^2}\frac{E^2}{\hbar^2}\Phi(x)}

                                   {\displaystyle = -\frac{1}{v^2} 4\pi^2\nu^2\Phi(x)}

                         {\displaystyle = \frac{4\pi^2}{h^2}p^2\Phi(x)}

        {\displaystyle {\triangledown^2\Phi(x) + \frac{4\pi^2p^2}{\hbar^2}\Phi(x) = 0}}

for given E,

{\displaystyle \boxed{-\frac{\hbar^2}{2m}\Phi_E(x) + V\Phi_E(x) = E\Phi_E(x)}}

which is the required time-independent Schrödinger equation.

Also the time-dependent Schrödinger equation can be written as:

{\displaystyle \boxed{-\frac{\hbar^2}{2m}\triangledown^2\Psi(x,t) + V\Psi(x) = -\frac{\hbar}{i}\frac{\partial}{\partial t}\Psi(x,t)}}

In the end, I’d like to illustrate the steps for normalization of wave function of a particle in an infinite square well —

Starting with the wave equation: {\displaystyle \Psi(x) = A\sin\Big ({\frac{n \pi x}{a}}\Big )}

The wave function is a sine wave. You can see the first two wave functions plotted in the following figure.

Untitled-1-page-001

Wave \ function \ in \ a \ square \ well 

By normalizing the wave function we want to solve for the unknown constant A. In a normalized function, the probability of finding the particle between $$x$$ and $$x+dx$$, $$|\Psi(x)|^2dx$$,

Also, $$\int_{0}^{a}|\Psi(x)|^2dx = 1$$

Substituting for $$\Psi(x)$$ gives us:

{\displaystyle |A|^2 \int_{0}^{a}\sin^2{\Big ( \frac{n\pi x}{a}\Big )}dx = 1}

Solving the integral in the above equation, we get;

{\displaystyle \int_{0}^{a}\sin^2{\Big ( \frac{n\pi x}{a}\Big )}dx = \frac{a}{2}}

Using the previous equation,

{\displaystyle |A|^2\Big (\frac{a}{2}\Big ) = 1}

{\displaystyle \Rightarrow \ A = \sqrt{\frac{2}{a}}}

We finally arrive at the much awaited normalized wave function, with value of A plugged in,

{\displaystyle \Psi(x) = \sqrt{\frac{2}{a}}\sin{\Big ( \frac{n\pi x}{a}\Big )} \quad \quad n=1,2,3,}.

and that’s the normalized wave function for a particle in an infinite square well.

Hence, we’ve proved very basic but extremely important fact that a wave function once normalized, remains normalized and illustrated the steps to normalize the wave function of a particle in a square potential well.
