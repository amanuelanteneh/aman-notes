# Introduction
These are notes I made while learning about new aspects of quantum mechanics and information while doing my research work with the Quantum Fields and Quantum Information research lab. To get the most out of these notes I suggest having an undergraduate level understanding of quantum mechanics but I may go over some fundamentals when appropriate.  

## Conventions


### Computing $\hbar$

Given the canonical position and momentum operators $x$ and $p$ in terms of the the annihaltion and creations operatrs, $a$ and $a^\dagger$,

$$
x = \frac{1}{\sqrt{2}} (a+ a^\dagger), \quad p = \frac{1}{\sqrt{2}i}(a - a^\dagger)
$$

we can solve for $\hbar$ using the canonical commutation relations $[x,p] = i\hbar$ and $[a, a^\dagger]=1$ to get $\hbar=1$ {cite:p}`mcintyre2022quantum`. As a refresher let's do this calculation.

$$
\begin{align*}
i\hbar=[x,p] &= xp - px\\
&= \left( \frac{-i}{2}(a+a^\dagger)(a-a^\dagger) + \frac{i}{2}(a-a^\dagger)(a+a^\dagger)  \right)\\ 
&=  \left(\frac{-i}{2}\left(a^2 -aa^\dagger + a^\dagger a - {a^\dagger}^2 )  + \frac{i}{2}(a^2+aa^\dagger - a^\dagger a - {a^\dagger}^2\right)\right) \\
&= \frac{i}{2}\left( -a^2 + aa^\dagger - a^\dagger a + {a^\dagger}^2 + a^2 +aa^\dagger - a^\dagger a - {a^{\dagger}}^2 \right) \\
&= \frac{i}{2}\left( 2aa^\dagger - 2a^\dagger a\right)\\
&= i\left( aa^\dagger - a^\dagger a\right)\\
&= i[a,a^\dagger] \\
&= i  \quad \text{Since we know $[a,a^\dagger]$=1}
\end{align*}
$$


This means $i\hbar=i$ and so $\hbar=1$. I've seen others use conventions like $\hbar=2$, you can always check what value someone is working with by doing the above calculation with the definition of $x$ and $p$ that they give.


### Quadratures

When working with the dimensionless position and momentum quadrature operators in quantum optics, $Q$ and $P$ respectively, they are explicitly defined in terms of $x$ and $p$ as

$$
\begin{align*}
    Q = \beta x \\
    P = \frac{p}{\beta \hbar},
\end{align*}
$$

where $\beta$ has dimensions of inverse length and is defined as 

$$
\begin{align*}
    \beta = \sqrt{ \frac{m\omega}{\hbar} }
\end{align*}
$$

with $\omega = \sqrt{\frac{k}{m}}$ being the resonance frequency of the quantum harmonic oscillator. We also define the non-Hermitian annihilation and creation ladder operators $a$ and $a^{\dagger}$ as

$$
\begin{align*}
    a =  \frac{1}{\sqrt{2}} (Q + iP) \\ 
    a^{\dagger} =  \frac{1}{\sqrt{2}} (Q - iP)
\end{align*}
$$


The quadrature operators can also be written in terms of the ladder operators as 

$$
Q = \frac{1}{\sqrt{2}} (a+ a^\dagger), \quad P = \frac{1}{\sqrt{2}i}(a - a^\dagger)
$$

Often times I have seen people just use $q$ and $p$ to denote these instead of the capital letters $Q$ and $P$ and I will do the same in any section of the notes that deals with continuous variable quantum information processing & computing. Note that unlike the $[x,p]$ the commutator of $Q$ and $P$ is equal to just $i$. 

#### What are these quadratures exactly?

I think these terms come from electrical engineering.