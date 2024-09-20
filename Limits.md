# Simple definition of a limit
>Let $f$ be a [[Functions|function]] with domain $D \subseteqq \mathbb{R}$. We say $$\lim_{x\to c} = L$$ if $f(x)$ tends to $L$ whenever $x$ tends to $c$.

- The limit point $c$ does not need to be an element of $D$
- While $x$ approaches $c$, it must be an element of $D$

# Replacement theorem
>If $f(x) = g(x)$ for all $x \neq c$, then $\lim_{x \to c}f(x) = \lim_{x \to c}g(x)$.

This theorem allows us to alter the function to find the limit, as long as it's output remains the same as the original function at any $x \neq c$.

# One-sided limits
>We say $$\lim_{x\to c^-}f(x) = L$$ if $f(x)$ tends to $L$ whenever $x$ approaches $c$ from the left, and $$\lim_{x\to c^+}f(x) = L$$ if $f(x)$ tends to $L$ whenever $x$ approaches $c$ from the right.

> If $\lim_{x\to c} f(x) = L$ exists then $\lim_{x\to c} f(x) = \lim_{x\to c^-} f(x) = \lim_{x\to c^+} f(x)$.

Based on this information we can conclude that the limit $\lim_{x \to c} f(x)$ does **not exist** if any of the following things is true:
- The left limit $\lim_{x\to c^-} f(x)$ does not exist
- The right limit $\lim_{x\to c^+} f(x)$ does not exist
- Both left and right limits do exist, but they are not equal

# Limits to infinity
> We say $$\lim_{x\to\infty} f(x) = L$$ if $f(x)$ tends to $L$ whenever $x$ tends to $\infty$, and $$\lim_{x\to -\infty} f(x) = L$$ if $f(x)$ tends to $L$ whenever $x$ tends to $-\infty$

# Infinite limits
> We say $$\lim_{x \to c} f(x) = \infty$$ if $f(x)$ tends to $\infty$ whenever $x$ tends to $c$, and $$\lim_{x \to c} f(x) = -\infty$$ if $f(x)$ tends to $-\infty$ whenever $x$ tends to $c$.

**$\infty$ is NOT a number** so even if $\lim_{x\to c} f(x) = \infty$, then the limit $\lim_{x\to c} f(x)$ does **not** exist!
Both of these statements are true:
$$\lim_{x\to 0} \frac{1}{x^2} = \infty$$

$$\lim_{x\to 0} \frac{1}{x^2} \text{ does not exist}$$
# Standard limits
$$\lim_{x \to \infty} \frac{1}{x} = \lim_{x \to -\infty} \frac{1}{x} = 0$$
$$\lim_{x \to 0} \frac{1}{x} \text{ does not exist}$$
$$\lim_{x \to 0^+} \frac{1}{x} = \infty \text{ and} \lim_{x \to 0^-} \frac{1}{x} = -\infty$$
# Calculating limits
When we are asked to calculate a limit which is not one of the above mentioned standard limits, we must calculate it ourselves.

## Well-behaved functions
Functions like polynomials, exponential functions, logarithms, sine and cosine are **well-behaved** in the sense that a limit to a point $c$ in the domain of the function $f$ can be calculated by direct substitution: $$\lim_{x\to c} f(x) = f(c)$$
## Limit laws 
If we assume that both $\lim_{x\to c} f(x) = L$ and $\lim_{x\to c} g(x) = M$ exist, the following rules apply to these limits:

| Name                   | Rule                                                                           |
| ---------------------- | ------------------------------------------------------------------------------ |
| Sum rule               | $$\lim_{x\to c}(f(x)+g(x)) = L + M$$                                           |
| Difference rule        | $$\lim_{x\to c}(f(x)-g(x)) = L - M$$                                           |
| Constant multiple rule | $$\lim_{x \to c}(k \cdot f(x)) = k \cdot L$$                                   |
| Product rule           | $$\lim_{x \to c}(f(x) \cdot g(x)) = L \cdot M$$                                |
| Quotient rule          | $$\lim_{x \to c}\frac{f(x)}{g(x)} = \frac{L}{M}, M \neq 0$$                    |
| Power rule             | $$\lim_{x \to c}(f(x))^n = L^n \text{, with } n \in \mathbb{N}$$               |
| Root rule              | $$\lim_{x \to c}\sqrt[n]{f(x)} = \sqrt[n]{L} \text{, with } n \in \mathbb{N}$$ |

## Indeterminate forms
We call a limit an indeterminate form when applying the limit laws leads to an indecisive result.
This most often occurs when dealing with dividing by zero or dealing with $\infty$ and $-\infty$. Here is a list of indeterminate forms:

| Limit law       | Limit                               | Notation                                          |
| --------------- | ----------------------------------- | ------------------------------------------------- |
| Difference rule | $$\lim_{x\to c}f(x)-g(x)$$          | $$\infty - \infty$$                               |
| Product rule    | $$\lim_{x\to c} f(x) \cdot g(x)$$   | $$0 \cdot \infty$$                                |
| Quotient rule   | $$\lim_{x \to c}\frac{f(x)}{g(x)}$$ | $$\frac{\infty}{\infty} \text{ or } \frac{0}{0}$$ |
| Power rule      | $$\lim_{x\to c}f(x)^{g(x)}$$        | $$1^\infty\text{, }0^0\text{ or }\infty^0$$       |
To go along with these indeterminate forms there are also some fake indeterminate forms. These look alike but they resolve to a single value.

| Limit law     | Limit                               | Notation                               | Value                                                             |
| ------------- | ----------------------------------- | -------------------------------------- | ----------------------------------------------------------------- |
| Sum rule      | $$\lim_{x\to c}f(x)+g(x)$$          | $$\infty + \infty$$                    | $$\infty$$                                                        |
| Product rule  | $$\lim_{x\to c} f(x) \cdot g(x)$$   | $$\infty \cdot \infty$$                | $$\infty$$                                                        |
| Quotient rule | $$\lim_{x \to c}\frac{f(x)}{g(x)}$$ | $$\frac{c}{\infty}$$                   | $$0 \text{ for any } c \in \mathbb{R}$$                           |
| Power rule    | $$\lim_{x\to c}f(x)^{g(x)}$$        | $$\infty^\alpha$$<br>$$\infty^\alpha$$ | $$\infty \text{ if } \alpha > 0$$<br>$$0 \text{ if } \alpha < 0$$ |
## Conjugate Trick
$a+b$ is the conjugate of $a-b$ (and vice versa), we can use this in combination with the following fact:
> $$(a+b)(a-b)=a^2-b^2$$

To get rid of some indeterminate forms, see the following example:
$$
\lim_{x \to 7}\frac{\sqrt{x+2}-3}{x-7} = 
\lim_{x \to 7}\frac{\sqrt{x+2}-3}{x-7} \cdot \frac{\sqrt{x+2}+3}{\sqrt{x+2}+3} =
$$
$$
\lim_{x \to 7}\frac{(\sqrt{x+2}+3)^2 - 3^2}{(x-7) (\sqrt{x+2}+3)} =
\lim_{x \to 7}\frac{x-7}{(x-7) (\sqrt{x+2}+3)} =
\lim_{x \to 7}\frac{1}{\sqrt{x+2}+3}
$$
now we can fill in $7$ for our $x$
$$
\frac{1}{\sqrt{7+2}+3} =
\frac{1}{6}
$$
## The sandwich theorem
> If $\lim_{x\to c} g(x)$ and $\lim_{x\to c} h(x)$ exist, and they are equal (say $L$), then $\lim_{x\to c} f(x)$ exists, and it is equal to $L$.

For this it to work it is important that 
$$
g(x) \le f(x) \le h(x)
\text{ for all } x \ne c
$$
![[Pasted image 20240920114049.png]]
## Getting rid of indeterminate-ness
### Limits involving 0
If $x \to 0$, factor out the lowest power of $x$
>[!Example] 
> Calculate $\lim_{x \to 0}\frac{2x^2-6x}{3x^2+2x}$.
> The lowest power of $x$ is $x^1$ so we divide by $x$:
> $$
> \lim_{x \to 0}\frac{2x^2-6x}{3x^2+2x} =
> \lim_{x \to 0}\frac{2x-6}{3x+2}
> $$
> Then we fill in $0$ for $x$:
> $$
> \frac{2 \cdot 0 - 6}{3 \cdot 0 + 2} =
> \frac{-6}{2} = -3
> $$


### Limits involving $\infty$
If $x \to \infty$, factor out the highest power of $x$. When filling in $\infty$ we must not forget the [[Limits#Indeterminate forms|indeterminate forms]].
>[!Example] 
> Calculate $\lim_{x \to \infty}\frac{2x^2-6x}{3x^2+2x}$.
> The highest power of $x$ is $x^2$ so we divide by $x^2$:
> $$
> \lim_{x \to \infty}\frac{2x^2-6x}{3x^2+2x} =
> \lim_{x \to \infty}\frac{2-\frac{6}{x}}{3+\frac{2}{x}}
> $$
> Then we fill in $\infty$ for $x$:
> $$
> \lim_{x \to \infty}\frac{2-\frac{6}{\infty}}{3+\frac{2}{\infty}} =
> \frac{2}{3}
> $$
