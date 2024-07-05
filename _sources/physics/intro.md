# Introduction
These are notes I made while learning about new aspects of quantum mechanics and information while doing my research work with the Quantum Fields and Quantum Information research lab. To get the most out of these notes I suggest having an undergraduate level understanding of quantum mechanics but I may go over some fundamentals when appropriate.  

## Conventions
When working with the position and momentum (quadrature) operators, $q$ (or more commonly $x$) and $p$ respectively, we will define them as 

$$
x = q = \frac{1}{\sqrt{2}} (a+ a^\dagger), \quad p = \frac{1}{\sqrt{2}i}(a - a^\dagger)
$$

solving for $\hbar$ using the canonical commutation relations $[q,p] = i\hbar$ and $[a, a^\dagger]=1$ we get $\hbar=1$ {cite:p}`mcintyre2022quantum`. As a refresher let's do this calculation.

$$
\begin{align*}
i\hbar=[q,p] &= qp - pq\\
&= \left( \frac{-i}{2}(a+a^\dagger)(a-a^\dagger) + \frac{i}{2}(a-a^\dagger)(a+a^\dagger)  \right)\\ 
&=  \left(\frac{-i}{2}\left(a^2 -aa^\dagger + a^\dagger a - {a^\dagger}^2 )  + \frac{i}{2}(a^2+aa^\dagger - a^\dagger a - {a^\dagger}^2\right)\right) \\
&= \frac{i}{2}\left( -a^2 + aa^\dagger - a^\dagger a + {a^\dagger}^2 + a^2 +aa^\dagger - a^\dagger a - {a^{\dagger}}^2 \right) \\
&= \frac{i}{2}\left( 2aa^\dagger - 2a^\dagger a\right)\\
&= i\left( aa^\dagger - a^\dagger a\right)\\
&= i[a,a^\dagger] \\
&= i  \quad \text{Since we know $[a,a^\dagger]$=1}
\end{align*}
$$
This means $i\hbar=i$ and so $\hbar=1$. I've seen others use conventions like $\hbar=2$, you can always check what value someone is working with by doing the above calculation with the definition of $q$ (or $x$) and $p$ that they give.

## What is this $q$ thing?

So this is a question I had when I first saw this being used to denote the position operator. I think it comes from 