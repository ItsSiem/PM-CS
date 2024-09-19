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