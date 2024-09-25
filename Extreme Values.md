# Absolute extreme values
> [!info] Definition
> Let $f$ be a real function with domain $D$. Let $c \in D$. Then $f$ has an **absolute maximum value on $D$ at $c$** if
> $$
> \forall x \in D \Big[f(x) \le f(c)\Big]
> $$
> and $f$ has an **absolute minimum value on $D$ at $c$** if
> $$
> \forall x \in D \Big[f(x) \ge f(c)\Big]
> $$

> [!info] The Extreme Value Theorem
> If a real function $f$ is **continuous** on a **closed** and **bounded** interval $[a,b]$, then $f$ attains both an absolute maximum value and an absolute minimum value on $[a,b]$.
> ![[Pasted image 20240925110912.png]]

To use the Extreme Value Theorem, it is very important that all of its conditions are satisfied. That means the interval must be continuous, closed and bounded.
![[Pasted image 20240925111128.png]]

## Finding absolute extremes
Let $f$ be a continuous function on a closed and bounded interval $[a,b]$.
1. Find all points in $[a,b]$ where $f'$ does not exist
2. Find all $c \in [a,b]$ where $f'(c) = 0$
3. Calculate the function values in the previous points, and in $a$ and $b$
4. The largest value is the absolute maximum value
5. The smallest value is the absolute minimum value
# Local Extreme Values

> [!info] Definition
> Let $f$ be a real function with domain $D$. Let $c \in D$. Then $f$ has a **local maximum value at $c$** if there exists an open interval $I \subseteq D$ containing $c$ such that
> $$
> \forall x \in I \Big[f(x) \le f(c)\Big]
> $$
> and $f$ has a **local minimum value at $c$** if there exists an open interval $i \subseteq D$ containing $c$ such that
> $$
> \forall x \in I \Big[f(x) \ge f(c)\Big]
> $$


> [!info] First Derivative Theorem
> If $f$ has a local maximum or minimum value at an **interrior point** $c$ of its domain, and $f'$ is defined at $c$, then $f'(c) = 0$.

With this theorem in mind we can determine the following:
If $f$ has a local extreme value at $c$, at least on of the following statements is true:
- $c$ is not an interior point of the domain of $f$
- $f$ is not differentiable at $c$
- $f'(c) = 0$

> [!info] Definition
> An interior point of the domain of $f$ where $f'$ is undefined or where $f'(c) = 0$ is called a **critical point** of $f$.

A critical point need to to be a local extreme:
![[Pasted image 20240925113203.png]]
