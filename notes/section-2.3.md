# 2.3: Differentiation Formulas

## Constant Functions
- The graph of a constant function, $f(x) = c$, is a horizontal line $y = c$. This has a slope of 0, so our derivative is $f'(x) = 0$
- $$f'(x) = \lim_{h\to0}\frac{f(x + h) - f(x)}{h} = \lim_{h\to0}\frac{c - c}{h} = \lim_{h\to0}0 = 0$$

## Power Functions
- Functions $f(x) = x^n$ where $n$ is a positive integer
- The Power Rule: if $n$ is a positive integer, $\frac{d}{dx}(x^n) = nx^{n-1}$
- Examples
  - If $f(x) = x^6$, then $f'(x) = 6x^5$
  - If $y = x^{1000}$ then $y' = 1000x^{999}$
  - If $y = t^4$ then $\frac{dy}{dt} = 4t^3$
  - $\frac{d}{dr}(r^3) = 3r^2$

## New Derivatives from Old
- When new functions are formed from old functions by addition, subtraction, or multiplication, their derivatives can be calculated in terms of the derivatives of the old function
- The derivative of a constant times a function is the constant times the derivative of the function
- The derivative of a sum (or difference) of functions is the sum (or difference) of the derivatives
- $$\begin{align*}
  (f+g)' &= f' + g' \\
  (f-g)' &= f' - g'
  \end{align*}
  $$
- The sum rule can be applied to any number of functions

## The Product Rule
- If $f$ and $g$ are both differentiable, then $$\frac{d}{dx}[f(x)g(x)] = f(x)\frac{d}{dx}[g(x)] + g(x)\frac{d}{dx}[f(x)]$$
- Written in prime notation, $(fg)' = fg' + gf'$
- The product rule says that the derivative of a product of two functions is the first function times the derivative of the second function plus the second function times the derivative of the first function

## The Quotient Rule
- If $f$ and $g$ are differentiable, then $$\frac{d}{dx}[\frac{f(x)}{g(x)}] = \frac{g(x)\frac{d}{dx}[f(x)] - f(x)\frac{d}{dx}[g(x)]}{[g(x)]^2}$$
- Written in prime notation, $(\frac{f}{g})' = \frac{gf' - fg'}{g^2}$
- The quotient rule says the derivative of a quotient is the denominator times the derivative of the numerator minus the numerator times the derivative of the denominator, all divided by the square of the denominator

## General Power Functions
- The quotient rule can extend the power rule when the exponent is a negative integer
- If $n$ is a positive integer, then $$\frac{d}{dx}(x^{-n}) = -nx^{-n-1}$$
- The power rule is true for any real number $n$
  - If $n$ is any real number, then $$\frac{d}{dx}(x^n) = nx^{n - 1}$$
- Differentiation rules allow us to find tangent lines without having to resort to the definition of a derivative.
- It also enables us to find *normal lines*, which is a line to curve $C$ at point $P$ which is perpendicular to the tangent line at point $P$