The derivative of $f$ at point $x_0$ is equal to the slope of the [[Tangent|tangent]] to $f$ at this point $x_0$.

We can find the tangent to $f$ at point $P$ on $f$ by looking at a [[Secant|secant]] that goes through $P$ and $Q$. The tangent to $f$ at point $P$ is the limit of the secant when $Q$ approaches $P$.

![[Pasted image 20240925092648.png]]

The slope of the secant through $P$ and $Q$ is 
$$
\frac{f(x_0+h)-f(x_0)}{h}
$$
The slope of the tangent to $f$ at $x_0$ is the limit of this function
$$
\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}
$$
> [!info] Definition
> Let $f$ be a function defined on an open interval $I$, and let $x_0 \in I$.
> The **derivative of $f$ at $x_0$** is
> $$
> f'(x_0) = lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}
> $$
> provided this limit exists.

The derivative of $f$ at $x_0$ can also be denoted as $\frac{df}{dx}(x_0)$ or $f_x(x_0)$.

When this limit exists at $x_0$ we can say that $f$ is **differentiable** at $x_0$.
It's important to realize that differentiability is a a local property.

>[!example]
> Let $f(x)=|x|$.
> This function is differentiable when $c \ne 0$, but it is not differentiable when $c = 0$.
> This is because 
> $$
> \lim_{h\to0}\frac{|c+h|-|c|}{h}
> $$
> does not exist.
> $$
> \lim_{h\to0^+}\frac{|c+h|-|c|}{h} \ne
> \lim_{h\to0^-}\frac{|c+h|-|c|}{h}
> $$

>[!info] Theorem
> If $f$ is differentiable at $c$, then it is [[Continuity|continuous]] at $c$.

# Rules of differentiation
Assume that $f$ and $g$ are differentiable at $x$.
Sum rule: $\frac{d}{dx}(f(x) + g(x)) = \frac{df}{dx}+\frac{dg}{dx}$
Difference rule: $\frac{d}{dx}(f(x)-g(x)) = \frac{df}{dx} - \frac{dg}{dx}$
Constant multiple rule: $\frac{d}{dx}(kf(x))=k\frac{df}{dx}$
Product rule: $\frac{d}{dx}(f(x) \cdot g(x))=\frac{df}{dx}\cdot g(x)+f(x)\cdot\frac{dg}{dx}$
Quotient rule: $\frac{d}{dx}(\frac{f(x)}{g(x)})=\frac{\frac{df}{dx}\cdot g(x)-f(x)\cdot\frac{dg}{dx}}{g(x)^2}$
Chain rule: $\frac{d}{dx}(f(g(x))=f'(g(x))\cdot\frac{dg}{dx}$
