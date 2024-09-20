# Continuity at a point
A function $f(x)$ is continuous at an interior point $c$ of its [[Functions#Domain and co-domain of a function|domain]] if and only if:
1. $f(c)$ exists, $c$ lies in the domain of $f$
2. $\lim_{x\to c} f(x)$ exists
3. $\lim_{x\to c} f(x) = f(c)$, the limit equals the function value
If any of these conditions are not met, $f$ is not continuous at $c$.
# Laws of continuity
If we assume that $f$ and $g$ are continuous at $c$, then the following combinations are continuous at $c$:
1. $f+g$
2. $f-g$
3. $k \cdot f$, with $k \in \mathbb{R}$
4. $f \cdot g$
5. $\frac{f}{g}$, with $g(c) \ne 0$
6. $f^n$, with $n \in \mathbb{N}$
7. $\sqrt[n]{f}$, with $n \in \mathbb{N}$
# Composition of continuous functions
>[!info] Theorem
> If $f$ is continuous at $c$, and $g$ is continuous at $f(c)$, then $g \circ f$ is continuous at $c$.

>[!note] 
>The composition $g \circ f$ is the function that maps $x$ to $g(f(x))$.
# Global continuity
>[!info] Definition
>A function $f$ is continuous if $f$ is continuous on its entire domain.

This definition is not completely agreed upon, so this definition may vary from resource to resource.
According to this definition $f(x) = \frac{1}{x}$ is continuous!
![[Pasted image 20240920122316.png]]
